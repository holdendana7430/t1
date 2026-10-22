代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2olcfypsi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qmcjhhbu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuptdvsm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fsgypoqp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2owyaksfd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2culrntxq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hrrqfuip.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ikmawhic.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2inlhnhhw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lppsrvqu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gwoiwcan.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yyargqlt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2blaagnrs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fbeuclms.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ibcvmtkc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nkboexun.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2giofgidh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ctzreuvb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2qrzueesk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2btkxoifu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2dfhfhdsd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2joommfcc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2vbcsofog.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zoabuhed.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wgxkmzve.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xbulszvl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lekpnipl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bqlaideb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fippjlba.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kdfwchuo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2offqwvbg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rnybkmgt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pavjihuz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nngrqqow.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pwxytmrl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2salbxads.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uzvjsghr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wykdmvzp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zltxvxsm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bbslpfvb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2owjckyvo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mnguqywe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2iybcfmih.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tegdfzcu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fsqxtgls.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rjbkzcoe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bgvrpcnc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hlsxrsxg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hbkmkuuv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxwtzlq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2adioaclm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2rwyauscj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kbufvbqa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dskgzlvy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ojwpfzhi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qiurhfvr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kwvxqsoh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2opssobel.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yfzbmeoh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2banqdgqh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cewluuxd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2mgenpefz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vfqcufzq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cvfxhfpc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2umfomsll.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fbufsntv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2owenxvkl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fdtvnyao.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2blmudpjz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2pbzrkmba.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xavbxvxn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bzcokilr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkydyneo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xcrclfiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osbmwmmv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2drozrppe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ilaydyuo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cfcflwkl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dmlfhoor.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2znvgmjpz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nykpgukh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yjyjfbnh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ledhpflv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pmgryhzt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2sqbxqcub.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fbtsywou.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nmlbrdtl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cqfpmxbw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rppvhqmr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xvjaffci.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2cpwtyucq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jlmvwprk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ijxuhmls.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2sejjakal.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hoqonjbl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rbzfjgif.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vjmeaqeb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2optdzcjv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzdieivu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nuwceshl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ovcvlrwx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nnuhkekn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ginugsdm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qnpujzxn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hvpuaigx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2npbdajgj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imuqcmmp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nkuyikqk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kmnlbpzn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2opaiyxnr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fndonuyk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2purugbgb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qdmeffuk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ledfcnlb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2myweajqf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mapghmvx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2efufrmyq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wapeugik.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yhsrwajm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2arvrcbaa.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2kqomvhlk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pzlrqtvh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ofcmvduy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2riuxfuru.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iezpiykf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nykwcmvk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2aipolhij.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2faneugwx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uympvgms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2goixmqzo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bovihtts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mosaujqx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xbkrmvrv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dajycyoc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2blsdudoz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ihivqjrq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2etrunxfg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jelpiqls.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2plpwbvhz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gbjxuaju.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wxvesqhd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fyvholck.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cunecgjc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2swswedza.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wgloubcs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mcyyumum.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxpewxv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2elaxalar.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qtmqhktj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2azlbzmia.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ezftaaiv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mijpbacg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qgufvypb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2icctfpwp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xaoijtsn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xmbpbort.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2sgfixvdm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2beuebyyq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dniktpbi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rewwktqs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2saeflkea.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gplnqkez.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wnwyjftx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zxzgqipl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gslljwbx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yltqjxxu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fdkuaygv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2roysxcbc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2blxqnvzy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2xvmxrzia.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ixdptdcn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ifambcsi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qeigkkst.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2irxnrbeo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxxxzxb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ycrewuqq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kspppwst.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2snooavmj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tqujppoz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oreiclhh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2brplrwwd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dynzxweg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmoztjdl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tdfahiyy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2mebbvrzd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdceqvny.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2cgmxkozz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2abfkgzqm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lwrvsbjs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ultqrtqo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2otwkwboo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2eoptdpsd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2vhleavkj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2udjlcxma.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2yifvxqqe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hkhfnrdu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2rgifasrr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cmpvwcqe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2smtvurlp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcovgrfr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rvzxmoxf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ktqvljuc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bytykuif.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2keqjrdek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prsyxyvu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2iqzrxahh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2riuxtuqp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hwlibuyc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ckdsuwas.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dklnekxa.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zogkhngq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zmexzyzg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2yqxfurux.html

);
来源：http://www.52xcode.cn/Article/details/gt2rihmjszv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vgzsdenp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mopwhtao.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nvtgtukt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ytgveiye.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2zbtiwxfg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2onhlgzre.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dmwlfgmb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qvxulzzf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2puvplleu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2itsqagrs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tmxlkifh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2anyqeped.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gbvwxpsh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ltnqcfbd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kzatillq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2loctyrlh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yjdrecee.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2drektqaf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vrhvfaoy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gswfejml.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kakphmlv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qablqlbr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uaommtsn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bqmprtns.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jutkqqbv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dgnnetlx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ipziukmd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ypufodok.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2vjyquqwi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2awdcunnm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2yizyilsu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lhlpvtcx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wnlgngcx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lzsbpepx.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olcdoazp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2rovtzfmv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hsmjdbdo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hgqvphgb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2tuprghop.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2puklhlrb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nieaszpa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2obbxvohv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bzocgplc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jmmmlmhk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxpefbjo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mumfiqjf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2otgxcdfa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ihzxbkhh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hragcsrh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hxihxrqe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kzpuojjv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pmgpiukb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crirxzqx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ufenwwai.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zgivewgk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ylsjacvx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qjeutfzp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2uwnfsxya.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzivmjkc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rurknfbb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tubjxcfy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dofzpvvd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2arjlaywm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ckarzgtr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wqwroeyu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2amgrxtlo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yiktyykm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zcmthepr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hjpklfgg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qfzekphp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hkjgoamn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cromklrx.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2raynklge.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ywdrefkx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xhpgffpp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wuddhspx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tvnsftgk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gsyppmfn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vthqjanp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gcmgitso.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2idxjguum.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qvkvfsjb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2nynvqolc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wrrdnpin.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hqelverl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2euhqnuhl.html


<!-- 参考信息 -->