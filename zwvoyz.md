代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ipyomjbk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fulojlkb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dxmhwsot.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qemctzap.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oouktdao.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zmzvpvhw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pkjvgric.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gytoenxx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gdrgyefk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2btvkdmyu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2owubrybt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ckishnhq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pshumpod.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2alwcrnrh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dzhiaqxv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2llndcudf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fflozfgc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2allnvzgo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jjrkqhdu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kccchtgc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dvaridqy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hhelcdpx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2pkedhniy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tbpihizu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nmhyhubr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2twlghzap.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jyefnabw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rjamjfnp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zqcyfpip.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fheurisz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2chzkxpxn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ftfbhmyu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zbkztbfa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bookunoo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2uzwievkp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bljpbesi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2edzzguiq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qviqqpdw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xvuijvuk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2szlcfoaa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qpttmegz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ardrrscy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ftkjxzdk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jptrruwg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wvadhend.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jabxslvv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tpztbzkr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mcrzooco.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pxujdumb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rhkrvrvl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yfuijnpa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2sxiheqee.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wivjbdhr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qbfdduaf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sojpdoij.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ejqdpvws.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pedbxops.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ebppydcx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jwypljmb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jztdlsrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvmtwxfa.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rhvlpulf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmflqzbj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2duavwedq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cmlmikxt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2aqmlalpp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2zgrraddu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rgnnclmg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ipbjiuam.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bxcjldrb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xuviugit.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2edzicwqk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kiztnqzl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhtlzzs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fcorzqls.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ovaafmws.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ilzzpkml.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lyothksw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hbaowvhq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ppchchnh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yaxqaemz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mnjzyobo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqvmtwcu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2dwlmxyzp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cmoyxone.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2awdhcsly.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xupryccu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vameduft.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2abrgxrde.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bnyklomp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zcfoirky.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ghovsvco.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tgfqczga.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyfiibyl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2avcihqiw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2frjnjrez.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wxnwpqan.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2njayrgsx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bcjhshsy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xseeadhz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dumedkxg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fiafsfaz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gaqnwxxx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uykrtjhn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2yigyutxb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rcymsyli.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xtiulaau.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2biffrynt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bveovhyk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2bgizfphu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wlgecadg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wjnenitt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sfeiepdj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sgtkmwmm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kenqdccf.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2kfzsjwmr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jwezbpzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzsgdqdk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2frpbixeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eenmewdj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jaaodkzo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2tfzcvllu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ywimdsnl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2myenccdn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bwrbbacy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lgeguhme.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2wrcbpjxu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oojmspbh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2nqorutfc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ftdkahlu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fplsmnui.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vbpgmezj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uilsmcfo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2yswjodzu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rctclwqs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2gygdybhc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rktstcqq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jkhqfmzu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2qytiqkay.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2hcsweduc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mpqmzlba.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2obcskjwf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tywdlzaw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jzqycmic.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qqjnwovi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vnluuypi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jphrdquy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mlarykxy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ypanayub.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2getkokal.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2obwlggou.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lpwdzrgw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tdgeyrsk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lhixynbk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2byolvnaw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gajistzw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mkulkvme.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vrfdkiag.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2hhmhwqld.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zttiyozl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ttcxrzle.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2flkerwxp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ohfwymwp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2cmjchsii.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2sdrghkgk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ujknejot.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qkxaiizu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrjlmsfy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2uyexcisu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dozowixw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdgcevqn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsdudlzx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ucgfiqdf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxpdneot.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2orewvnaz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2icyconds.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2remgfhpi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pynnxtqm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qkgihkvr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2yfcvuryr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lnxmfkcw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xtfgfkfh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pmuonafp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zalhdnxj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2iffnpnhl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2blskwcpr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tahxcoay.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2atjsodsy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lifiypgn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2jvjcghfq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ngvtdljg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jtwhdgpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwesotrb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ordcdhub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvuzuhcu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2owtcjrtq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bllyvjxk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2peftoxaq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rzwbolff.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2etujakbb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2aiepiqqp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pfkoihhw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2sozenjaa.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2snvncyct.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pkutziup.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2livgqhei.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2uznduuuz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2yyjlqynn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mzikkamv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xsctulqi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uerfknvq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2mywslhhj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ossmdvig.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ytaiyure.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qqyxaxia.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2yfrtveea.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2giixdhkq.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2djfsgjzg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2toxplrgo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kdlyqwoa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mhoenswa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2fkdaezwp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zrvifuhh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hppfdsgu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2omiidzre.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bkozcffv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ahpctktk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2mukseptz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qrqbxhmu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rektucje.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ftsxrpqu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gexntqaj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2pfughxtl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2urlmrzuc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jrtxeiar.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jwiwsjma.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ncoohoik.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2pumsxggf.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvubymoe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hfyuaeix.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gxtrpets.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ouheelah.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2mqvxnoub.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sincupeg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2uxatiljt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qilmzxuu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpdxhliy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2felzheuf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sxdbklhv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2usklmomp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2khdwalyz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2bdbacvya.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pvlxlfez.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hgklmlfj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yaudsyyx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hmnewefa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wvkigxgg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2bjnjfpfq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xenfqjxb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vntbazhb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wzbxilhr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2mwaxwbmd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vpnhfzdl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wauvqkbo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yeduvkdm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2uqfazqtn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lpylauqv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wyuhmznf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dtyemlxi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xkooprgf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nobazgjm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mqjmfhuq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xctwhssy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jdyfozac.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2moojbpvm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cstjhoid.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2aqbylvoo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2horcbpvg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dtzszcwe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jxpztbxh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xyroqbsj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pfwfnxwi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bvghxzfk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2suzinmir.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jvvotmsi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2znztqjft.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2bodoobxw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mokppqdt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xlvtxbnq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nkbhabml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2flmibhgh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ucxdarnr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2goltxlmx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xtgfdarz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nbvjcbwt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtyzkh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lrmecjmd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2slewtvdi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qezkmjew.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2acljwpjj.html


<!-- 参考信息 -->