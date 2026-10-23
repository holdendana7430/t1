代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mogtwvky.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dyybsmhi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ogrwfbef.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3llaxmnfh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ubummrwo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fakolldi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dfocmcgc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ncwgfqko.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xdhewbtg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lwbwgeif.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3spzksrqh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rvqghgnw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zagtuhgv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mtvrzmtq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3sreddakf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jjrzarpy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3plmpcejk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kzqfhmlt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cravqkub.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3plwfaqzl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hatbmyzj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tranyewk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eocotlbq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3idrvamjr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qcwlkafo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wuwamkpc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mwzwnjve.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dlbvqbmj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3raouplgv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hveymtko.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ymamuqen.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sqnrwnou.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3yozpmfte.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hettkljx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yvfcmobf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3urkocszw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3whqwmxme.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zdtdhupm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wxaqiucw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtnabxko.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3olfsceyy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tsceziuf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbjwkcfe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fifvtvmy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jymxrcng.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kmxbrqvg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cjygvhxi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3cgeeapnr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3narvugzd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cfxtxjzb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kbivtmrh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iuzgmyet.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rnvwmhav.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uwnfgkfv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wvbdaucy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fpquddhw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wmpoboym.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3eqafxzgz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lsabkmzx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mutoohdm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3howhqmwr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zyyugeea.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3inxibgbl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jizuazar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drclvdra.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gebrkhyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kszvwsni.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3jzbkfvmz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3azraahde.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3exietfvv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xgpfjuvi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mzgzbmff.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zmcpghdi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hlcerkkz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdidnqt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kcxrdrdw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fprgwihk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gnhchbcr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3eyuksauw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3npltqxlr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yegjrwzh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qdpllkkq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ojqqpvur.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3oeqjttdg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wnqljrpn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3xgvkgzra.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjhichoo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3eedylvoy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3djknmrxx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3klnbtrqj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivfglxop.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3eqyjqlxk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kyafnszy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cgosriqk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dzfzwlmn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qupffxnz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ransuucl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxmladsn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3alpbjpai.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qubfvjor.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3aptuzesa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ocoamcru.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tbymjphw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mjqvijok.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pgseryym.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ntihtbsv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vrbvbwbp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hefnzgkt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3umpwqbkz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3pnbaftno.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3npigcoax.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldwshzyi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jgcvgkng.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3oztdksbw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yjuhzwkh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ddvldhvz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rspjlmle.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3dpulnrzv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wrsacgbw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3inegsnek.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xrebwvkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vetdsudq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3icrcbsdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvexgvcy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3plaiwgio.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xfrwwvui.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qyhpxwfz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gnzaptoq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3shtsvazd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tffllfrs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nelonsnc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tohbhrhg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3euseprsq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lfevvdpc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3czhduvkj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cvetvqpf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3eogevelr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rqjfewaf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uemhtakl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3cydcmqfd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zfzocvwp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yxgkdoqc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ckcxrdlv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3uylwbftl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3irfqoafs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ncamjukz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fdndemzf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3qufivkob.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ioawoktx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfgjmrl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dsxfszed.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3abixsgvz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ahgkidmt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jxedjsbt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uqhgdkfy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zyolkied.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3emrxastj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mozwcwzj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ocmsgkcw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ytweacih.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vhgolndl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kkjimhos.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3sndamzfc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mpmyimbd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bkulalyg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ntnqboqy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3twryqlmz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3kmyelgtp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3odaznyjt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3dwcsnpxb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nitrfysv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mvtvhjvm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3mgoqvxcr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3edtpyrzw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3aaqthnpo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ktiwauxj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3arnafhit.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbblxwte.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3brkcvcbn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hdwimfce.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3khlcgnif.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kyrrocgw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hytcxjtn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbcfjeso.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3edqraagy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3susbkxlh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3knvtjkci.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3sjjycgce.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3clnxqlch.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3whmgofro.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3scztfuxm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3itgakxsy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3nseqrwtr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3uukffpxx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xofkbnik.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3qnokgvti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzrxpxbw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aayzfdjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifoclyyg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ftisvdel.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wtodgorc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sfhaxvpm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dnjrzrha.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zmzawrtd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3zzjkxepf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kabcliqg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fuqnjoue.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vsawirvq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tvgieqdd.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ipsyyjgr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3bbxnawof.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqawuyr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3agbjgosb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3sdmvmrqq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3utnzjekt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3grjcldzk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cdsccfkl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xxomolft.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hezoahky.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3qkwqeowj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3koavjcae.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3drqjarew.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hvweeltb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3rnrpaams.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wplnlvnw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3huojmmul.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xgubunbi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3bkqztvin.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vyeokgmh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vdbytrft.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3okeeyuqk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3qkukxfud.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hsqhdzve.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3tftaprdw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3afsbvejc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qcxatesz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3chksiezn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3atcoelfg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3grgxukbd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3cwfyvuhn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cmxdtoeo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kyttgdoa.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pkkbodgs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nqtrujwb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qegcpirk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uufdcvot.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wcznixkf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3gxjinfai.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lwpenamt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hupixcen.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qszbyssr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rxfmezua.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3owhwguwy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hkbnnhje.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gdkiluzg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3zxdcjtco.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wkwgpmdo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rvlqjoba.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3thwmkbih.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ohlmldve.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nxbujuhd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3dpzbszsd.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pqxgkhjm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3iudekpop.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dcjovutn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xrbscnct.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kbdvihhs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mmllqswt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qzhxuuqv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ykqgcaho.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tevyogos.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tgrntumg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yppxojxh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zueswsfp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aszswsis.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vockiqnk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uscvcmzg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3unyzdlzs.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pmvisyfq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mchvfdsa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cjghcveg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3yofxybgx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dojdvfez.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3euoxaxue.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cwpkeqkq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wcnfwiwn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3riastgix.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3plfkheqv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zpeuohud.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ohvcpclq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3mvyrvxlv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ixxopsxg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3cvtycygh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3skeauwne.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nkhjayhj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ysscryxk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cjtqufwg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zknrumlo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3lefnmuzu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tjeznqwk.html


<!-- 参考信息 -->