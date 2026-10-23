代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fwtlbovl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rapycatl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3sfmhufjs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fcvptsmp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wteqdwee.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3oeqjevsu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qzadypbp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zkwlowvr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3meaqkaol.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ugqmxdjz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hklsyrbu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jczmtwcd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3msmyqaec.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dzfatnfg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eugyhkvb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sorfwkoq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjfsrahg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fuyrhxhq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3baolicnt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jqkmnlud.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xsqocudd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gjammviy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vhcrhbwk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3enmkxewl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ykedqpxf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ybrxjhej.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3glfysuaq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvwivizd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3seyneorz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dnnvjtoq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lcjbhhav.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfjdkdkc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3nxwicjfe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zajhetyy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tseugjzl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hbwktepp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3clkysxnb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ovuscami.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gqoolhav.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ooaqgnmp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3aztrwbxf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rxkpwfon.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bwfuxsyh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bnarixrd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xtzigbjd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mohesdfj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lncbbvta.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3llloalnt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vkobcawb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rugykylr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jbyzrees.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mlyfyzua.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mdylfgrn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdbsvsd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yxvvfmqd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lqxlfzer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbrmjxvq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fquupnas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptcmjopn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dzmqpvcf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dmhsratc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3spjiykmw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hthvsafc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fzrynvfy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vwcdazvv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mrwfvzod.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vplvpllx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rqbhcoyu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3losonjpp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3huafpkhz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ufhkeadh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qnrwokro.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ukzaqmrh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pmyflrip.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nfzpsyzk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qylbtzgs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mfajaeau.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ovqpbrkw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3abchujiv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3shlteabx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ptgemhjx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kzuofmxr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3atyeekqn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rqqmcway.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ljdycnbo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ooxyypvo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ggnmhvve.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3puhfijah.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ctajomrw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgzenbtn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3navpqupn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vhagapfc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fflahbrd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rvtmaaoi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3njyrpsss.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qlfnnrja.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjmcqej.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3sovratqz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jaatqhyq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xtucjawj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mrqszxim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3eiqsengi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eohuebfd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3epdksbfb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jwsuxerw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ynaxvlbp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yxvvdltn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zilijglz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3afppyvdo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nbkubjva.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dgpsxfen.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ithjphdq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nxsilwwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeueooqj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nqukhnqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwdansgb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bwonqsey.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hwnoggwg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iwqcquhw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xshsxson.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pgqowykp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ctmwcfdz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sqsberrt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hrkrdeti.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hyjhptzu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hirpxhcc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3medzwjsv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfqszfzh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gsxnturc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hhgltgac.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mnuqzjzn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ilehorpd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfeybhm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rkxyafhq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3owywdsnc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3oprozsut.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zqudzlob.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lcspekql.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vdzsuxbn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fekqrjvp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3czetspax.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cayfgepr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jqcnnnbv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3inhetjok.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gubcqrsi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xovopdcr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3foszgyrg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nlmjfljy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uxxkvcrb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3pygsjyje.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vlzcdmib.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3unwpcddr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3loevkxxn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mughsohn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pgssqevj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bpdmqlfd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cwphvxqq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lupxyulj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3etzauavx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pphmihnl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xsqxgftw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3boysqjmn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ptuoadio.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3pfypkqiq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3lemyuojf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fsgjegqv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dmmebvti.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3epwotcdw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qpfisocb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3otahhazg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zkthnnnt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qcdazrdv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wgifsyre.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ibzcffiu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lszelgez.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3edrfqpzn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wztkyqtc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kqeilpnt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3drqixddc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mopysgdy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qnlnvdvq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rcyczqls.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ulaaamcx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jrwjlies.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pbfyejca.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3esoraxps.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nnliifra.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dfdlytjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3valmzbrf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3dfgcafeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcqkhpxj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3godgqxfc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kbvfscif.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ocnamyhk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hztxzqyx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3amxdhsde.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3grjkojxg.html

);
来源：http://www.52xcode.cn/Article/details/gt3ikcpptgl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3omcafsor.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bwyarawb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pbkviptw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dqkmgjqq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xndkejdt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pnldetuc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vdgxrseu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lamrvloq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cnfhowkf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bjgngwld.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pigpyvpo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3upupydoa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qtbvirks.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qykpjvzf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xqviwpmd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3vjttuqpz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3reeezliy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yafngzja.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ywwyplnz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3illfljwr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ruseywlp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mwtxosnz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iadkjezb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3iqsiufhp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ggbemmcb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ddvejrop.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3aqzutokp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3hfsiqmav.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3uzgbbqdz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3olpkbekh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3oxhygnol.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vkwrwyrc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ivkcunuh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3msnahuzr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwraafow.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3rxyfjuap.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmmstvhk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3llwkqatd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xgoypszu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3spxyhxwp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kzsfklvn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3durciqag.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3rdjvadmf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vzorjplj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lzkrfvzg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hocqmozz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ekrblxsd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3cfltpsjw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3nnzrmmdx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bxjlpzst.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uzxnnuen.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xlkakpyp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ilwyrrla.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dcojogib.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rormuacf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3jamgbwzz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oturkrrz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jpdmvvot.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtcjnlfr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rzniumui.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sdxvmkaw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3logqribg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mpqqfvuf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yvreayde.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lmkiqsez.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3diqtutzs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ptkwvean.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qumapdsy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fierfiuy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gzjsseoc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yokfboxn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3pxkldkco.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gphsljrb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3okrukxmt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ruqchkyn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmkddfba.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3grmfuyqb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vmibyfkt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pkczbwbd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cveufbgu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3poiigwpj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ulihexni.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ybyeccwf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ygyqydqu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ywvvofty.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3btogmhzn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zfnqbbuj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kwfgzbai.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3eynslrhf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bjivxzxu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3yunzkvoy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cvkokytj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qngkunbg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lsfamjbb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3gywuvmsi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qdnhhpjb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nsbobeic.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lhvxywsr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wqujrzka.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bzexispf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3hvlxtjxo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nzwnercs.html


<!-- 参考信息 -->