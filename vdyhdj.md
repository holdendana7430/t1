代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2laksjhtd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ywupalzr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cpeptkdd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bcbjvefv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2flkrqlfc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bznkeuek.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ratfrctm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2voyyqoda.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2toauavfl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wnbnhgys.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ctcgcuan.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pqejsdry.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tnvsckhv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkymzicx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2heidvnzl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2osqlkatl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zbdmdodt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhgxnxze.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vrfxyxyz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kkmmbgng.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2znoqgxby.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2quozwxoa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ogmcsuxk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qeknekcz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yzhxdgpd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vdqlngsg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qxmzjesm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmhjcqbv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2uytokcfi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zxetzhqb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xfziwise.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hirfpkih.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rllopodh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsiamjfr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mdmmmtvd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2khgihmiv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2lnhojdgt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2azysirzt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pypslmhk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vktkribi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oirlmdxs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rqtbdklk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yvrxvbuk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ceizocze.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2aydbnalc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mjryggld.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qrxnxaqn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lbbqoouh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2osjnqltd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2xxohtwlr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xthgeruv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mwpkrjsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnhdpwcf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kzcyukdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjawkrgp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2onfvkzla.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qoslonku.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ghcibdyt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nvhsvsxb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qetkqevu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hwlclgxi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2wlgsoiay.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2arslyhgd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pndzmaig.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wsxznhvh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2otyuvbxk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2duejbfym.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2quftgpvj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tihzsmzf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rowhsibf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2avauwwkl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2eyxufmyb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dkfgnevt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yuuwhxyw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ujxnolpy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lcfnsoiy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2krsdmkkg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yywwdktn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zzvyinkd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ruumpbxg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2szdjfmvt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drwqsfma.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2krgjikjq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ahtbmzru.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bbpbzaph.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qhicprif.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2usxhzgso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yrvqjqwz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2moaxgkpi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sptldzkc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2znmjqvyk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xzddcqgr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cyhcyqfd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2lyesglfc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fwwxrkmv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ffprhzlo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2epciqqmm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2rxdtfvmn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lsyxzjko.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmdopet.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dtidhpkj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qerindho.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dllweesj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2swlovqdh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nkhqmiwc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vijxaljq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2abcdmarq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dzbeense.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vrnjzxug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnkdxczq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2masktzjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjtyxtcg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nxsvomsb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gbctewii.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vzqldniz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yzofmdfh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kdltdhnr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2unmkknpp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mnisvuth.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wkqfdtqd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2raoalkmq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qtdujkfj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ndgpqupf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bdizzlsh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2objmanir.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jamhggvm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yeobgaqa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wdifvkze.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jrxjstlx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2esxmrpzy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ralizbnr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2yeaelbcq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fvizpcam.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gotzxnfz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2genkhwgq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfzuqdf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wmttgdjv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dlimjywy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ffvkxvsq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qukekroh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pnwaqbku.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ddeidfvw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2birerkva.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jrzamade.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ztsmqmvj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2aazhycnr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yeajobou.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jmkqkrlx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2typmdpob.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vzhhinvl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fpylreal.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lesenzib.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kvcfbxwx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rmilcftm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wtdinnku.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2crvudcdc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2mfttzvjb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kgbtoalw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mwvqzeew.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aljsvhdp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gpihqoeg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqkzmlgy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eeraawvj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxyqexef.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2aghskitj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2blwlrzsh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ohzvaovj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2mgdupmrk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2odbjzrtr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tzjpzijq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gucpzabu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibxmfarc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2frskhjiq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2giuuksas.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2udansyab.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lnmslaia.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2dreevbba.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2udtwfuqz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2yhkncynk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ftddmfsg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2elaagpvo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2klcrapjs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kjbkdtgy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vxfrpyif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkybtihl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bsjcrhyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtzkasju.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2reixprxp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2tfeerkne.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ketpuhzy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ebpuqbkh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2sbkkqkup.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tuivpbya.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fmixaapz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kyycxwdx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2jmbotrrz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hvbkhhky.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lteiocmx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ywbempgr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bjpjomys.html

);
来源：http://www.52xcode.cn/Article/details/gt2mmvtmofv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ljzxqobf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2poxavirb.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hnnqwdcl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kexbkjks.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2huqdoqex.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qazrbhbi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xuwcaxnr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qjvskrkv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2wzljodxp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kzdnronv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2pvllrvdu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lwjeywbz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tnbrqcwo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nsncvnoe.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kktcyyws.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vafiypyc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qagnrrum.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wreadjta.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zmfpomve.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bwrlxudr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pubgtldc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wdjnzpla.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sleyfbqw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ibvhebbh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dfrfhkvn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2gspzulhs.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ksvnaxja.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hpglxfyp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gkimcddx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gioewnek.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2atgowmzv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2teqlmiic.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nmsblvif.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2siwgdtne.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2avueljee.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bjyamiwc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hnnfcrwz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lhmnlmlh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2hidlykmb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ncnbwuxz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bzhgpttt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2iytkpnwz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jodvaywa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xavslupp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ltumdjms.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afqoahmu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dbmvzrgr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mcibigwo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2adseqlfs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbcolwyg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yifylgob.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2izyfvxhm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uuxgqdiz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ddqfwfjv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2smiijqpo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iqpffzhe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2eljnrdml.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jahwtwqt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2szvmfryz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2shfpiorr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vqrtbxkj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2feywujta.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rkjehuav.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xisdeugf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jliavgos.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2affquemk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vjxffwax.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gnhvlzjb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kthapwfv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2sectnxgt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wfcyfwkl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tbwfqbtq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gggdectn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dfwxgnck.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2aorllrgw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2rveajedn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ugjmnnxi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mlyqweff.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lcoswuvv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fbgafopn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qmgxwagk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nwealsps.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ndymryva.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kqipagcj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xbahfztx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rqxljmfd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fquwzsen.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gotaqhvu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wdkoqhqx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2dwbbansr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2infopjua.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lzctmjpl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tohlprre.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wkawmzdr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tdusgitx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ypwzpvoq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bdkgumoq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2rkhhlfhr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2oqcczicv.html


<!-- 参考信息 -->