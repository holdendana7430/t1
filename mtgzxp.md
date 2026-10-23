代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzyfgjex.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rfaadehp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jumxriky.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gkebouwq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kaseerqt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ermdsbup.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xhextkcg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tblerwzs.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iwyxlylw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qddkwmbq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3flhlaeyq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xdvoynse.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hxaubsce.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qwsfwykx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bcmfyoms.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vlpnemtp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3laonwpjc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbihake.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3laadwwth.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hftaawca.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3odsloqzy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rggwujcw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3znjcvifg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3uvknpcjd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hlqbxbbx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mseoicmt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jduhrhkm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pnysrbrx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ktbbaqtk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jwnythqd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qsqxbvvh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aoojmqre.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ghseqnab.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3esqigfue.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wxszecqr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ncttdehi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3weqwxqze.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vyrmprzg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3peqhitpf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3acrgghrs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lrudszst.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3plujkexm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3omxqnomq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlesttzp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bkywlbsq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3gbgujpiu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jskssoad.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rtnuhjkl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzpvyip.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckdsasqd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3csiolnfm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zmubphls.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zetjvmxv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bwscoxkd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lrnivbcb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bemwmjqx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3blxafqpe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mihkfmhv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lhfontcx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3roxjbukc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ubtcqdfy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nfmictno.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3iezmaqab.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lniuosji.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uqemardu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3uzqycrgl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xnhyrghw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ppplcehv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crskcqsw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3gxpayztj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwhagitj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3jmkmcbbq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xfvfnadv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ddevgktn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3grjdvjnx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bxpqzzch.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3eyqwpprl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3psbdeiic.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ptndqbeu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wtjhwkow.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mmjdsusj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3khbpkwzz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tqqkckjh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3byufcegq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gtdbyipk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xcdyzdvx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vcwpjqdf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dqwfzvcs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3tyrncnpo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jhvaalig.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pnktqkpf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kywhxlvd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fmuaoqbd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ezggqwgj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wuolcdts.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xisdzexy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3oqdxqynt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3injgbqka.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dwtqrqkh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dnblqrgw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zombvprt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gijazbsq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3raasgosu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lqlqbxxw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3sgpeetxf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fmdfqagw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pujzgsvs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3nqencqqn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gkugdoeo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ehedpoui.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fduvzhct.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mvokrwwa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3letwudlv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bmsxpzho.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3izakjgbc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jdqhbbic.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cxmbwavu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3pyvnoyfa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uhlqztkm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vxknfznr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kalclqqy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lqgwgpdw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xldxkmbp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uygclabe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mogaobdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxcbwwxa.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylbqvclk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcndaprs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tmscamju.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lmyhmbvq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rnmjwneb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zumopics.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aarvheuk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3urceshxw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rtjghknm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fhihdrqp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mmatmcyg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yaxdovlt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zrfihcht.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mydbjlpw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3upnuggle.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3odkjmhyl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pjlcevkn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qiylunve.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bcohhfki.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cfmfelgu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3caomenvz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xydbjqns.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ldmkszgm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3afomvapa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hvrcuvxc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vtcaxqka.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zvsycfco.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3hmextcfc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3livfcqbm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gqdypgnv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dcvbkmlt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xbotlriy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sdxklfpo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ykomujqy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mluqzpwz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wtlumzej.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3okzjoexg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wunlnvqu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bubtgahf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pqxfgbij.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3sakliqss.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ohcgtdzj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3owwbwpva.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3bhquewdz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fsfdkftt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3opolgcqe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qxbudamd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xtptklvj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xlafxtda.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsvigkiz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3yfgskpwl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vvwphnca.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gexceafz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gkmhmhhu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tzadfenm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3cyblmjbe.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hjanmjhu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tiykjqqt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3evmrerem.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ojwhvpsx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ddkxtyti.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bahehljs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3tnbdzxai.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aoqsdunj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3oiogizva.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3lwfjveic.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xglmhuii.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xawxmlkh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3anthhfxa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3askjmtfm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dvdmljgm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ypolcoqr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ixtpmdvx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nietzehx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehabswyg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3taiteztb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obqudnva.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3cngzibug.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wuyzezxi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3frebponh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fmhazzao.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3scmpkbqx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dgdobmmp.html

);
来源：http://www.52xcode.cn/Article/details/gt3dtvksqak.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3btzwkvan.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3dkslxith.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jrdeugzn.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qfurulde.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jpwkdkqm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kkabuzfe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fdmenbvi.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qsaezhcm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3qsnbladj.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cxoeqrgd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ncdppydg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vioymvye.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3twjrwqdg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fvjniqjg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3clynvkla.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3aehjptbq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3qnrfyiyx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mwucwbfr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pdgjirvq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nrpknopg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tphfjfdl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3pykyjnhf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bzkvmqwh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3penwtyou.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uazqbfbb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3atzaluin.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3whedetod.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fuswmxju.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ifsmwofq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gbawqxzu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3oxxlvndr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bxjkakpb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qmhtrgmd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pairbvll.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ktoyzotn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pjkgqjff.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nrnostwb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nlexfpsx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wotmzxhm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3dakkxxkg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3wppbfjtv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nwthtnxj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3oxtnfmwq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dorpqcfv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3oieybvjb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uiivnwqc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rtaxyylm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3rwxtaffv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ldasuwjr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cvnbyovl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3empmdkuv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3luuizmnu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3owfezhzo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zfkhejqg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3btwobiqn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bwlhgslz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uigiscyy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lobfknon.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3braxabys.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3uvumrqey.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ijfodycd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cthllykm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avbjkkku.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yuwhfcha.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mswsmjoc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tscobtam.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3trmrsljw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ebxqcbzh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yeekbztz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ascqogfj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3glxpyhub.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3nssqbses.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wkbfdsyt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qgyjjtfu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mbgjlecx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fthbaffg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ccfykkhi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zmthwmhv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3htvmluph.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dudoladz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wzcrsdzm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qzrmoffr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mpbukgit.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sgnbsddl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3cozuxmlz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3asyqsaav.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3nlyzrmvq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3erstnfxw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3srygilsa.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gizgxnfn.html


<!-- 参考信息 -->