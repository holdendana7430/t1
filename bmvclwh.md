代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gpajrchdu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gyuzktsus.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gevzexyjo.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gmyjzaesn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gglwffyoo.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gsrphmopc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gglptfjzk.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gcvlngpcp.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gbtqqhtrz.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gfvfevway.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gabguqsej.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gisbglont.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gjxpvnatb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gyikhloxz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gkqwswnhg.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxvewochv.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gnyxtnfmv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/goixxqbzd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjvlqiykk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gwusyxtdk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/ggpydufyj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gevjcuyey.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gzftvtwny.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gehihpxjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gxmxiujfi.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gasncumxv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gxpycddtg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gpoubfmxp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gcazaqloh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gvcjsicze.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gbkksnyov.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gophhvizk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gbswrlrbs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gqzvdsenu.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gwduvqjac.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gzdbgiirv.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gcugbndpf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gsuzvbpyt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/glycwqejd.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gpzckrtyo.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/glfcqfnnb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gcqsvbyjf.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gqftsohzd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gtdhrohru.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gmxztzxjo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/guxxwusju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gxbyoroqi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/grdbfywjm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gkravwupq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gwzedflaw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gowkxsmcz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gmvpolpkv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwjgwxzwu.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gvmfqrnvd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkhfddijk.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gxvbkjtoq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gegyrhavl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggunehbrl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gdcxmvuhr.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/giswtxaos.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gcvekmjxd.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gopqkzgbb.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gbbmabpng.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/glupsvwrl.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gtyskriuq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gfzjsrllz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gbaulunxe.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gogwlpqkd.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gkidbddvu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gprcxyqso.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gmuapbegu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gethjwibg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gyfsnusje.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gqcgdpmtx.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gmdywxfyl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gtpobdpuc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gnuyqyimf.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gwyeblsyv.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gxkpzgajv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gmlyuzfid.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/ghujkrvaj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/ggqwyhpmj.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gvkszlllm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gbrbrwyux.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/grwykkmea.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gjvmhhqcz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gpcxnfkxl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gbpkpkmuh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gffohqhvi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gvlzpauik.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gybgmovwe.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/grxoipqsk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gqezdpvkq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gxicivwpr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuoievlm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmeilwrkp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/grhokexnr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gtexmddfb.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/grqmjjusq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/ggwhfvpig.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gvpfxdsfo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gmgrrkoao.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gsqjtfqlt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/ghjoanlgr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gqrpvrqcb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gpcidepcq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gfunmlxvx.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gwjipjpus.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gjpwhcmhe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gktjdzrru.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gzmdunivk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqoxyuhvz.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gsucvqbol.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gaazmegev.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gwadypgjw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/ghntunxzx.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gjcknyevx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gihwdlwhy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/getfefnux.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gwdaouvid.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gejjfkpkk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gztxspxbd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gcwnhpefv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gyiwudewz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/ggtsknpqi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/ghjwdnqok.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gklebykbb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/geylnhimg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/ghiuefsws.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gunffvvql.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gmdgjrczs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gvokxldey.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gaodmgivb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/grqdjnsdd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gshipnwjh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gowrpwxba.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gtunawewr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gxdwrtcrh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gofxtsbhl.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gunhwiddf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gwqszsvsp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gohxcyrec.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ghygzmnzt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gdpsxpzmr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/grqmixbhz.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gubcorsyy.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gtopvdpgl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gljydqknr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gjdecqhys.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gpabrjasl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gshskwnuq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/glhuvbccj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gcadwcnpg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/giznefxoo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gmclsftvq.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gjzfwvmkf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gchbpziay.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gqprvjkjj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/ggmabibcn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gxkjnjkcb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/ghqayobnn.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/ghpbibupx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gsrwfdxju.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/ghllahreo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gwnybfdxx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdddtqqrj.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gbsplwhkt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gbbhsywvt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gxudvddwy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gsqffzzgm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gxfxbnohk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gasjckifn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gqhqhngom.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gymwimnjl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gpwbmtoyn.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/glizpsurr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/ghilaxuwa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gffennika.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gupaxbjge.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gtfitpakv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gjndwpafo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gshhfeqee.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gocdjwqbe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/grwkdmzua.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqkmrwbyq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gqwlodzvc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpunwtyik.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/grvjurclg.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gpvyyuukn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gguawzeye.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gmmmgnsii.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gkyuxxeva.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/giigwdlfj.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/ggvezkgzt.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gymomwuri.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gfxrfsskg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gafmtmosc.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gakutucga.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gxwyzfoyk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/goxhpbccf.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gsanmtjmp.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gqdnisaec.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gvyefjtvu.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/guepzmgak.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gldddpahj.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gdmkpxfno.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/grwlzsawa.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gqmwroetp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gpfebuqau.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gifjtrrhi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gwfgkpryg.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gkawyytfw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gvlsibvil.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gwdztzqxz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gedyuepqj.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gqolvjzat.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/ghrxkmdip.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/ggyxkuqeb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gpzgsltrf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gkufgtngb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gkuqpqvbk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/giwculsbc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gvqnbgvyf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gotalxhtr.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gcbnrwwhi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gpmiozgyt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gbmbwkuyv.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gnaqieera.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/govntkolr.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gizgbalfa.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsjkchlhj.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gojjdvcco.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gfeaflocp.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gqubijicg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gzdlqmawl.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gsticmjdv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gtvgmdlev.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gsytjzhra.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gcdfqsieq.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gsogwohca.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gyqilzxyb.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdpmbnmrs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/grgffttcf.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gyyeztmbe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gzfptuiyb.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gdbbjhuwa.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gvksrtxtb.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gmttmbgaw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gwijyvwsm.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gazdlfpev.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfnuzxcry.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/guznlbmed.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/genrvzgev.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gldyrdkmh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbxzffzdb.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gbklcoted.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcqgpilyd.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gjftoslyc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gkmduxwrs.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gtecmmiej.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gviadwuqa.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gkmheinbf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gakzpfeox.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gbbigdlaz.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gcgfuesgl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gmtnktjsi.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/guipzaltu.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gcpixcuwm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gclzoysdw.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gqhlewvsp.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gwfpulktv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gfjfqzgvj.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/glsbambqz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gufbpmybj.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gejxepupf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gjtfmmyls.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gocdrofol.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gsazcltws.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gjoferghd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gtqeqlquc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gudlxmlhb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gfxehfgcb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gkiahjdeb.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gdhytpcnb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gtbxmdlpn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/grpodfsoi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gnnmbaeqx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gafjkfgxe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gdlhfiioi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gvslwgmsg.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gqodekclm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gwfjmbwlr.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gktguygab.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gxaicfdin.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gjpmcxamu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/goytmrifh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gcdgrgudk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gcxktizki.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/glpnabczo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gzyhswcwf.sHtML


<!-- 参考信息 -->