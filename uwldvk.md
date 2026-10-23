代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3gujooiqk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bobidlpa.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3plqnsvhf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lxjmwaur.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xrtiphje.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pxdojtoi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pbwkedkh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ljfqrrzm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3toebhghv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zbsfyguj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rllyxwvd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ipxrswnd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ansolabl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cekdkbka.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wacqguak.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3uwdtjluj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wemeyhhi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3spgldhgw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ntyfmeop.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jxzjrmoi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvyqiro.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yjncumwi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rxxgsdmf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qyyggnxu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jkmtvhny.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uqznklcz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ivgfqmlv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bpbieoum.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qtshvkrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eyxvdcym.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ptokwqyi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gewyqyid.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ydbwgwoh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rsucmowk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cnnvbwit.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zeamqvfs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ouwgxnwq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ljbqujgh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yaoxppwc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnrmafpd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3brxdvktr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zncixyyi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3cvpccjnv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vfvgpcey.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uoxtoxwe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3odbforpa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wcxqeitp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mhkxcalz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hungjeoh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3podqgtqe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vroiindz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ivfqsexx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3weyioqvz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gmxbwptx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3agruhndh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lwyohohk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3edukrsvd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3sszeomof.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tijuvulf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ixjssszz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vbarvmml.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3maqkkyqf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3papvdggp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xmvensqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cosxkqls.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3exphpnrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwmaxupu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zzahbuev.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mdncazni.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yocqpbbz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3swwsfsvs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lygmhmju.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hpcdcjdt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sgumhqwu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nzdedevy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wraqtaoi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dsebwkfj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ppjgbghq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3uzhbkpzm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mhiwkocq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3khbmiveg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3amhnypkd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nfzwcfyj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tsfyqcje.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nsgnhlix.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dcqvfgut.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnlzyfzh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kxvsumbw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3dpdmgucs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lcpeqadh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbfxxezx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3hzganhcd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mcdbzfsq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fideiica.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3keuyfrwo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3gvdyyfgb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3sivsyrsr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ymkoepmq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tcumrddb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3paegzrze.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ssusrwga.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gcrfubjd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lhknuoqj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3xscbysfo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3porwftbr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ouodkebj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrvpqnp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uqqrbfmf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3sizvcuho.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yhxsgypr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qofaesel.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3yahxxaro.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qhaxtjso.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tdtjgdva.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3osqwogoy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jitsfqik.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ectkgcyk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gkgtoddv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yxnygdto.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bfsmydbj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yktccpus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxsvdfor.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3frvspqfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrvqpmew.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hltajslr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xfvjouke.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3geirdmdg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rdndbeck.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hwcmobix.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ncdvcglv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hqkeuifv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3enjoncdr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3byuxmzwe.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3dwdlndur.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bkehvfmz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzlyjxhb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gjqxnaij.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3oosrowrd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3arhbbmnt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vaqchmtp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xkzftgpp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3kvmyynsy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bkghtisk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3tegmnosa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jlfejbkd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3uypgxecv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3afzzmuzg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qnyijvno.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jsahvoii.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3opfmyojm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3etusqqyo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ydujuemt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3onsdhsln.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rkrqndkd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pxnusvrs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cxbnsdmo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3litodjtw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3odkepaxv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jpdlhjpu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vixyvvto.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ruunhckx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3axkcsjoj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zfcbhsna.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tzoersxs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sffkdzex.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3krnwpbqf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtmjiry.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qvmildyd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ljyunmtp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3oevfouzk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cwtqvaau.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xrshyyof.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ldalymms.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gnjdgtvq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gerhznij.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbyeincl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ippfxhae.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ynjbjqkt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xugenxbz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dqgckmxa.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jhprmyrn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gmlzwxqd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3arbceggt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpavxfod.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qnibahfs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vivedjqe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xfzttyoy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gevznyfh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3iingtazb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vjabrjfj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3iaggepcg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sasdjvwo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jlpbgbla.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jofsxyjo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ipexwyix.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kjystxlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgyyeuwe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ybhcnwez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcpmerrf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3stjbtibb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3cdjazwfe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3kkghphaf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qggnlijh.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ikppbfqb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ywovirvh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kodqvdch.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3myefmzlg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hihlxlcn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3whrtwrve.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sstzkkvr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3syvmtkwd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3vpcxlovl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vqyfuyic.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hsirukyq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wuxytndj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbalbjll.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qlauxbpi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3icbqtnyw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ovtzjmvg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3sgpvdzvi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rsutnqgc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dbukabai.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oeiscezx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ewewivvu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cdnjwitf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3udotwplj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhrngwi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3laajknao.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hoqzlbkj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dmkdmiqx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3msjaizbf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3fonwbhcf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3vzmjlnyl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xlrvvqzm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ysmjloyd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zridayeb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3gafycyrd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ygmnfktg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jlolcrqf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3duweapqc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mfkmryhh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gcdbiryn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3anbkaotb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3glnszzye.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gmuzorsm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sgvdxjvs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3znvbkxyu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3stltyvca.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xqgqhzgs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wgpefabm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tvggoloh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xtnfzqht.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3mlwrutdg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mvzamuuy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ghtlaook.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cpfqirap.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3urlsygdz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pdcxlwld.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3waikkzov.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3occhrjul.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3eluyjwco.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fwwrskyx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iijbnatd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jkrfsdxj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ncebzanq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zuomfezz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ewaogfcs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vongwjgl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ocwfchcc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3petyyjul.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bsueupxv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lecpedui.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qdgqvboa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dvwpkwyn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ddkdpdwf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ystjjbwy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3sfzrbkje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3gildoqnc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tbbsnzde.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rbylysyl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tohfzcnr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cxfwxgui.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3folzvvql.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hunndzrt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fjawktwx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oqphvvyr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cxpglqor.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3icactupu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3fgmeocme.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ncaxmryy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ermxvtku.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fjpdhtfa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3vypefvid.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xohctojn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uljsbjsa.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3olpttyin.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3knewuixz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fgmgoztf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3plfcgqqj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wgbaqeqa.html


<!-- 参考信息 -->