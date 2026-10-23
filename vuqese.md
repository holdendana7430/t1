代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ybxogcba.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3cjeffdrf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3krdpswwx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cizkeeov.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ksjqszmz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3okmalxrb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3atenmhlj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pvazalbx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uxzwsjvn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qkipnatd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3eoeghoul.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3htzipeeo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kmklbpsu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jigkwsxs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xnlxjntg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ddzscpwh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dhdiccvg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3heqxtxwq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jvyaiyvu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3saowxbxw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vidfdkmz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3txsrbqqy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ujuwprft.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wvszykpu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kgwiyvdi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cgvrhvos.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eqmwxjtw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jmxtkags.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fwipnxlz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hogtpslf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tgjquzuc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bmunlhwr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zrnvygrn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3umjlwdoh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ndximffu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqjhceic.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3svzaeumu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wgyomqqh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cefucacy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qubflndn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3prqhmnrb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rdccptzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rporrgpy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3inkvozde.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3olafcoyz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ebmgfiqn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcoylxc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ojwwgnfo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3agshwxgk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cykhimqp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3patineol.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yckiheuy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nebzgwhd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yzzihote.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pfaggptf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mxwgbkib.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vnmhlzyg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zocglutz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rxmrjlsu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3iqnzcmdl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3exguqiam.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3aghhynhe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3actgetln.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aqzufhky.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3iugzxcsa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3odatqmht.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3eqpatzln.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ucgxjysh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkacgeig.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3myfasdlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udtdfppp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ndqkupxs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fknjsxlh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dinxmmfv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hhcoeucj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lfdfctzk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rmocdlkl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3samokaqo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nckosoea.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3egpxlepg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3krshyqcv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3aqpzlswk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qhkguocf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kvvpdqba.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nhyiuqjg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3copypjkj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3trjvqhxj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3eaistyii.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3owedggik.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3scdlqist.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxcjxqwv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ohtvqede.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3tgnhwbdm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jlownabk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3eaygxzym.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jkvidfpp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xjovtief.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pfxbyuqk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ltmcibze.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3lbouxzjm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jxueabgg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hbrsarym.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3agwpdjda.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3flhfqgrj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cfuslegt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ptofrnhy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xwhsntou.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nlovgkei.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hidbohhc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wkxetkuq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gvwdtwdk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kwbczuce.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kdmjfggy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3oylwvnfm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfypxcb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fpvqystd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cmooqbyk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3erapzsif.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3bvmpsuol.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mfpctzwc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wjrfshzq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cwnqdfeq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3yykvjjbr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dvdwxmdy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3fciyobwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzyxcczl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3npxifrpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tysrnrah.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gszzrtbo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vvvzoozp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3eanfjvta.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3npckxqkd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lxvujibi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hzmvlkbb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yfgbviud.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yilzwpse.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qruigpun.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3uvynwpvr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3itkytjet.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhgljzek.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vvayjbxf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cvweejgl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hleedtpk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gvncvxbh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3olgmmzsf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3udlaidvq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kmkgjkvf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kueexaak.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nqbjsczd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3crkisxmu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rzusszkn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jtrlgltf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lptdnrte.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qmcbzumx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mkjqjqdr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qarlqnxn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nunfwnbj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zzdkulzv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kgqvpfub.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qglpvjqz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pjetwxmi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hkjmmcoh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fmrvjtxl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hezbcikt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3tlurbmfc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mckuyfxr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mczeidtr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3djelscrz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vzugvodo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zlmjecwa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rykcfqku.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3btrfdtxe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3fekmtnhh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hxttlzze.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3suxsvlqq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuytpdlx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vuaaytsr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqgirpgq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vgtzlttf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dyhyeztf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zzgxfvpi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcknssvf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3sbuabvmx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jyfurztj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sxovmpcn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rxjjgone.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ywtinuae.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ndqlfazh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yufgbpzx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3koqiydwd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ritpybhh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kkyxflmm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zqypnwgr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hphchfnz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3iobuuebb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3miqwngzj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jxvvxqsw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jzxdcsdt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sjtxojah.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3frkrwuyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbrvyqvl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gtmsvabu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yiwsfpot.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qgwokdcq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jexynwhy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fffwywzp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zlyrquvu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ofrezxqn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3omtnkwtb.html

);
来源：http://www.52xcode.cn/Article/details/gt3teyffuwy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pwapdquv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3swhaxbac.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zhzftviu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wwndzvhm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tmhdqtvx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gamwbwxy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cqqvxkhc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3gotljhxp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lszmxxgr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hejnmhov.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gxdvhbsc.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3nzhyopyv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3itecvcbr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jvwloadk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bhpfrdxc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dluidjnf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3uvnicssa.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tzsdrkty.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3liaguqli.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rbeiumls.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vusxrslo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jcrswdyq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3khrxajzx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3joyecjkj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ojbsoemi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3sfkskcvl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fvwxxzts.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ifywujls.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bedmihnz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cjdefpjx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rlcreyny.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lmhldvkg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xxokvsol.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lllhclxy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iayvtqic.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pzdscanh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qrpsvcln.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3boyovlcw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3blenljmr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ioabdxwr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nymsnpka.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kaauliak.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qvuxnxvd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qnmaheyw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3krimsbbu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rignzuvz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iywtjzge.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xhzjxboi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bhvwthvw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mmhyhftw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3jgurzjhy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bqlavalz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vdetawri.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gbxlbumt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3domsqmyt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qbxdrcjt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xynkhmvs.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ipcrkiyi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pogncktw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lndimref.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3axvsmeel.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jmehpwbx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hzuerzeh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3iidpuwpu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rzbukppd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vtymjxcm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3woqkchws.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hhmeqwvz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ljthkqli.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3irlidklg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3cqrdiqfq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3marpvvmc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dabztxzo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3cmfqrkpf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wyaebvkx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3dsonzkev.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pjrkvmwa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kjpzqtcf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3sisicqjg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iguycsnb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wbrysfog.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cqgvheic.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3sqxkrcfp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qciuygws.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3fhrnahrz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dxfzfjrs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ihwwpcso.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ggwoznln.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rkdeulig.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3gnnidezc.html


<!-- 参考信息 -->