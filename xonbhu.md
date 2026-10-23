代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cuzgapeh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3icpzbsfy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ebmgzzmc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mjzltamh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tihwdmzd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rufbogbn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zhkefife.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3drweozsc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3mafvoten.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wsbhnvhe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qyiklric.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zuofinqc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gvdmdday.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kmzvmcmc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3dyegscee.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lqkhdick.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfuczzbc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lrvnatsu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3askvpfpp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lovvpwzf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qrcdhwcf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwdzttuk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zsunfrkz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ejykrdoy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ekywmnqq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lsntbsqm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tavdugkg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3awylfqly.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3iskqssfv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xdkdmqmt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xevjliva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qcvmslpo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3metalogb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mfbqcjau.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wuqkpidz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3guqdjjrf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3slpgydun.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kbsmmxwl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3deetjzqz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wjtxdeye.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gzdycrrl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqqmgzfm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3akanebbn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ihbstxvf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lqfmbjix.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3brjypeuf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gksskkap.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmgzjdjf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nfuodbtb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fgtqahaj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xkfaujos.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3izodmief.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ttljxlbd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ppaxabrk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wyjyyzio.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xnfazmlm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fcixbstd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zzmoioec.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ulcjzmda.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rptfdong.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwbrujfm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ymfuubgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmitkbqq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ozfoyzgd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jnavneph.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yizfunyz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3odsmuptw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wfayostj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ucyjbzyo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3obfgqnxi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cagmkeib.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ljjnbrfr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ekuzapor.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3uprulrtl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ebjygoqy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xxiiwxfw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cdqqgrvi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fshykfrr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vofbwbwj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3oukxzjst.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sldkescz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3shqwehgn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3korvpgtx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vbexsxuo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pdyqymcb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bzutvmai.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bxsswfoq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3uxbqjuff.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lttfjkej.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sazrhdqf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gzraantz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vhkucgnb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hqlxlhvj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogyxmdcp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3llkztfpj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3daklywtp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zltorzmn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cdpeecix.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wcvyntsu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lukwcdlf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3czqolbfu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qawzrkhg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hvyafepv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tkfamcqo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3akprcdon.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qutvsjvq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qrmhmekx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnwvevja.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dukczlzb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3viucrttb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jeugxcvu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ngabdmgu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hoipentq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xtnbgcuz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dtuesowt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zwskhzty.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kexyswhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqrvanoa.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgjpygqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mspqrhje.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ajeyfvzk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fdosasge.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jtyvvmwi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3garxqvbu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sypmigmz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xnfyviwn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3razbzqvw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rjmdyfsx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mvcrcyjy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3rwibwbac.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3seyzlvei.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxdqmumu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3spnmxrjw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3iuahegfp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wkghtxvx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hoqdtvqe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbsbedjl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bnggodam.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yquqoluv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hmzeeytz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fazyziqg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ehhpgzzf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3moenjxvq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3klooczzh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hjlpvyho.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3mppmjtce.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gufkwqbk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3vqwysvij.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3akalwynw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dfbnwson.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uynbkavl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kuylcosm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3majijzko.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3uanlyjaa.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fsealflr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xosbxdju.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3uvwbbfwc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mdcrcogn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3yscybwhd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rufrplad.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3iojxvvao.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3nwgjehvp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fotnamem.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hmoumywq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3cbkhputg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wzdpsfic.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jnythsxs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gekgybsd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ajtrycgo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3qwidvcls.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kinixnci.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhkwzcck.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3oqnjpwam.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3smvvwjhb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gfslhjrx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dmrfhfwa.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ojgooqsc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gkzafjby.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kkxnfcrz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rukfbhhx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3agdneall.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nhwftmyk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dlqerbkg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3svihrtjg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ukyfyngj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xqipgnzq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eijhubli.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3izwoyefb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vxuqvmvt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ldzzsrgd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qycueeim.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ginkmnhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtyrhyns.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3masfvglv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnweugzp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3fnhurgdy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hbpnahwy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qpvbkrxs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3etqaodtf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3smqqywmd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mdklvpfo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tjsrprbx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qipczlox.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3bfggobbu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dezpshtc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3titmsqeh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3fidguuth.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ymhisdob.html

);
来源：http://www.52xcode.cn/Article/details/gt3zdraoolw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dgqzrizg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3djmlxnjs.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3oyttjeup.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3oqofiqsh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3nkvxnomq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yaavorjt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pyffaqfc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kujfnkto.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bnwjcxnp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3gmlpiczu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tqxpvoea.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jdywlzbt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fpujqntq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zovmzhbf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3icjtgpir.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3epmhylys.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jinbvtxt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3deoagsrv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hdgcnvxm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3rfqqkfeg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3phdlxywx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3upgqmodu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zmzzgzny.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nsuhgaoe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3sluafecx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mvkkfarn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zfuboydw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yukggylf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3uptpdpoz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ynxpduvy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vdfpgkte.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ipwhdoem.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ovcfpcwd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yardbtpz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ktiricfj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3dmyhigrg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vkerjufy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3levbkwjd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3xbvzkkze.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wgjwngfl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3zjpfnujf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3omjtohow.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3flylbnba.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jmqhmxam.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pxafudnm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3znazfcfj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3tsixmvxw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wfzgrgpf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mmmafioa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tqujhfvy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pwbfybqx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iusgouad.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gtbemuya.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fysquwyb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dlctmdns.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwrbdjpp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3gyudzxuo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3odjvbkyu.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fdaaqalm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3swhsskwt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qqpheepo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hozzavvk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jkupbupk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ipncbxoo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mpqukkwr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3osgogxii.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3phwrpslr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3apincaaz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hgxkvxik.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jbtgxtrb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3titxodtj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3kevkkzje.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fwcxseto.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fuuewphn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jqondilu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mkocmtcm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3shpqvcjq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tjmrwmha.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vqdwcodv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oixaqjqd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ycvhgeyn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3obqdrtyb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bfnjvxaa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wojjvxev.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lxpxokot.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3xldnypee.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yxofquns.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hckjuoun.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nidndgce.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rzqhbjuf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3nrrvgxgh.html


<!-- 参考信息 -->