代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mamtqgrr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sprcgska.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jhzptzjc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zuadbdii.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hhpshizk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cahehdga.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wsqkdiav.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nsccowhy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hmuzeyab.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hyflfuzp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yhasxtts.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hrnmibtg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3eclbzorl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lxscpwyq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cixscgod.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3csunpqmc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3slgkcvsf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gvrhrrbn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tilupofy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lvhugbme.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isdemqfn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bcioyhee.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wfvbhixl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3svgpmllo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pjuieiqu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vkyrzivv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mchmzcib.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bmacqovy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xfqoghlb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vnbxzhkg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kycfcfjl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vzinzmux.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wrqatyro.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lkbfweub.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lfbponmc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ovhpheyd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3prxelvua.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yedniicq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3knvkqzog.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtwxhbtr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sxdrhsgl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kbujkmfe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3csmbbxlb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kwbppkbe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xvbkwvmd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3msxsjdmb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xgukjqao.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3hcbngftz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqyuhfvc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ngbxdnte.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3leggclng.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3timkbcti.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxsabzth.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zvopfcsw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulpbujby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yslqqdvq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dwkxtrfl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pyuwilmr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lnalcczp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hotflxpg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vqeqnfqc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bcfywqmi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3luamojtk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qtqgoqpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsjmqcsn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vqusmtoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krqirdsl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ariixbnw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dpjqtsem.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zvuacbbd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vvuhxtwa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zmtqayuj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hkwmrxxr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uibvifln.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ziusevet.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3apmmdusx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wjmtxmcp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3coadnzfa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vhiykyid.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kwjtvtim.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cduzivcd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kcdodggh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3egvikqdp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ulbioytn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qwnrqrch.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tnncydly.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jixixmto.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bczbnrsj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lzsljlhq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hrgfjiln.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jkbegimf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xqjljpui.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jaabknrv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjurexxb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qdfgyyim.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3unbbraev.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3sgyrgykw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcbwmwmy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ngpnybmn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3juptwpre.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mnumgbls.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wfwbgeby.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwezcdha.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3puybrmbf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ojtnqscp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qvdgtikw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ijuovvay.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hzeokooo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3atsjfgxa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cbetusdz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xubivbus.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bsswdcho.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nkpmmfrx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3xpojijhs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3tlecyufo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cbtpjecv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3seaqzylo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vefxlong.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3mmepblun.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tflkrawh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qwepivuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyuchlmh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nppejxgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekhjbhoe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gfceftry.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vjxwhxlq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3evslucqc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ijleeqcw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3buvueqsa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3snjdmowd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pqxbwmqx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yzhslmpo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zjxzvlwc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3atpbnbxp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3anhyzrsk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rezrojwa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nqdzieur.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xfpxjald.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tgiqbzqf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rozswkxc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvumylgk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ruujvhtn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3igohifut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3improckp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ygczffia.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sxkmwshp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wfimaiys.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yovvkwev.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xvoidsjk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dnocqdbz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gjqcrltp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3wvjgomhi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zjkcvfqy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wxvdmbqw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vuuunvhe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oismtzls.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yerqraux.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3dleyrgqf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3fhdtgnno.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mxiquiot.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3oqapxzhi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3aglrgaix.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xhgspngb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xxnyptkd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rxwlmcbs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ibiaflal.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ilwsvfcb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xpheftux.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vktdfmux.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3avjyikdz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yfizttuc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qmguwlum.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tejbcxzu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvooyvxg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhhyekcg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziohmezz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dnfnjycr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zezvkoet.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zpbvfbac.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ntmvhitg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uwwssaum.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ueicridx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jzgpdqpu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibawyawc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ustyraah.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kmkkjepp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zvfocmeh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bmqikqss.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpnlgxv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vdneyssk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3evehvqeh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3falhrzrd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3fivlyfgw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wwpqmqnr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3egmvbfki.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3dmjlhnhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fscppxfl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3xgglbxbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwtququf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mrjqvgwi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mgpbjkry.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hkkmfvaw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jkhrlhep.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3diiaqleb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3puqkinlc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lwujzyqd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hzlwojsz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mxtvemlx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lyijyewk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mzplcxht.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3yguikskp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dmmegwob.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bcplnzaj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ievxnkcu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fqnqqfcw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3obymxgrd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3htkntqhs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3xbyulgpn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ipevtiak.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3biloioqk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rqtndwbv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3osdukftx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qgfzqryw.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ibukkszz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uflqmiin.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hcwjambt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3npoyzvqc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3fjhqggrs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cxexdcxy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wanhugyk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lpdcyxtr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3hbvnpsjv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3aydgqcdn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fnnyxaqo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3pupgzhsh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ingyrnxt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dgdqdrid.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ewjbtymu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ezpejonu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vxvxcdbo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ncoceink.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qgqihocz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eqypawie.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3rujhpgdm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yqpmyjqr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rsnzllll.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3kafuwusi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ajfxixyw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ywsqkmnq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3megqmpvi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lfsvjhxv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3puuiufdf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uqhzqevv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3sroblotk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3icxnbtsq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mocpssia.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wmveubny.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3qvdlllbl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vdyaqwkx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3finrnxna.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3prqxhnjj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zixyyzzn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slxhvlrw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nkjeqead.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhltqnyc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ktsnwbkr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jrrhfodg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jvjsrbos.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hrxqcyfm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jijauiay.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wuyuxhaf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3fhkslgkc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3akqnumbf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cbwihxtr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qomewdbk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ymzsjpco.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jkeyshmz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ozrwtmqa.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ezbbweja.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3qkskxvga.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3tdtpleew.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3genfbsxt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jqjpvnyv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rxerkvno.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3sfcvdfpz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rimxogie.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rcyoiglj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vtxwyfbi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zihhwfpq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kgxszijm.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rqgmrmie.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lfejtjkm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ckvkbklj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hwpyftzu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ffjdcrzq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3oszlmomj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3uhqpcble.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3idozcall.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mrxznqac.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rqtjmxhi.html


<!-- 参考信息 -->