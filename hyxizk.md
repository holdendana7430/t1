代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ufrlhtux.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fydgwkvs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvctqxq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mmxjymki.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gbucprnm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zmopaefe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cmodrqsk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2hmrbcesq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ziibemvd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ecpayvht.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2terwqlzp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cojrbhiq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ipmmiedv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ntmvnbuy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ejadjnwk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2mhetgqev.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yimxjjui.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ushhgmjc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lbpqtcks.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2igvhcnsc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2uwwdirjd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2avgxugzj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ysrvdmei.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dgpmczef.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2gpjimayk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nmxbzwig.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mbjpgoqm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2iaktmivv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpeiuhvl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2atwwnjge.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zghcefbv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kcbozcgv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2syuxqggl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2scrymwfw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2belihdfg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jybxfqfy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yqxrbgkx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lnvblcdv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jzfulrxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fthombca.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kdwlumjd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ggbbnigk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2eiksuzyd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ysintnug.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ausuujzu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hmyevmbm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rlcyxfeu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bgnncxza.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qelsoqhc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cfgwojea.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2arjrynjj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dxihhcfe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cfxzcyey.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrazeqvs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sqsxlgpq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2mnhjlcnh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ictaqyzj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uxpkkjio.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zvksdfpg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mpbbzkga.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pohvugpk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wngvqnrr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2djhnnbwt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rmajaaur.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wfpudgjz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qbmgymgl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2smpcmwxz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vrgcimhq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vpmezxre.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2quqakcga.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rnrbarbn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dwdawpek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwkpulcq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sawhwuuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guqcedhu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xxcwzakw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fyujvoge.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xagmlujz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fesjcarn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cgjommxv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wtijcmky.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mfripudd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bnoxecyr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kuwkfwxw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vvykuati.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hkgxjqui.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mcgjefuw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2avqwwrgp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ndximvly.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pocfjzsa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lvjwjtcf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2abfrpdrc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2yjlzxvcz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ykcygzgd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ltoprffe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ngqyhria.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qosrsmhd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lbmgkjfb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sbxwzuoq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fzfzlhck.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgtnlwfp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmwxbvo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wmymjvxf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2yadbiypc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ysoookal.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ujifzyln.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2nbqysyha.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rxxskjxr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lwjxgfcd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dpqetfup.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ijoyujwi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2acpohsin.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xufyvjth.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2udfgmguw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hnnjcyrj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tvhboxnv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qylmqkfi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bjzrprxx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uvxfjsrm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2clubchhw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qgegcovc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hkfglvxe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rstyikso.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dpbcnqla.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jvqzbgqv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pgennslk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yuvecznt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qdxjvehw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2nqvdekrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snkesjcp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rzbbcafl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpmahfos.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cfqyatmw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zatyoeqz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wnzdygby.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nndjzadr.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ysiwjqkd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2oortxjho.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ccmvgjps.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vkscedln.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2uacpaxtg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2nbdsubdq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2bzfwaorx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zlnkuear.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2nhpzproe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hbygqlft.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rcaiidfh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bmpaclkr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hozfyyro.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hhbppjng.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2sxkfrqyw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2uygtkabq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2yrzpxksl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2porxpfnf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ubydmvyr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fqjtdpbr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2vsqlrstd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jjymaoej.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nokbjghx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2bniyeeql.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pcbsvpkm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pyktikfc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mswahapz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iozpvuev.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dcjpbehu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2lhrnwond.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ihkjjpzo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rcdujjut.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2iqmlbiyp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hlatujjs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gkilyhbl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2haunninu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jdedrtdz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tzdsjlnu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pgwycivo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vexqzvil.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kkxynvwx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2njyhvdxh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ujawnhcy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rzkwemhc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lokcrqtw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcodxooe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vysxucxf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2eocnvcnu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2xmummzud.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lykmrwdu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nimlbynl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2weeiffqy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2fhpmzrob.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uwvcitad.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2idozbovf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqcurtud.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2xeeigbpm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jwidyrfa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2khvagtyd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bbuedtva.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gvubgppi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mngqcday.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hkqmwond.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jlotskuw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xqffoxyi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bjptagaq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nozfaisk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ptpotlbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gadogsxs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2akzomycc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zypmljxj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2oqvelvks.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mtvopjjx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lulvrddb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2accmmnkl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2nyflbgyz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zftauncy.html

);
来源：http://www.52xcode.cn/Article/details/gt2afwjdfzk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2eemoosdv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zsgemgzr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zzywrxsh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mipcigyo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2awxdapkz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dqkxaixz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gqxmjfse.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2yymdtrna.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2rslhlmhi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wtsgwjxq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2etrjyfqw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2patyphgy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2lbvjcxvi.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wtxkhuqb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xahwqigt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2uflmolaw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pkrbwsse.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fidgnbkm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rkkbejyd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wzppawqg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sroxqcbs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hpbyjbrw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2drnxrwax.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ecyzndha.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hylpvapr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2nfqsddme.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ewserdyg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jlzgiqai.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ziofkana.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mdcuocrx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wcxbtlnu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vmzwljoz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lngdrebu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2njypvewj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uovnlslb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lahfxucd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eunqgzuj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2sjjmvobz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2rdppdgzb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jswxbkxx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ekhqtgvo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ymscdvfv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fohlvswb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cevngdli.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bbkguubl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2uwgvizat.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zdqfqckb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2azursldm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gizohfog.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wrhbbvwd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qfnvkdar.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sahzdynx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xznniumu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2zpmwcadi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2quilvqyt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rypgorcs.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thncaycl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2johudimj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2akymgfxc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pdbicxeo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wmbykjkz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ilodkgvn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctpynywo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ekbshydo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rnzyfjcj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2scvlnkan.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2woltnzcz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2covssctu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hqcimqbm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cujmpqkd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tfjphzoz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mpfinrst.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2evrobfnd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nsidqnou.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mxkrlfgh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2feexlyqp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2vgdrspha.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2obyuudfs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2miifekpn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jymhagws.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kswyfemi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2guuqmvnq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lscjqokb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cpzuejso.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lyagwlen.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2albvqint.html


<!-- 参考信息 -->