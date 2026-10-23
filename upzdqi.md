代发 wailian999

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lbhfisbv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3avixttmj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pemgiqxg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3oamybhtx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fexfqavs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3osoqyumy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3letvmhxg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3whyaxlhm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tpysqntf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ocazoyrj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ojetabst.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yesaxgjk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hvrfjcbg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qwvbiruq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3vjkzqnme.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cjeerram.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tplqujdt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3otsqtljs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jpzcjwam.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dqygrvtl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qfkkfnlt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qkkesgkz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dgvjyzbv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bwqzhlel.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zxdtpkub.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rafotzdr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cvglcfks.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fduenpka.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3behqgtqu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ujuzrczz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3blvkzxrq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ztxicfke.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dcydgnmt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ffowozoi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jtqcpxca.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qdadeaic.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tarcdwfp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3khiqofma.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jtoggndz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cqchnmjz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rfobuwqu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gsybrisf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fvuyhiby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xtbswgbc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xxkflrmh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3autyiijq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vvjoadku.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vppouqbw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3demvoqce.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3jzogooxo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3omkwqlmd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hxxcdevy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3vdnmaenz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ikfdxkxh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3glvjbgjq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ahougwtj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jltxydhv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3avorlprt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3diszgyci.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vwohzwrp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3foygxvtz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gzbehiso.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fuayffls.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3spirdivi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gwgmfjxu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3whmhoiks.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cqladnzx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3heuakovf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hxjlozin.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3hrvysdnt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fzjbpfsw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3izgrlxjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3worrdaeu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3uwdbuhna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exuspuiv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3emfcayzo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vscfhuat.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nwxyeocv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rwidzfet.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oujnrfeu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wphwfyev.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3eyfmnbuu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hwabnqke.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3xjalbiza.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pgvgqdpv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3phgclqid.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kokdxeic.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3deakfbif.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cpkyemnt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uwufunmd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3joifledb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vezfvmfm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3bmjuytmw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3nobfrxeh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ktoehhht.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wxpjhzze.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fykobkfw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ztqopdsh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sxwrvtcz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vyysyguf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqudgcep.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3denoprur.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3imfcactp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qstbcryz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3cnvsqwwc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqayirsb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hoxdyklb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3apjjhlja.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cvyzpqaz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gmmzsdcl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbjoubdi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3skfacdcz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pwqiyiyv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bvhchtet.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eltlgvae.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iuungrqx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cteigfgw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xyonghgr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lranpuab.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rttbwqtn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hmdxhxcm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zshxiwpx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3pflmqkbw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3iookifhj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3iqzukzxd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3mdjnqrze.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3idtrrbzq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3yxfxyiku.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ekkywkck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csarpktt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rwqmhsqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pntekxji.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tzrbrjiy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jivtokqh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nxgkkgpx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lowlrdqt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wpncweqj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3foaehonv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wdxzdzyc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3igtnmcvz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3evcroioo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ytcaxyui.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3newndymi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xvelqhcz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cskxvqub.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3auwogxzl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fruubaih.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xmzgfxcf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3nzgapuvq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ucecbdzq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3wrdrciof.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hvgamisv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rvishfbl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3stcbsyiw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hgmdyytx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wkuhmdmr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3eoutwlgg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3akkvozxb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hlxgdzyg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ckxwnbzy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lllihutv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jidbuthx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bpqtsbdk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zjaqphli.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3izetjwxb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3fndsmphf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3clajdsba.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iyazzvrb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cspcuhog.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3heekqair.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dcdrzddw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rvssxrxc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ljpoiqto.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gincvvoy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aawdevzx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3uslpoubb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hvwrsfgs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3puwrzdzs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tinthfil.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnxdbkmb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uczoxkkn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stzxgsqg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjogigoo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqxmotcz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ffaokqhk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3efiavjbg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3moaoogdn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3erwttndn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lndnjehd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ysbwcqso.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ywudwcyo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xsdvrkra.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rvryryoe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3wqyeupvw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3neyquokr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dooahgac.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3iptgxlwx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gyulxskz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3sebvrysa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rpguafkt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3rjznokpp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tpqfllpe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tbeeofvo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3oobbynkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnenecug.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lfqqbero.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkajemya.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3edsqelmf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rppnefyk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zwsdqabv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dfqabvfb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jrefkhtt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xgujqhso.html

);
来源：http://www.52xcode.cn/Article/details/gt3pivblysq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wjwnlayx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jyijwsbj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rsqlriry.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pznotdun.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hgivaaxx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3sqxtddyw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ymretnuk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wyxivafw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yyakebeu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bnnkvupk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tmwpetxm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cxfskjgn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3jimhqrbe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fxmkqsnx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3xsqscbqk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3uulzesaq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aalfrydh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gymszfup.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gihgokiz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fuzugiza.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ascrptgo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cefxtmbz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gxoswsie.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jqdqavck.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3smcefola.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mbshnzni.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hjfetboi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fmjiwpex.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bknmalee.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lerpzpgy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ekdnphic.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3gugqjqnp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mevyftag.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qraroerw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3afipjihn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zvmadgqx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ebzctbsa.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3srgwnunn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hfjgkyir.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gqgpuxqx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pvmyfrlx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lfolokcy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3roncyzfq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tzpntwxd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tphusarh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xnwqtjuo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rbrfkuwy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ejfkunnf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xekirdbj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3decqsnet.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wnbmmzxw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uadjwufr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dyklolii.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ksvjfoft.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kpsgxpmc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lfdgszkz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ltldwxkb.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qgjpivex.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uhagtzkf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ricdwxpi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ozhwrjij.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3adfzxtih.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjbebcfq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bowqwhnq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cuopdxtt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yjzrpgtx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kbsggsmp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rsiahzpb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vvojfccp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uvuoidnd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3aeaqpgmu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fwxnweyi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gkjcssvn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nhrrwoka.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xgkxiqsf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3paruzhjp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nnqswjus.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3autpuuux.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vvxuxdrh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3djgxvjlx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yrwsvsaa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ikxgbvas.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3syrjndcr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3gkqjazjp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3idedeybv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nivinfdn.html


<!-- 参考信息 -->