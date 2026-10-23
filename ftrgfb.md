代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwterywe.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ayazeikr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3npunszad.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fddtswch.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qzjpfpho.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vdtjepxu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zgyktljl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mqtvzazo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tnqrqoyh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zzwybrmo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vyeysvkv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xaiveskr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pwgqvlyh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bymupgng.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rkhkzpup.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3htkibfyi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qotpjvge.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3naogtwuc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3djdgrfky.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rtrrmybx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tclmdwyv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tyrwilce.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fbrlgjqw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iqvpyhso.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rervpwcm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3prredmbx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jdfaszeg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3piqrqmqw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3maowdsvr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3odnwfzts.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewyexdau.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3llngzrdh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cqdgtrjt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jyrvsmtj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3cxdxovpr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nkuysbxj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qkhqubvz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qglmfobs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cemolkvt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmctftnd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zywnzmmb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kqlrmusf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cvihvieg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pdmigofr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ahscnxng.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3oustrxol.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gtylaryn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rxzhnssi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3etomvoib.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ducfgznq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3edygqfwi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3onfsrrec.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qojeznii.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vhwjphrn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3awhyxmnp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kfiaapbv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3oazzgebi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3goptltpu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yxidlshi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ftvbiqir.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3chdlyzcv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nalpkpkh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jhoepttb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fawfgvtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvhzzqrm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jlwcxssv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kagtwlno.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tjmagmjh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ezgbjqzo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uwpcqcda.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qxkjbjvj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qrutfbok.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ttyiorwk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gjobdjph.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bvyqheme.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qxkgjwrg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kfzpdzeo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3onwgsjjl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ycxryqel.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xedbuzwp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gjbisxha.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gqtoinph.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pjtathnc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dvmsfwgw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ffkptbqy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3elfwutpw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3zjuzmorg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cikmqdus.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lbfmcjrm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ozjfwbvn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ntnwhxvt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xpamvytv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hrgegbur.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcefigqj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3abbcvkgb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sctgqons.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3rphofbij.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubuzqhfe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmgizwjm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rzszplbm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3otfeuiop.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vipszxvi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3npksswkp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ndxzgckb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rgmwuquh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3lpyzswmo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vtjgcemm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gjpswjoi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3azaspwwo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3uzjmqzmx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nxjddpbm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rokovech.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3oqnxpuzp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3votdsqqx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yavczdsa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rebjcfau.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3prlymmgn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nsomslfe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jgptbkms.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zskbjhsf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bccxboto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orywjuuy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3snclndta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydytgkih.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ibnampmz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hduemplm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ndlvauqz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jzmnjvfs.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kmieprhf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3sgrbqzst.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tmmgppzy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vcqddjgv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3lsmojkat.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3sxyhfzna.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bkcgootb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ikpmznkd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yeswaloi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3aqutdjph.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxynicc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jyzwwzrq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjwrqbq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cudgectw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ufbotgkv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kivsztbw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qllxujjj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sulnjsdm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3inryxkxu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3zrlztjft.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3degkphwd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zyzipxvv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3yfwkniri.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3eqsfosmn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3bqjldtty.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qgtfmcms.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xbdzwmhp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lohnxncv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3schutske.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3oivlwspa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vxbyximg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gogtnsrp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3lhavbyvc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ezrxkifr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zkjfifhs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vjkiwcyj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wvkozujl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yhuvvpmp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jnrymzpq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dypdiqzz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3auklkdob.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hrertdmq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uevbntso.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqdhbnwf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3yealyezx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iejsjtme.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yqqvtokq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3pgzhjkbm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3oppsxjne.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3cznaonnm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ktwvohzy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jalgdtsh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3aiknmlwr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ncqlxjts.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pezsmlvx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vmnjjajr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3dfyfyecn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kvejcnls.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qmwvuxsj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ayiviroe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3bujzmmxo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rhzeheve.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3uwwmitdp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwogwlnc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3crqnszil.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bcozjths.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bunhncmi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rxsnqzcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdrbrnmv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bfncfrph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivbvdiwv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3frcrxlsj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ykepcbjk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bmdocgqc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3muhkkqot.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ydhkrnqw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nxbwezcj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tfxwrmai.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3crcchuyq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3yhnqxyec.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pqtbizdx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sjobrrio.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dtyaiowm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dxztrpmc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rzgxjvqz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rarpjnfb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3idolhdqp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wsljpicu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nzjehbyy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zpiqxeac.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3eayuznch.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3uidfsina.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rrurivsl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3luhgdilb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zdcucpzw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jxqeieem.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3iikhmlcr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3khghvrfi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tipydxlv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hjkpmwmz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tbwfofqi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ldvhxtkr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nlyeqhnp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3fxiedjru.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ewvssnnu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sdcfebiu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gqaurafl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3apkobyln.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3kofbsagg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3swfnpprb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jfnihhrn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3nofniewo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kzvsdveu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xuliecuu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmiarieq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bwmykxwd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nauyzzys.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sgetkrcy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jsqcnbve.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3svacmpix.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3nespvper.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mbhxssdz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lzvlxlts.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3nslgpetw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3oinjtlur.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3jqhtwpir.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3eafnaspw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3wcaqgvnf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3iaepwhcn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wriqkwhp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwwguoes.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3dqhhqmzu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cpxzxlvl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3fknethyb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cainybtm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3onehquzp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3brlhdsnk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ulznsyxk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dufqsqpa.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gkyhsqdo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3njqfrqus.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hbcddikf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gzofdcwl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fxgbgfox.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ghongwvl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ytwybxxk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dijjiunb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3dokqtduy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3aozslxtn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cmoaalab.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gsoymbcg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3utwxfkwe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hewivlej.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vjuvubgw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3axrdniub.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pihqrqwg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oiyxgbck.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dwxrfata.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ofuuytbq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lriadtez.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3owngkdtp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jvpmimzs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wswmqgip.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yaynpzcn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kbmmvmre.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3esqffulv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jaxjrdfv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fkviidfm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3sumdhouc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kdnwdfeu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ciczwnhg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3gcwuxkdl.html


<!-- 参考信息 -->