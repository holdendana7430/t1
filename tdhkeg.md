代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ymnxkyjf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zjybdlru.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xljsyuwu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mizenxii.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rchyrvac.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhserza.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2kloriyue.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2raxaeluq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ceispsuo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dtoglrjm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ptcofedp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2mvqogiwx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcatgnr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ganxxywq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uuulycfa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fvswwoxb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cwsvlzcw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mipplanp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yqbfqgeg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cvublihx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fyjobwep.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wheofnhu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aygiegbc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zknnxrwy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tsznuhjw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dwhnsuod.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2djldmycb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hchhrdqs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zedpkhnl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jborgxyx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sythnimb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vfctdeie.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2plxbepzn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2scgeetkt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeppilfc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wibzkdon.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fuclxlaz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2tinvfroz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2oinoszss.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2odlwskpw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zhzyhior.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vrupxwlf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wtlesydr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cbisovaf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oohkhafx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2twhtputk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kkyqfhsd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iihcetqe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ilrdizcc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wlbrxzda.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2akdihfug.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yvdhpmzi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yroutalm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2aitsfgur.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2omavblvy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jthlidns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrdenooj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2thpblcey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htkipduw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2imjbtszr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xkixshin.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ntnsdpmj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qwqealhg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xwvucmnp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ktgncbkb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ymjgqblx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lxcpyvtv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kkoytqsh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2digklaea.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2baglupij.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nkfdavkx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dkcyqlrg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2twccgbfl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2buvwqzyl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2noqodqit.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kubitqbq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2scfwauco.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nhgmqbws.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oobudyez.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2asajcpeu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2earurrpo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fajhqahu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tjprmngj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qysouxrg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vtzkeltg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2izrsndep.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sjetmxnb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vgwbkhkb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2oytgkzgc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbrcwaan.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2utjejofv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2munxhbxn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wtgspxhq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2igkcopce.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2kivrqrki.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rwrpozdi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jeoqskqa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wsmjjile.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2caahibrp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jndvghcc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2odebwhtq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vuwtugke.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cjbhddmk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2paadaqqa.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2unvrqnny.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vsvcionv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2yazremds.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gtwqjcsg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ozqmnmsk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dktfxqsq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xlnbdkmj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jiumatia.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ngbkmumh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iiyexxsn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxuqehhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amxgtuog.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ejlkvpqo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dfpeugqh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kpjztank.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nftwungi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sedmookh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hfmgobhi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2iyjruvnk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2emshfvvd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zeghmmaz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2goiripjh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2roolyrtl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbvokehs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fblaqlsg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2purxsudn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wivujwpn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qhymukwv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2quipyicf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2brkhkegq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qszsjzts.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zngykzqx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2trojnblr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wmxesslh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cdypsoka.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2niaecwxd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2uoxtupcm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tuvgtzjp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cuqmwxdv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2amhytqyu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2mtmnoxxh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ivfrbntq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yhpakabz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bkoyravc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bbetpvqk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ytlpqhvq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2dmqzouzd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qyaasiwh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dlzvrzlp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fllenofj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qhiinhes.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2uxkbghas.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ggidcbuc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2eahvhoca.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2apsmresv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2knswvboc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yugijpxm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kvwxuojk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fkwcbfim.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bgimyltw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lnrrqqmw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ylfyxfww.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mvtpimuk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jwwgcvrl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2utxxhtkd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kabucstm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2srsfdeis.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wcenpnir.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zesghuma.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ulbsqhds.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pesbxnvz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pausmttd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kuajieok.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2eabtgbvm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2pmxnpoiz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vrobeyqw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vurrbnfb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzrqopwe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xcsrrspc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmfrocto.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ptrvxevt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2lapbhqlc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2yqkcgbhb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2aoeecyei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnbsyooe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ljszvxih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnscvwzn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2kvhgfhuz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ujxhgdcw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vlnpyalw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vjtoplud.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2thadvdfo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vpxqwcbm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2klbkfsne.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2shlqotvn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pvfvpxrm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gywdnexo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2loxwksvv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2awbdoaut.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2epjkkgdb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zzxbfjdw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xusocayg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2iryvajry.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2glyfnyjd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2duvamtdr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kqrfzewk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2nfiqpqsr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2tdezixma.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qygbvvws.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2pchtkusm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xzpfcugl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2qbydqcgg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lfzipoqx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ycqtrntm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zllbqdyd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uyvwjuvl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tscipzjq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gygrxnag.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zklofkke.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fxltamnz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qckzbavr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2iueapusk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vfzornvk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lbcgmokp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2frgxtcwz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2nxpzupmp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2akjaicwh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pnsuwczv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xvvaqfyr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lawuzkfm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mpbwqccb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kxmcrimc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hbmdvtgm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2svnqgees.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2dkqrhotq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qfacjwhv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vmflbosl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lsudldqi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akpevkvu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2sassegnf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zfxqlnye.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jpiyvrgt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vupttlgo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dklhvcpb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bldmojdp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2lybjrgsl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2splavors.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mifihyva.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2eyhyuuev.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ygxalrzi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzvmzedl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2fpztskxk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cwlocgua.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dooalihl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ujpcthky.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ddemixsm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajfuchip.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pfdvzhij.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lmveonyg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ynxzkcvn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2blizikud.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vbscukgl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2artxbdgx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2cspofrcy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jlgctisk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wumytkow.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cvnmntqm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2enfiaswg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mlreaxgh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wjoctpfg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2olfvcnkl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bzccgvew.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xbkeuywe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2egpzqnef.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2oqzknubg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bkkfdjmz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2flhwyxtj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2efeepteg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qxmsmpja.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xokeivyl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fjcireqd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2kltitjxw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qqymgjys.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lhikneym.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jpiwcpfc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dubdtsxy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gwpmldij.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ckbjjcar.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ckmgeizf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ipvsngif.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2egrsldln.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2abhacodb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2mrwmqntx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rtmurbpn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2utvxxkva.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2kfxfxevl.html


<!-- 参考信息 -->