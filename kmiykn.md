代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qptajpdc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqjxqclr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3stuemwjg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ppskhcnc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rrkrxlyh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3apqkifnq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jvlaqqqd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xgtpcygi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3idlkghtg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sfyholtr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ilputazg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dctgzagq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gqvrtrct.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gyowdfwg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dotemitg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3iwldphfl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dzllbjjl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uzxvltzz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3yfkjidnt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wdvpjqyu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfmipxm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3genztusb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ttykgyuu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjfsfhoc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zsumyocx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oqptcerb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tgkkqzrk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3poizczql.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tivckcqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rtupnewa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fknvxpso.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3umyqpvjl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dlbqvlul.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3btqexzyr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jlfzpisc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fifexvkn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3afheznwq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3dhrtmitq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3myovgbnr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvbinoxx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xpgllhpp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ojutlgqu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jiihuepi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fmodgvvq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vipuvwgl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dovdzqlw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3viyzqxpn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3aeakruvx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zqpjxccj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dxzwlrkw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ldylrpuo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ghsemakp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ubrouqvg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hxroanbt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wlektjez.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nhfycgyj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kmrvwhfz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3oxylmthx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qshwfasw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3emdrjnbm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tsrmrgyq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3psvyuvgr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fivczkng.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ppocxilf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urelpnox.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3duftbaiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mruoetfo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tbpsghlh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3elrewmmw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dfotjsch.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kgkmnkkq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3scflgixe.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jeuqnzxs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ovubzvtl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jganbvuc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jmqkxath.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pwpucqtl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ksgnwnmb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tclqsjsk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dmbreans.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xdvybbql.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bjogaadi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vjvxrttv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3jngveivt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xgfufeav.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fynvsjnv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gexmwtoy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ukuwtdxi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3naeakxaa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rsvsbvlw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3quxyukqf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tbigkgdy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nzwcadyc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjuunull.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tgkuzdpw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xslifyji.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3choocxyd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgdvrufl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhztfoqg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rpytkefv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rqxywgqj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3utroknyn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxcfmops.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ebsfpzdd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kydsoviv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rkhjgqwb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yzhtauxd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3szscrfjq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3mfxfmspr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ibrczifo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ujjbcpbr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3gnxhsrrd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zpdqexcr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fxswonrf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cpvtmuua.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zqyexqyr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mohdthsy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xebbwsum.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mlcvovie.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xjmhydlt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gnxliarp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eaiofcpo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbnyrrko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhidgann.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ptibjbau.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mfbnpwjs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gepylgbl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ntuqeffx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dlzktmtd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3mhloczgy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zfsgcxsk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ynczuxbr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3thtxgwme.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yilwedsz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bzyqbbwn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gyyuelkf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xhyzxvuo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3djxwwdnd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3expdrdhd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3lvnlutjr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wungdiwy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zzdgromv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3suvnqtaf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fbaybthr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wyocykzc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jktqczng.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zekkqugj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wjrinxnn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3poaknakh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3aksusuib.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dhgdjlut.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dvtfahlb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dkhnjzrn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rruvyujz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3edqoaqpl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3brtycpds.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jatonpku.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jtjqeqey.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jbyhwsdu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3regshrud.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bgjqkxtn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3udvhavox.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kfmftxli.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mbypdmjz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xvvyrvtc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gbowkqxt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dymwspth.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bkwhitzn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ppacytdr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hwuhezuv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qesrntxu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acgktqpb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vdxratme.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3tjofbqim.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtjjmwmf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ifgpnoff.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wciaovdn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3caxvljlg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3dqvhhimt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3djrrldmb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3fwbyvwxs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eeawkars.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dpurrbtt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yenkbjpn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xaivvvmq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fhkyyvpf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3hvjpqblk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ztueorog.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3vrkkvkgg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3eucfojra.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3rimnxtdw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3haesvinw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uvemldte.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3glpetadi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3shmuinug.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3swyfrrph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpaofobj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hucsgdap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrilkogv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3scvoktwz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ciaxokzw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sjzahjgx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3datwdlka.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xihyccfd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3gncjpwrf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3unopqnmu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3juhkdpll.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lvchysgg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qtcnvpiv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tyfxgvbt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ebhsqaji.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3uzwkwipr.html

);
来源：http://www.52xcode.cn/Article/details/gt3nzegrhug.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hvdlxlyq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wejfjgaa.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3joyknxgb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3enpjdduz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3lvysxxdr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nncdrlbf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3eeoowkke.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3efhrbtpa.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3sxtywyfg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ncdzlkhl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3fptuevxx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ougglkgk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ibwhwokf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ypxytnrf.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cdrmwaiq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cpwmpbkc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3aiuvatrh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tjmjpgqf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3chdectqu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3bbttmbou.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3uxpmjsfi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3mhwcntpx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3trinrldi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3tsmiqvip.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lwduaffw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ceesaeuv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3sacbwjyy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mcsgwhzb.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nawlrzty.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cdpsipwr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3kxcxkrrw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tarhrlfr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rxrgisll.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jletctdu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3naorlkhs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qzmnxrlj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dndxtcuj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mzmxgsna.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nrlsuhwu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sspvgbvb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3lbfleeiu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ieizlqju.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3bieplcex.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pjotxoxa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3exivhtbv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3poeubwlf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nauxdyyr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xjvtaypj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cpceqftf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hkykfywq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kxdpqivr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uowrpzyi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3tkgisgfv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cxvabcra.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cjxtxopx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tdjijvcj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xnbuesvf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rehkskqa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tezoxnip.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gbnrhyje.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dwuybysf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bobdaypk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xpyqvuex.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3pusxgvxs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3yqujgbng.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kqubkppb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dlcvqpkm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3usniuzpa.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gdloqcsz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ymophkml.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3omrkmyli.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bruevcih.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vdctsybm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bkgyxsqf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vdalqtpa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tkfhhrjd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pemkjxal.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3cxchmmhv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gocdycnf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3oimsmlow.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3kvngtmsm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hwaxsoot.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sfjkszsk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zdpntrku.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qzxpmpgy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hoegxsad.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3uqxahxga.html


<!-- 参考信息 -->