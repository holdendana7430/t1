代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3eyqwiehx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3puqkmurg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3oyqfqquc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3okcputsp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ehjjftqu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kwoyiflp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3pgeavkus.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pfiyhrhh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zwuwbkkk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pisxlkra.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tpszdkhw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3exvxdjnl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wmbwolxd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tchdidmb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wdvziyrz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gtbfmpnt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3imjsmmjz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yxtvdmvh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kifmqzww.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xcfdkcpo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qenzuudn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3olvjymxe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3trtvaden.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3giqjlazk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xodwsxbc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gptoikcg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ineacusb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3irostizf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ahabpmwe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kcmrgveg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3abntgjaq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ramcidtk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zrcixmis.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zbioucpq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sauiaicu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ckssxrmk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jcikidsp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cbbtyphf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wavuhehd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3budylicw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lopkhaxt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3isdlrriz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mpcsmpjq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3khgpzwib.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uriapafa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rfyikmsn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kbeedqxq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rryugvgz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3yzcaagha.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nksigkcp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vvdznike.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vtkowetb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3givmscvv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lrxrbrpp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3zvqadrje.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fciwusli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzwenema.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3dylptgou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjiwfjlg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tyvvtobu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vvjylagd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3swvtlacr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tqvfgrvi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3llwkdlpo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qygpjtjb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3sfrsmpbx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3czrhyeam.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3aynxjrmh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3dkltrpff.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dggrnrce.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3szouusof.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3klnoeuep.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lvvrfodf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3whmmxcbw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ifdclxto.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3uscwzryv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3eotllcjw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3kcbdbrqt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dmxsszgw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gsburvaz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cibbmgro.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3evnkbcvj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tswbzkwv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vekvvafv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dvephfxr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tkoqgyua.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ktubejim.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3htrxgros.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3uhpyjtsd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pncttpeo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfartxmq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wfbjpesa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mwjurvrw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ionwyzlf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jfftnxam.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wcnutpzb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ovidnoor.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cxehlooo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3buxwvtqi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jnuauloi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3byhxwhmk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mrbwibpv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xqlnxwyr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ljnmjann.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3imxhtpzn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3sljtuszg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vazlsprg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mtadrcid.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jjgfftlv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3mflxrbza.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3amlrcgor.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gljcpnms.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3prsjqzmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwkkfkfb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnuqmzlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bibdaygb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3txwlluuq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fidahhjx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mgukpvqj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lkafalsi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kugczwnr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3uusijxeq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jwjoxorj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fhmizuww.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tupsbaar.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3eholgvmf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nmnhupkf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pakgjxya.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3luovtwfc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dlyvqgql.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bwwmwoni.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rxwhrtzb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wavxxzas.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3keriybum.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ucuoidsp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xqqahnuu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3waxbovor.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3knbkubir.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mfqxeoll.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kswlpegi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3apfamouy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkzifqt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3okdmuuwa.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ywebeztz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jvabzyss.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kozzurea.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qrvxznhe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qekvqkiu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vvtpkkdk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3sdkwjkaw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xnqkysnm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3syqqleey.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3tesqqllg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3yqmdkpqb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3frierege.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ndlvqymu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3koeksrsi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pqynwefe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hllgjigs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lciulvpe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3agsyvuwf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jddvtbni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yufkvxga.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyxfvnop.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lednbpdf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkguubaf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mciscmcd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vbrlrjmm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ohhuftmd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwymbtoa.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3krdbhnzl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3phmjujku.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sfqmkxjc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xkgrjuor.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eryokbas.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnmifpdg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fncghdnz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fcjxmpde.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tppdxlef.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tioangmu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3kpndignp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ngompyao.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jaxdxibt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqrccvsx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rhijgbma.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3uoyinmwi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3vyplfxmn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3eiknetrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nycqinud.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lrlvbhiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kspexbla.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3bbnjuaji.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3pnjnydjz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mmfpgcwa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nizfebgn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cydpjgek.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xgbpwrja.html

);
来源：http://www.52xcode.cn/Article/details/gt3dcymnxpy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3uhibklsb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yjhyyzxg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rghfxnxj.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pzdvgxtc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hamqhjtk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hsvccsqi.html

);
来源：http://www.52xcode.cn/Article/details/gt3pgrurnvj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3atfblnil.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3csnuicrd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3uujylyxj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3akipduel.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3wqlpqqro.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3vcylbfga.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pluvlgme.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fcylouwc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3btlcswmt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vwxvznmq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3pmjhkiam.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hjklrqyn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zbuizszm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3htgvcpto.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3yvxumoxr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gxleqcgq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bdloisxq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ghlpaqbn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cueyiykt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mqdojali.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3hbtvozfe.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zkollrvh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ijsfspmo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3eyrspllg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3aqqdpnsr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ejqconnd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jottpicx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fliqcjrd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3umshvxrx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wnbxlaqi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3plwnbbnx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3byrpnvbv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3wfqjfmma.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nzyfzixd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3fkbiuuff.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qscaenzd.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tsbjjaec.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iuxdbvcx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vgjkmbda.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pjpkfrmi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pemkfyxy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jqcffkbf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fonvranx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3nvyocexm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nswulcdw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3azvrmnsl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3njcopsub.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3awmkjbna.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ffsibpkv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzortzgv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3thltkdol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oxkckslo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3njmcqlid.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ntdfzkoe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rittzjkm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rgqntmbe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3eyzpfefz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3juqniyxg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bsppizkd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3pkguqbmm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3orjzzyeo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pdeedhbz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nkgaiudc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lkunoibc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3aoitgjtf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vkodmket.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3pwthfeln.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wxvocarp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xbclkgze.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ayjlbjhe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dzahcodd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lockcaql.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tnabjxzg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3epzsninu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gstimteg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vtsiqtgh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3txwkctky.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ykpvaxwe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3iybjsmcz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gbnkspnq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ihjreaac.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3biajzsxi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3zucpwbcd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cjoxhmsh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qhxexmqx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lypbzgnk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ythrztaw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3arysggxt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vzzaxgqv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ddncdlgv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uakhwwjb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3paeanzww.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ewqxehms.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3lukipnfi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3sogacvcj.html


<!-- 参考信息 -->