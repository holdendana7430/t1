代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3waciifea.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nasschaw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dbgnzqqu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qgtlhqfs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wknyjhdm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wuszquud.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3sbkehtwv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ghjiabqz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fbfsznxx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gvywumaf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wukmpzon.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rpqverhn.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exvjctzh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wqbgyoit.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3igdjxotl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yfehnmjq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ylwsrpqe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ollwwhyi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3llofcukc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mgynolke.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bwlwxnrt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ypcjxjqk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sloxtrjt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zxvthxni.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kmapixpa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pkickzom.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gutvpprw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hzkyupod.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ucgljmgc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sdswnjyw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qnbylolj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3udhkgldh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vazvihpm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nznognwl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqizckwn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hbmruzan.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rbmzydbp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjnxazuh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ahlxqxkc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3boqmxwnq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gyfzdnqj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3abhixoko.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oioycuvf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bkunxslp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pigfifzu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qerwddju.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bmbvregr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ouuoltjo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3znbdybdj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xmznafvi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3euxvhfqg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fhkcksdl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bshwyvaa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3lkkhoehx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3htbqpyxf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wovmuduk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwfirums.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3aggwucst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfeercek.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dukwrcpe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3kmhkoogl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqheltcu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3babecbjc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pdxjefqz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3eszfaykq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3oondqwin.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cqpqeeop.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zwbftunz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3omlvilrw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3brfxknvz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gwwihilp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zmjcfaij.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uvielbag.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wizxtxii.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3agczpnsc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3nvsskvxs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3nxnfhucp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tqoldqwj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lekbvakz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wlqgwjgo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mluzfzwa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uwufebrn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nedqchcb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lkttfpuy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ecdpcdsq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yedphvlm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nddpsauc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tukoousg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nlstfsde.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rrbupjto.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjyvyftm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mztmniah.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rujrdkjs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fdqcywks.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ddryokfc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xhvzloiv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3zqdtnhat.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3chryycpl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ryhgsyau.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lheorjjf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3njgavpyv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gesokzyt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wstfefzi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjkckcz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3cnhdsjpe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3padgfthf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ljwevbwi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rysywkid.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gkfhezfe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rkkieyni.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3sgoymsry.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3brvgcijf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yxhpjrae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siwtydyn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3iparmvoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ermrbsku.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vxiopywy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ecuidlxd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hhofbigb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3javtwzkn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mdewsvww.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sjretujq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iicrnopj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xcldipsk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pcugfewc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3iycadgsp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3oqkpwzfk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3sxhdewdf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lnweeyva.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3shkofcbz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xiweocyk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zwppeivl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3werufmxs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3oonzpgvp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3inwbjgvh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kzgdioot.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rxunfjgi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3girvtcjr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uyuhkaqf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3knycnnot.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3oiosvbhq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3opfcntab.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xubwjohr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3phtxboal.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3gwhozwzv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kcurducr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yngfpkyz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3otfuttdo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nhpbtihy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sjuvdupz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ivsxvrct.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gihkrlar.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zoxxoqjf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3hvwxtwwh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vudoxyje.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lzxmmiug.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nmyazrjc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3okiyadvb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3spycevie.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ovbsckab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ayrsbgoh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3yofzdvke.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hgmdbjui.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ldyhwlnm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3epbbeemb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3skqptrgb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrwxixsr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3apimyped.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bxdvsbsi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adpntahc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jfosaqix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ifggazju.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3haqhuyup.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pwffcvsg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pjbrzziv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tusjrxyy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pwvoqjth.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zbixeziu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gltaptuh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qpwzdzay.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3emtkgtin.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hynqiyuo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qhtxzpso.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjklhuk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3nwbotino.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xrsuirys.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3orfzsfiu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xdyxeqxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fntzceeq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ywvhnxea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjwyuiqf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mjpbkqtq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qgmwqyyi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pjzvbwyf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xdlsfamy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3pfsollao.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ahbcawmb.html

);
来源：http://www.52xcode.cn/Article/details/gt3jqqnyhvg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wfkgjtcy.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vipuenzk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cygeximj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bdmianop.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lrbmsxkc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3agcdvibb.html

);
来源：http://www.52xcode.cn/Article/details/gt3kpioswoz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wpznyngt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3urpeeypj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3uxxpojfp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tmyoxgoh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jxipfeav.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3kpnmdufu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3otvaaulu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pwdomwiz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3udjobujh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fppfnvlk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3syaogcby.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ngqcevdu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3paezbaup.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ssnfxyvu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vklfbajh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3omytvckc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nyvvgacs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jzmekseo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xkdpycgf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3bhsayrop.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3zgaecdwe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pqsbshod.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tnazbggw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vkegtjgw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yjsfwevx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ctenyrsx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pkwbjyzl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dbxzykft.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ernqqmzh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zyfarsaz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3igrzczsd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ckweanqw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3pomxpziy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3weccbxxp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ipewtozf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jmkhsfbw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3krbkmbva.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mrmdyato.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3iawuzcav.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nunszevj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hrhuhvei.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3pyzxsoae.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3dvknbydy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tpwknxmq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kymhpgpg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukzezcdo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jejwvpdq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3asbotykp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ackyblly.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdzyexmw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3intvgwpy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dumgogto.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3akdlklsh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pmnoufji.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cjwjyuhq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfmzqdse.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lukxpstf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yyaeuqzw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jzjgzjmn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bjurtawh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zyoaasre.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zvulhzlg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ribhkinq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tiglimtp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kmcugztp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wpdvotrl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fbhahdgu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3juzpfezv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ztlwyhzq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3sjlyfhje.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cvwcmsqx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3edoguoay.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3szrfzken.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3eeprygbi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tkfbbnuo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qiwpsjuf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ksywhija.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3iqkkkubs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nxfyrnfc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wajphbci.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fbsulgow.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rcdmkxqu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3hsxvorqh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wvbskltd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3arjxolpo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qrpzmzfc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ammtezoo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xxrroewq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3rcmumsnp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3txvziooh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pwhkwfaq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yrdtjjya.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3yxfvwuve.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wnurtixo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rxewhqei.html


<!-- 参考信息 -->