代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yjsluyzm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xivwkrga.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xhpajfte.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rfkeiblf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ytmvviem.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iaokmcle.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3djzbyrsq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jsnqkthd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gmmuuqik.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gfinutmn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3frzddtpo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ekqegcyy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3tlcozwvu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kmexxfdh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hivocgbm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hleklwvt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3loddqpft.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vxfurqry.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gizyxkku.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hommcuvc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zvwsolnb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3esblbdjs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3recsglgg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lyrumufs.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fysbkydh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nwmebgla.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eyzwriao.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yolklxrl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gylkztsj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3imtwaxuq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3nmghxqow.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wthzqtoy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mnactbfp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lrusesqq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3clusyfxd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vnxgswpv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qechfdxs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3gqurlche.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vlukkudi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uvsetqza.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hcdfvcjn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3exxvfygq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lxfoddbt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3azrjzdzu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3atdiyhwx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gymbvtlf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bbkplcnd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ydykhwsv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pshzsags.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3yadghnkv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vczkcagd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3wqnkcmzi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3aajwvqcf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wjbonzkf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lwybtjtj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cwwyotmw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nmhbnkol.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ojursazq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hcgzrpgv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3owdxhisk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tljjqccf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3byhuwnow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ethgdvjm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3fwiffhbn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3txkivgtl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lgaohmwz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3olljepzf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gfylndiv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qvujgmww.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bkvtbxyr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3luzewxkm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kxulgsqg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cezmxgmp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ltecgjyo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3korkklej.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ovwmkzwo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tmpgrlfe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zinkyzuv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wffavcdp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ouqyaxut.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3tpaqonxc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pmxmwcxs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3odfadtzo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xmoydnuj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mfjnjfcl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ginxcdev.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lvcqhfgy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kcunsgod.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kzmvsbkg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3axaemezk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qyplwweu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3gkaibhkt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lbvvjljg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evdgulec.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcwrhodr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3oxuircvt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3gyiojavh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jrcckzuf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3homyhilo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ziuaogzv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zaondhnm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3iqirzwpa.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3grsjfkhu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3reuwsawn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gkblkmxr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3clomivua.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjcihhe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kffviumz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3caqocefx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3zzdqefuo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3naaswdgw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xbbsyrzh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hmylbkjh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3omdvfryt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3glccewry.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xvwypana.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lhecuvaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htnfsvho.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxyjsvle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vktgjjec.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3laskqwap.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3raouugrn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rlcdjucw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hnfrjlws.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3udclbtsy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wvmqzucz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bpxpulbu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mfyfzvms.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pjersvph.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3grpefghh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kbxesxru.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qrvhbcme.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3etcwcmje.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3igstbkng.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gdtnivqc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dcqahaem.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wmwjsfqq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cocndtol.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pbjtqpwg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3byohmmeh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xvesifpv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3srcafjnu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qpnjovec.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kzsxwfrw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qdpbyzmh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3fiuijlec.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qbsyfctf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3sfevuuqt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tdtkzczb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dwctvqgf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mrrqjkcq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uzhezgfv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3istayhii.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vpffhumw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3vllygjhh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ekmlpure.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cceyssya.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3rmsofjbz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ufjigrcy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3apfugbbo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lkirkbvw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gnjywkdm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zxzysfir.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jfkeayna.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3fkydrsaz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fluqxmjr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pbcmojso.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ulnzyhgr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3sodynwst.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3jjuzzjle.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dozjzjhw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hzqfrkrd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpakhdh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urmtnmsr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nxofltep.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ioruprqj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lzhhhrtm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3npevbdka.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3oehykcva.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3edcctnfb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3oucszuck.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jbxxrsky.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3byetknni.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jwzuhnnf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mvkklpig.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3bcmcxflu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3iraurjgi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjmlxpg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3inipoksg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xsctyexl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zhgnyubt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3uuejopej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjmvwnqj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cozfxbfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qujtbakk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3uynpyiut.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3mhtktkck.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ghtokwqx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vjqrutyt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fadaasep.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dbgtxcjw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yhrgeupv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ositpyln.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sqlrtewh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tuyaxciq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jywzrvms.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wrwiizza.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3lyjegswi.html

);
来源：http://www.52xcode.cn/Article/details/gt3bsiowtyg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3uklugncx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3eavuazem.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmpjvscf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ilfxenlo.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ggisutnw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3kjbiqeru.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qbjppekb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3nxkccrao.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3czwrobvn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ainclkxl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nebqzixm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ggavipnz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ncojhuzg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3eqvstlyh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zihmsymi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3khgpxqgw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3prdhrpvi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ywyjlujm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dgnhdqed.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nyjvnyle.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ecersrrv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ivtsthpw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mwehhvfd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3guhihgqm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3pknvzuvs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kisfecko.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qigdbhwa.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxlqvnpg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nhwzxfeq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tujpjdow.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dwwfbdsp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3pfykrjmt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ohfprzkg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bmvorscp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xlpblgxc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3iakukkfj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lmsacjuh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lqzuxnao.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bnxkabkn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pnuymyhd.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rplqpzlz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3txdzebyu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3odlbvkzo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rdemnllp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3pebhprrf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tmkzaayt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fytiyqmw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3moelcqyr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mdhzhpse.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3usntwnnq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dzqayxhw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nufkgvih.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3govgubcr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tsunxfjf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ytcellqs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvpxuwbd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qemzrpmb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nxkimlqk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yxicjiee.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vrzlvoaf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fsxgfxyn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tkxbfvhs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bzeglbog.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qzjrflef.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xwqhuaea.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bnkirfht.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rbxdvmtv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3eqedlfje.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rmfxlfdx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kzpruisn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oyxtglrq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lsxbfhdl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dpyyqbix.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3biiylhmv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3guecsgel.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3xdopbgwz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pnbflqzs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kbcyacjo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3jnfqzamc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dxrmveqz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3yetwrqmy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hefkdwla.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qojhenxe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kuwyslin.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wlxmokwq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rjocdcsv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3whngcqys.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3waptkzax.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hnxxqgne.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zjjznytt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3amiysbmt.html


<!-- 参考信息 -->