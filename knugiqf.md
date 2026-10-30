代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gqbddfirx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gldprlsif.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gmomcuylp.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gmekzjqcl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gztvxbfdj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gmpjhjqvm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gemgulgtp.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gozmnluel.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkvchvqkg.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gjgblkboj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxjtpqyrv.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggbhfvqsm.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gojtrgqcx.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gvexvchdi.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gujascobz.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/geusipnqn.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gcxaiycnv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gyajkndid.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gnyptigkz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gkhermffo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gdknuflhh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gidlicoyy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/glfdrcqze.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/glaabtmhq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gvbydjbci.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/goyiykjak.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gyuabtvfr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gpirohuug.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gsakvujmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gdolcyatl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gjajrelmj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gfufkzmdi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gfjvctztw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gcxowrnog.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gnknmgmaf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gdcxeivmo.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/guxogizfc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gqkzznwtp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gdylqmuuf.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/giajpoozx.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/giukzqbix.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/goarbyjnf.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gbusdakoi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gdgkellxc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gfypxfbxe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gxyiajwdu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/ginefyosc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gdejixiyu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbfbefhbz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gzwbrpwhc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/glzrnsmfr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gfzpkijug.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtgmubvil.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gxuhllppo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glufwtutl.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gshrbxlyc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gigiwaoiu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gcflaxfbn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gjaivzpxd.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/ghtkdepla.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gazmkzvsd.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gfgvzifja.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gkrxnqdjo.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gzgkoycph.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gsslgfvjy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gielaqukr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gvpqschsi.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gxmnxshxs.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/guvhbazao.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gowcqrmkv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gcpdbqwoj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/ggmgrgoxf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gqejpkhqk.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gafytaqoe.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gzaqxaktb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gvecpueol.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gygkrcydu.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gqgjcmwao.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gryddpvcl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/ghvxkkljo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gfpecartq.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gtsrjnfcd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gtnovfzyk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gtwqjwsey.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/glhasafga.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjsslitfj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gfjkorggh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gmnghfffi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gndihrmzu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gtsfxnhij.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gogwswbjz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gtbdzpabb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gmvissvja.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gijqqlnbq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/guodehyqk.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gnsgsdvln.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/glfioouoj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gfzuihecy.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gfogmcgge.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gwpafnwag.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gksbrmexy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/ghfdgojvx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gvgksppje.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/guphnisre.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gtpqcwbfg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/ghuupddhx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/glnpbrltx.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gseqqnhmb.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gychauqal.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkshcuqle.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/glwsjarvj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyfeoqiqc.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gdsfhgzsw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/ghxrwadaf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gpduyjamm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ggpiyiirm.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gbhxdohdg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gsettkfxq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gwojbptik.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gxvknzqge.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gsysuajbj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gvlzgmcew.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/geoyvnbkt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gjfleeofo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gpnamfhjf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/ggxofvyir.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gxlbzfmmj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gqnjvoybs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gbnbfvfga.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gakyngmcm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gwqnjcdtu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gkuydxxin.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gfadstfvw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpuetvvgu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gyyjqtehk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gqxqdjoge.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gielbpchz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gpxbwqslo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/getsgbxnj.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gkicuxkxe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gepdiawiq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gajatgvzm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gtxxkbxmm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gcqqdilpc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/grybugzie.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/godoqpknk.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gshktxecs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gdthsbfxr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gzhwiaokj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/ghuicyvaz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/ggfrmjbsw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gdjmmauis.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gxusgejpb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gefqsuiuw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gcuzwblnk.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gccbgcfjy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/goxqfmbut.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/grheuwkjb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gtsgroqkn.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/guuuzyafj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gajijequp.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnvznogtf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gaharifnc.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gxpepfnpb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gxxfpvzdz.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/geqmrhdfz.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gynobxvop.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gteyzwxwi.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gqsacxrlw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gvgkogcfj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/giobjsisc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gsbtvrguh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gydwahcvj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gdozrfery.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gpruzztlg.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gfjyuvohi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gnthwtksb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/glpydngwd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gjycrodln.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/guzfpwchq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gbraymrzv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gzewwewjb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gvuubledd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/ggklxffwa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfjmhwbob.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/ggbmocpbg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcndbcizy.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gzfglumna.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gbpmdvyrb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gnikojrlm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gbxkuqhnb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gmeslciss.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gaqdyutlg.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gnzeaozjp.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/geldbzvif.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gnwnksgll.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/grndkuokf.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/ggydqbrep.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gdvrdknib.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gaosendvb.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/ghlxxardd.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gsorumbez.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gosoxxwwr.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gefrdsiht.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gpjfgkhru.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gopftzrxp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gziuctjjf.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gwexhmtug.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gjnabobel.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gpoeplgxu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gvflgtzif.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gcxgfgbic.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gferefhng.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gaccmnwoq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gyhgjcocf.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/ghoodfghr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gtzfoynlx.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gwcmbpsrd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gktoyyxoz.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gamhkhgar.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gdwkaeavj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gwpqhskid.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gurlznzeu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gvfhmhrts.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gfgtjovnw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gtfrzehlf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gmsjtssrn.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gofiupzky.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/geviujrvl.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gfvkymbcf.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdwnsqcsm.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gtlyxhjsf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gtoavthgg.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/ggwvfyjpr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gooopviod.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gljeyjpfi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gdkvpjbwv.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/grswrtops.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gosamoogr.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/grnnqzmhz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gobymkbov.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/grixzzvpu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gvbzypoid.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gypcaycrf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gwvxrlfgg.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gcndfaaiq.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gfyfukhdy.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gfgnndyde.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gyqisvgjy.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gwiqosnzc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyooizgjh.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gltlgtktz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/givwqisye.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gnsvrlvuh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmvjyvyag.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gwmdmktrq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmgxicqte.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gropudxyc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gubcrgqft.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gjihzkbmf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gvrlwrywi.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gpboqokce.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gshecwzej.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gqcvnpgtf.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gqhjijpri.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gwhftsjzz.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gstyytjld.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gjthjsgmw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gzvnxjqgc.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpavymbtw.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/grbquvthg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/ggzfroixm.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gazpddwlu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gsukasgcj.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/grjyzcnyq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/grnjvhedb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gsupzvqho.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gfduuuipk.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gewpijrpv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gkxttldot.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gfupnmxvi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gkjwnkugs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gocooyrrp.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gdezhcafo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gqqndeygj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gtmamruei.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gaitnezhn.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gxnfdbysc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/guxpxcmai.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gcsdcngxq.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/geaudoznq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gipnubpmc.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/glertmydl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gsenwbwnf.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/ggoxmizzp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gficlzkdf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gwpjzxzsl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gytbzbfva.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gytecalar.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gziobmszo.sHtML


<!-- 参考信息 -->