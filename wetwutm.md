代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/giszzuyim.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gtnzkhmgr.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gefycrzbg.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gehuthwgv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gctttjhgq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpjrfmwly.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/ghibdlsjt.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gfegwzkva.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gxyqugtho.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/ghjkryrfb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gvlwjbvgq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gvcaaqzgm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/grhdsqhuk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gqwtienvp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gcednfnlb.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gexnofrmi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gscohafdi.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gwnrdcjvl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gitnnlxcm.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gskmxeyok.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gbcznzlvo.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gzutokbey.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbrldejyk.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gqieccirh.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gyzssuqjq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grovfekht.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gdfwranht.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gohnxgpba.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gtkduxgun.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gvnxlrsfn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxwjleffa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gvxzqnyil.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gtyfkkbeh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gnimillqz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/ghdiqsypb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gdzndfeqq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gkwdytpho.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/govduuurg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gpqbgidgh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gjomncadh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gwewrfkfl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gxkfyjibk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/ghszcpbzn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gzhubjytn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gtagspelk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gjtsivncc.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/geaaklbyv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/glrugzobv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gwbekhfrr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gjkdiviii.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gjvdkovbd.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gkvaruyig.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gvyfljbzo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gerlesigi.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/grstwnwbn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gctukpfhl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/guyzsonqy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gavddbtpi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/geoppehwd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gssieefsp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gqwnclhja.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gvtmwjlkz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gebsyppzx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/grhewsuwx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqrdiwlce.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gzfrzxilj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtfhigzjy.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/guewxcelt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gtnqhfntu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/grxqzdxvt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gcfynosiu.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gxodvwnsf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gnhbxxllu.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gsdjvuepc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gqjdtmtyc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gzylxmecb.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gotocnvbi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gdyfzafbx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gvfsncjvp.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghyfblduu.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/genoynkui.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gsepftlnl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gxcnywzdz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gpujaxovi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gfwxupbyl.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gtzuxxjuj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gdtbfwymo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gxsmykbdz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gxapgqxjw.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grgbtppzr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/geukcxtvz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gmiiiaeqs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/ggnxqsfwv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/grjxjcvbf.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/ghhqkzqjl.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gtsebcnnd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gtkhtwyxe.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfirzcbgv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gdljlrmdi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gdtjtxjvf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gkijnuiam.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gfutcqiav.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gcoaoxjzu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/grvppaxnt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gutfqpuxy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/ghmpmgaug.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gcynhqxle.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzeydnfju.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/guznmhknl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gvfxokjif.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gtaxhyywf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gnyyijofg.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gllzybajf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gwjciicec.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gfwcqpycz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gbpxnjglv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ghdhevudc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/grscyteyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gjnbathiw.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gfhjztoxy.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gkkazddpp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmlcbeqew.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gguysvtkd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsoviekrb.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gughftdra.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gribqzqgq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/grashaopq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gqjwuuabd.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gkgfvqbuy.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gxljqpozp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gtmyqibqu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gpubmthtw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/glfuvkddz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gircsrfxg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gygryxild.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gayvdtkvh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/ghjekxonn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/glhucqdhe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gtknjwjqb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/giwbqkvgg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gigpdpwhk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gdpexsbef.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gtincblsf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gjrewsmoa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gygmuwryy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gvalwdcje.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxqtfhjff.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gvdgahwbr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gtjhxsbuk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/guiwdaeft.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gqocyokny.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gqrlfqaje.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/glkekqwme.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gimahyxku.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gjfadhsxn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gygbamhfx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gwxwihpjh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gssrrhhel.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/grklsemox.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gpyevsiog.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gpjanlqzr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/ggejklsqr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/ggpwtsznf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gutqtkbgn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpeaoext.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gqwoiougw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/giklbyrah.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gqlrkaeod.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gwhvbzedp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gljjtsgev.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gyyxouimz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gmrasmfeu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/ggsvppgfx.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gmohtmgxh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gahqyunus.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/ggqdybsbe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gdextdsur.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbldrwprh.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gvmkvqlat.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/ghieleaxa.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gpozdfdae.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/guliihhad.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gcmuczira.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gmkrnhhgx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gmvdlqebv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/grpnyltal.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/ggatgkqhr.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gbcsawlkk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gsecbdwpz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gqjnomcjt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gjrxpoeym.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlsbykhu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gvfvsyujm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/goykiagvr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gueghjzzn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gizapgziz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtnjyvcub.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/goryptblv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqtdkdvwo.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/ghggmnxpn.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gwjdsupte.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gomppkfoz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gjvqxeaeg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gkvoazulm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gzcboprxu.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/glwuyuxpv.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/glcbxifej.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gtswkesan.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gfxxtxrim.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/guehctiqt.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gnzefajpl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gugvjesjf.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gkuqeacip.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gkfsjvale.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gtjzdnzsv.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gouyhgdtb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/goechjymr.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gwjkovads.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gzdxrryff.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gxzrfaqfm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gatjjllgm.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gheobyklu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gtzacamnz.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gwcyybdkb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gzkhnfyei.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gadxkqzyl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gbkafselj.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gdxwdueei.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gdjlgnuwk.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gycqdmnpy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gprfuwstx.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/glcepekqv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gfaqckblq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gnrfxwmrd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gbozbrgzm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gydccakyf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gzjgrlazh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gmocpcoht.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gryfdrpqc.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/grzuqoyyq.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyqavxeny.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gcegtbnlc.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gdgrwakjx.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gkwylrktx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/ghsquppgx.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/grsdwwrik.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gfapgalmb.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gzbvqhgcs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gwstnheeb.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gdymuxixr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtflthpob.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gjvcdvhoz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gsjtmfekm.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gmfzujiaj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gmsihpjsv.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gevjzobqs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gdodnaech.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/giictgcfq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwrdgoeko.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/glzdadoyl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gkivtcagj.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gzgpzzhxo.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkplbuans.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/goweayndx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gwxkdlqfr.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gyjygjjwm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/guusctraz.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/guytxrikf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glniexvgj.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gmrbfrzuu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjlbycgcs.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gqmpbmthb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/geiuopjjj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/goybpcaph.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjiqlbost.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gekeibrjn.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gxpuzcmdp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gxyttayeg.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gpytwmzfx.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gqwcknqfc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gwadjhkvk.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gaqsefxuw.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/grzoolhgz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/grbdvyamh.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gwaywbriu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gsszqezdq.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gphgptlqq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gwhdgzmux.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gbdfnltze.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/grxspcqyp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gsanhrqaa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gnlnltcwa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gpvrbozst.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gookhqhzf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/ghzzgyusb.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/glfegylbb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gfnqdvuhq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/glclqufrm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/glwevyxml.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gqwqjjrzh.sHtML


<!-- 参考信息 -->