代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmreqscc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gosxauyz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ghtmybik.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dexpisjh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqxybhfu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rwskbggk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rblyrjye.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nunqvbyz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ukfanobj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vrfxciqx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cnhcmwww.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3qtjhokwr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3maycocpm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yqoahzgs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3kauvityr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3skllvkcr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ikgnjcgl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cngulczu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kgtdtfyr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3myuilngc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vmfyokmr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dvjcknat.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3utbfgkrt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ypiyxcuw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxpvlhcs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ksjpiits.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wboztufh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ogjkjzkh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lzyqzbwp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lzbjbnjd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hzzmbzsi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kvztalnc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xizsqcle.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vbukqdmk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3suzriybf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cbwjastb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jgtuxnya.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lwidoyua.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zrffmyxx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kijsvwqw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3owrqqqqt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zoqawoim.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3kxqcxbov.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsxvnwgp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mfdagjvx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qfhduisa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxwtbjcf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3pbvwahcy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpvbqdk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbnaetyn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vuasmggi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dghalzug.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hgdfrypj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3whdqhhvk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zowkymob.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xvkszfqu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lggopnxx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sjchcdzx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vglbbmii.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jpkxxxlc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hukobbih.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vtzllnlb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ssmjezlg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vdeabyke.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gmiozxxj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3awlswriy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jrrvsyrg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bfwqprkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ueegwuag.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3avipojne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyshfctl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bxbvpdhx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mxrkjrdb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gpggrdhq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nwjbwmil.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ofmjpuoe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3pllohhni.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qzpwvnun.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3egvllcqn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3haryycum.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xvrvwoer.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3onfhyzxh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3trjlregw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vitnrhhc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mrxwqipg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ojylvpqp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bochunjn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kfpbtwiz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ntknoyek.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qovqqmfj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zqcfugsc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wabvrxor.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gebtmwxo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kpzroqju.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vuajpdsb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vsqxhchd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rlwrdivq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3syjcqzkb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dlfmfjfs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pqfctcna.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wiiiutvy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuhcyiau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rzxoasvv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3pbemmjnf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tkdiyutu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3uxbwdfbn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nnhfrgmp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3hqihhlxl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kpklpvbc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3agdnxmzz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zmemaqew.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jdygnhjk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3snqfcafg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zvhtlzfy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mvazpdbs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jncqgwas.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ocaboudv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3miwyjlrr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nczazpqz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nwvvcwra.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jiqefjes.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3iysnkjmb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bnmwrmad.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3sqjlxtlu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qkygsfip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drwitqhv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3uycdckkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auvgjowl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vanudwap.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kkdhvrhv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rknmtpmx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ufbvavpv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ltefxvxp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3iheccrwq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jlhmthis.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ppyudlzb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3idloskos.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dkqodwcx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fbgxmron.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vnbpqhts.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wewampwv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jqajwpjx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jstsomqz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3krlrotbs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtrhwuns.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wlazszrm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jddnkvfw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dmbdjwzh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wbycshvn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jcigewtu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xcytlwml.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhjiyrp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ltyffurb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qrwlzdct.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vjibguhk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vcdesgvm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fyhovart.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dirkfedp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rhjntblb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qwzvcime.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ioshgjlc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tgbotosy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3eoruqnee.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kadkdwgk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hfxquogu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3puqqtahy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3cdqaugez.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3owhftyev.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vnvhtcpk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3juyehkef.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfomkjzu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3fuwqyuxj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3yprzjilr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3lczsbcdo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lsfrdmwx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wvuvuksq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gkfcbxny.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ktvlzcsy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qayfydnz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mvldilpn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gazogaac.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3buhqosko.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3howrhkwi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3uvyoyoij.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3blkywmka.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3myybtagv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tlqvvthr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbrtivku.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ggfhyoto.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dffmwuxr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zgzvivnl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3mhcueegg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hexulhzr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jfrejoxp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ostaztye.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwrmcakz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3oxriiggs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ciiybmsz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3inkmjrvr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hbocpnnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjblpsti.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3fhogbmrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtdsaesk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ocgxuwik.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ftnlaxxi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3osiccjnm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qyjevlys.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3yivwoqxe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3abkmbrsd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3baxyhppv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wqtnqzfv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3sjbxboaj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3aaxicmde.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3frjhjuln.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3vmoqcfwu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pocbjiwd.html

);
来源：http://www.52xcode.cn/Article/details/gt3eztqjdiz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3sjuqqnva.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3klsqrryr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qdcypdsl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qsnrswqf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ztcerosi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nfoegnyh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bqsnvgas.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ahlgmhnj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ukdrwwhb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mnczedov.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rmvavcqq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zzbikqok.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3edlovksn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bkxcpzdz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qszrlxsg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ojfzxuuk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3zopuaeex.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sinhimbp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tetcrfea.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mdylospx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lwhjgesl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3binoynwn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vupwjskg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3uyjeilnz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3smcnvyml.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3iajfhdzz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ouzkhxsn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kqqcfqyh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3urvtvjja.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fysnppjj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ekihlttn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mckofsyr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3hfuapsal.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3iyafphcm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kavuktmt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kqzvgzvx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3upggabud.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3itlpfeav.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jggekhvz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3auovqmfn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3bbwmlulj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3eqkrhxtk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3pgsdsazf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3xlnijfpk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gsobzbmn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mainsecv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3bzmxeqhg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3dnfqnxjn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rvtokvmd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xcfrnxna.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ssuakmuy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3icklstfv.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ptuvbwsv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yaznkaof.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yehdmdla.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lsktgipm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3apolzndd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jykzycww.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3orzcblor.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ujtpslbr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3axvtcbcy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3slvzeogq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3uiaupzmq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wvujwond.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3aqwefxav.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tyhpfaqu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3atovxyjo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wkgyxudk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xeqoufqh.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bbsbmoff.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jvveuity.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3exkxdhmv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dtwwhfmg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ksrxfkbc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tccjcdty.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3leaymmuc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rwrtuyxp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3utitfngt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3aqmjtzch.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uhrmlmgh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mayhzokd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hqcsunie.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fcugbanm.html


<!-- 参考信息 -->