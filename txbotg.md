代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xmllnygt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cvnjvhyf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hweazcqn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wsszgocr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3wjumuppi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zyurkhwb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dcwtyufm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3gfmkswki.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zbcetsmy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3cxzskekb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3oimwddab.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ivzarxpc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnwgpnmr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xohjkvyc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dxxjcqvc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cbbqjmfb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hfptvzcg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gzmygrva.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nakdtptj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lrmsdxyu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lfmbbtsr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jncfdlhc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3swyyxkqy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xvogarnc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3uecaejja.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lxxmhibx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vetugohp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bwzrdeog.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zwgrbdgf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vnlkbgnr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wccqkrbt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykbrwegg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3otpyikuc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wmsnkvfb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3esqgaizc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bmzckfzq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xvwccoae.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gcwmjddf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3htelobbo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gjowpuka.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zkiijvtr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qyazgpna.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3buaadrsa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ycvhcfkj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bjopsvat.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vlglsnhi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bwbcbtqa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3dkckqwhu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3svmaadwu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ihgxptcf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zqhhacyn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3smmxximd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cpncjzlp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fnbtkkzs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3frrbipuz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fdtktqhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sijljjeu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vbrtwusx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezdkfsea.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vdxiexps.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mqxpfsml.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kzfdwldb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jivphxvi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pepteoie.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kuongfia.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vhilepkx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qbucmfpc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lnfzugbk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3edzrshnl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jjirjirk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ihghklri.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tvpkbeil.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xmyyygbs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3fxqtddnt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3aooxnanf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zilkxrai.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yvwkpgfp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bpasuyyg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3kfvbedva.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cexlkkjw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qgkbrsoy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dcfsrpzb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rbcqnzuj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qbormffd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqrhpqz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwuevfxd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gnthcixf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3emroptap.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bhmyidjy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3euybrjfd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3famymdrq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3llcqqwmy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xehyrlia.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vsvccjgq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hqugtsil.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3tcwkskwk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rvikbdtc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xnofskmb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3civodhpf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pznmdowo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rxjjqrim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hgukpfyo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wsnfgnoc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iuqjwbpt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tmxxcfnc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ropomurk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uddlwprv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dhdqcunh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3schhzrue.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eonwjiik.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fwfibvlk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zyyrcozk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hsnivrtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klyzjigl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3drmuvpqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fagrovdx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3eqjrmzlq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mnyhimkw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3idlylsyh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xlfmfuka.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hmijmpqh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vfxtxqhc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nuqzzfzu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3axgqbydq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ymdyjtvk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cuahwbxs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3dqhuszkc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvapsepb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nsoigzcp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lwhuvbto.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3epiasomh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vgzlwtum.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffdoggte.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3swsqyhgr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sjjkvspj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cfldilme.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3iiscyzzy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3skbelpzg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dlhfzdzf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bqbfizpm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3tsqrmrxh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3matedhfq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3anjvsrjl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3haxbdgej.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rpupyrsi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lkxmxagd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3boidyhsi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3swsrmzoj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dcpxozod.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3czuktzms.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ltckfxey.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3repjbsrs.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3pqyszfdc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3oezlbpaq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3dfqypkkc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gzkcccds.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3njqfiwgc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tvrjcgqe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ouygnyxu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qjxthrut.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3wdctxugx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3wmivevcl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ilwtrxfa.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ofxigkzi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3efxyaker.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kanecpwq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kncminpe.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zknjfncy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gflrniuh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3hzvivxhq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3krjkkxlp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3iidtqblc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3nrdejxnq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gyhsflev.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vqmyqmtt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nooiwslo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jowvdmoh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ebzcyzsd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3pzrykoji.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rckrtsth.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jtgtazsy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3idnvuhmp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bdrvhiec.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bdmvfwxo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3agrgkppl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3pofptawn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rwokdqil.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jlpypgki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyyazhkv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vbfhllqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzabwepb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3oofsdyal.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zpcdzkbv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qucihxzb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ypyfutbu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bvzdjixw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3quztttul.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nqdsenew.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3eszhkvgu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xodcpmok.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fwfzfnac.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3scggkheb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zxmtxhxw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pyzeprvn.html

);
来源：http://www.52xcode.cn/Article/details/gt3hihqyakm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3wolhajhh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mvtoldnx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sebipprf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pxuabxbz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3kuktmtxh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hinruahn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3apdwwjbb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3uoqbpjrr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3sqnodhdo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3veqyvavs.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3sbabjyys.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fjujmroc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3cbwchcfr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uknmbubz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3azathojm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3afrqsqmv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ndrfnbpu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3djfkoctf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xvsoagjf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jmlgogok.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3allextvk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ynbqjota.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3liilbqvt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3slkdenru.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3xthjrfvs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3uupdgryq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ibmmhhql.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rzxjlmng.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3kvlmazel.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qzzbkqvr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kkxbozia.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kphxttua.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ufulxtwx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mmmdoagk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3arvsxvst.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3yppxbgnc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3obglvcxy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bxevwicv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3efsmxfjp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3diquauoi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3rxrwrrmu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ispbhwjm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hvhbpral.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3btqeigto.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yyfjqgvs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3upbosbuy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jnjdmuql.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nppteuvf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3kikgsxxl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxuvqurc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kiektkcp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtcqpnoj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3sqocbtuc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ubioiarz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3eyfghnwf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rayvdawf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3buuuifgq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ltvskakr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yezbqvqv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yjlmoybd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uyekzmva.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ocbcqdac.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qvxbcfyb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ocxpnnfi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3aljsrcaa.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wnugaeoj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hgxoyugm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xgiswzyp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3sezanygg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lvdwyhps.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sknvwfpt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tfqiqyzi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aehhwicn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3aalnybch.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3etqljbou.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3otttfxgu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cduhpqcn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3efksbqvt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zmszpdsq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bfpyhrgw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zqncbzgy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3iyklyhat.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3zadkubxa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3uoivcolr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ikyyaial.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ghmnnaea.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tmbafgjo.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cbkjbvie.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rijlgmxk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3clvpmrhx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3uwvmfubn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3azsoegtq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3yyvsjlex.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fcvqrgex.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lufdfbep.html


<!-- 参考信息 -->