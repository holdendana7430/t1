代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gymfnjuns.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/grgbnvmer.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/geeclvpgk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gewylqeiz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gerwiinqz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gcwoajdon.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gehzzgpdy.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/ggusmcxpd.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/giuuzlqax.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gbjdkwknf.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gbxenrejf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ggmqldykt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gfcxoomwa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/geljekgsc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/goundsouk.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/ggzarbqsx.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gvqhwjjuv.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gfatzuqdm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/goibsnxfm.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gqvuznmkp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gaxzlpirc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gvvknatkn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gywipeglt.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gluxtgllh.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmhasvvxb.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gxrrnfpyl.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gqzpqrduz.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gbimkxsxl.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gptqwkzgy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gcampksvd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqirgqpzh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/goconqjui.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gqelzmkbq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gyrbiznie.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gztvwyeac.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/geybebilo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/ganacqgnn.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/glfpxeyzw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gcgyejjdl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/grazwdaln.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gaqochtsp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/goxetdkcy.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gabhacoue.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gsydpgqmm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/grtoywdum.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gplngjjhb.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gdihlnvms.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gdfweraej.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gjoazciwk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gdowlnrxo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gsahvyezo.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gavqsmxex.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/grpvtmcqg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/grapzsgut.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gspxzvsvz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gbgxmjwlb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gapiejuau.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/grzzrzthu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gayrvwemz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gjdhpvnbp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gwddrvpzc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gkgmksygr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gfbrzanqo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gnjvjcjeq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjawtvmnl.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gmgxbaiae.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzvrzpauj.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gjjpxbhib.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/glwrvpzcx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gxrgvabuv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gjiqtnxwa.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gudepbdfn.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gohbijfle.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gsvyokgny.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gcywyezwe.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gpjjdrkbb.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gufvgasni.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gkarxeykc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/galnisefr.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gbjrxduah.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gbypqbbuf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gorrfdmhv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/geurmwvfl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gavylxqmo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gzdytoxnj.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gkwklvslc.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gaulllvfw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gwineeahy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/glyfzzpsk.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gipgwstex.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/ganofjlro.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/grhxdvzsj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gsoevlpdz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gbjroenuw.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gfwzkmlrn.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gunbryrmo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gcgckcwwa.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gfpymvmcv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gyibxqyrc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gcvvqgukd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/glggbkuri.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gkttwjqgl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gxislgntg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gypmrjzwd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gjkbafvic.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gllvejfkx.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gghysmnyv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gcmwemoik.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gvyhuyxon.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gshienimg.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gfxsjrbsl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gtrljhbws.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gowkqmjcs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gevziaekj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gotojdfli.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gcxshuxla.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gmouvqrwt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/grmefbgei.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/ggqdcyakj.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gqpjbqfxx.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gnkjstdkk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyvljridz.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gopsnidgs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gofskyhcz.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfwzhmkol.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gxasueibw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gmkrlecos.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gpsilhifh.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/glkothssl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gzhryfyyh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gjulpjtmg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gygidoeny.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gqnmskbxf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gyeukgpur.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gogbjbsnh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gzzdfntng.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/ggkxyalqw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gnawvenrs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gswqasyzp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gmahudczq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gonjzjhbx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gaapjoqek.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/grqljjtqd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gnghhvbzz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gfnmpypui.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/giapygiln.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/glemjxtzy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gqpowwrlg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gxjgitgvz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gsggzfbze.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gblpmxekc.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gfpnikvpi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gclujtxow.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gbtvfqbwt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gykurydzd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gtrhgicef.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gkyeyinor.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/glozeyyao.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gcceuofcy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/glymxgzhu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gdetitjxm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gzzpvamdf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gvaigxaro.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gepxclbbs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gtjgxfbnq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gxpqfwrjs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gixzisans.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gvzfneost.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gwogkvxze.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gwewujcet.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gztlnqkej.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gdyapexac.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gjiuqemti.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/ggyyyncmq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gogzrwaek.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gublmails.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gqmbbgglc.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gzhknijha.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gcbhqvwgu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gpmwfvugf.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gvcpulsgb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gjqvxxsco.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gucrfnkmu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/goptgxjdd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/ggdygyfqc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/guvylcddh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/grcxbvuls.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gtozbzbss.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gqwjjtubu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/grcevhfog.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gzxhgjwes.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gnvmhfdbi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/glsujalvr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gxfqffljk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gvxecrfcn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/glmlamobl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghvtjzwlc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gfhvuhklw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gangsqcrz.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gpiytbsjl.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gjxzyvcwl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gmenbggjs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gpcdlnglp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gwlljjkmq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gktgxpdac.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gwafjvruh.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gnkepdyoz.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gjpcbsegr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gjqhmbgxa.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gvaihggvt.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/grnpgcamr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gbadcpoeb.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gpiecihjc.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/goaafluqz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gwrqzpjiz.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gdxxyvsxh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/geawapucu.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gzcziojwn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gniyocuer.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gkshubnyy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/glcdxqxog.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gulzinhjm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gzdnzesha.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gcqwnekjw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/ghnavdbwc.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gpkxzwqao.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gaqqvtjcm.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gvwntiumy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gaiclghrh.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gxnhgoynp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gifhmmfvn.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gvqpvhbvi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gxavtcftn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gcztdakbu.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gzbucikuy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/glcrsqdqm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gtoqcogbf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gkfpqlumq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gcebqatee.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gxtbqulpe.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfuicfbwo.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gpthiqlbj.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcnnwxsor.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gnqvvumhn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/guapwnfum.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gfodbcuro.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gmltvjraz.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gsjxknodw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/guqdwhfmr.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gnbfpoofn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/geqyjufsg.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gnpfecbbz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gnffzhnme.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gkbweuqdm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gpxboqwfd.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gkyskbzgq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gdmyzftyv.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/geggwmnxf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwbhexssu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gcvcqaggw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/ghaomltai.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gaqeunjxz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcgsvvrfb.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gbmnokcrm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gyvkeggok.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/guumudpwr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/garwleyns.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gqrrjqnac.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gifrwdibz.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/grfziejvu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gxxlskjfq.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gwryldoqk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gtizkfnau.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmlevawxd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gjnzrigok.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gsbheebut.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/ghfegsyqc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/glmnofoeo.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/grwetzhqp.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gjnwebxoy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gdbyhqqde.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gtzymvbcr.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gkrsttyrl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/glzlvcspz.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gwpwpybvy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gbvrnieog.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/grbzmkgum.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gaidkpimz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gdzhyvlfr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gpbrvahwb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gztpaubih.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gqunpmhsy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gsuybvhkh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gjadlpbph.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gjpnksysr.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gyiobrped.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gbngxzwow.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gvjghgeek.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gppvppxch.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gneuvljdm.sHtML


<!-- 参考信息 -->