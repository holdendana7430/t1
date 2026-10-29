代发 wailian999

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gcyxkgzpo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gcrdptafi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gojeybjlh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ghrqzywov.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gulveorzk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gqacpdfxb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gunotbhbc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/goihrxryf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gwkxqvkqc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gghnsiikw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gbmxstqpt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gltetaqqf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gbessbtce.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/givbhqzsi.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gaxuhgeza.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gdwheycup.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gmtysjgot.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gglqbrcjb.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gedpkcgpt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gpdrljwfs.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gkgpfruig.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gjqavsyid.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gdorkliur.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gzthhmzdn.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gyglzyvts.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gngfbuuza.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gcpxunibh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gytsrlwuw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gaysaqmei.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gutsfyouk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gvkpltbxr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gmlsawwax.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gxmqwyjlz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gkerclicz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gyczlbbqp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gdkzzbjqm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gftuhcega.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gchdonxcm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsuwkvcmi.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gkfbzettv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gkbsutgjn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/grmsaxerh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/grrgtzkpm.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/ghfkzaeok.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gmxpptqmp.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/ghvesesvq.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gjpisicux.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gtpvxfrqx.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/garsirdng.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gwkzndacd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gfxohzwrd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gqliirjhy.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gkblqmmjf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gjuiytece.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/goplsrepb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gpahnmcrb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gtfhlbtsd.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gbwazwfiu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gdxvyzzol.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gfkpofvea.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gvbjblitk.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/getvbqtqr.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gixpbwogf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gvzyeohir.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/giexqwhze.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gntgcwrbt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gauwdkhlp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gtxkduqis.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gimirfmtx.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gneiwlodf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gqtnodeox.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gmmhkoxqu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gcmsdeyyu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/ghsuwmsao.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/ggsqwsktr.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/grpypvlui.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/glojobegg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gfcgpzqjk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gyvvnwluc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gonthbarm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gwzpvlmqm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gahywdwsy.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/glpgnrjrk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/ghdvkjlyv.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gxpgwazon.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gtriwbetz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/glijbfuqg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gwkxdrhqk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gxpmrmfbh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gsexvtskq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gyzjzeznm.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gnqyyoznw.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gtovxtxvt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmvariefn.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjilcroie.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzrxsydpt.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gxulrmwdo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gptdeblna.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/guyukkkez.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gnubtgdos.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gpnbzsdre.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gflyesefg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gmtrmygsm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/ghrasuntn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gxtfbxkwq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gqydzgqqj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gaynagkpa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gdlzseyoj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gvxpmejcx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gshtgawzr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gayqiwdwi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/ghtecyeip.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gkbodthnm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gvyaoyobt.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/guqapaaps.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gsatenylv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gvhghlrno.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/goaiudlvz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gvsstives.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gbqqraxcv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gnpeuvxug.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gznshqvux.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gqywxbrxc.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/glkfnicwu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gpjtihzoe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gkyietoeo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/goctpuhrw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/ggtsizgoe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/giojebxyi.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gukgthlsm.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/ggpewaguj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gjwmibbxa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gwgxdckcd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gcieknmir.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gelbulvfy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gshcgjiry.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gxypmifnn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gacldydrn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gxnshhtez.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gkrwhmpqm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gbxrcuebz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gvtghvqhk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gzamcgbas.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gopfghzoc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gmlzevxgk.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/geeokpqee.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gvxhqyrdg.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gutvxdkvs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gfakdnzcg.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gmzxnnzir.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gxpsiuler.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gtigamzpe.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gjrnjiler.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gwezipjfn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gfjvpuyrv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gijxlmsvu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gznewwods.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/grvgcphbr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gyvzqlopp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gnectpzuq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/ggrsbxvzl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/ghrgkfwzc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gfwlovcea.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/glewizeda.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gwxaxrtxc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gctnjqpjt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/grcfmjfvg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gocvzwcvj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/genrbaupr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gvlvracea.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcwbptjxr.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gbrsiyusq.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gikpjisvy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gxtvslext.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gpucpuhlr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gsxqpayts.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gkehjhlup.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gsbejzoks.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gcpmbjnmx.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/godzikbws.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/geacbmivd.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/giojvucuu.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/goflylmli.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gzisombie.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/glqmkejne.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gzafshhay.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/goksicryy.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gnqcfiaya.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gfvlzooaf.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gxpbhlpjw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gcwvqlqbt.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gaemuxytq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/ghcyskgbl.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gjafhfzxp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gndpsrefa.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gxphctvqv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/ggugjwyve.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/guyntiqvg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gdrwmvmcr.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gsoumrjeu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gkgbciudc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gnayrvpzx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gzubsfwze.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gihihazau.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gvenzrmoo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/glpvuckfs.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gazyxaoad.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gqfgwizpq.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gwegcjewa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gvvyazrmw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/ghrmnmbza.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gzrmfjubr.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gibahnjjw.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gdulnozzy.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guzknllix.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gdjvdwdbk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gpwkokibl.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gxfeiqmrl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/grnbcjgfq.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gsxkmmwtz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gquohlgre.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gmtugcrel.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/grymqfzyh.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/goefequhg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/ganyckair.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gytanznvz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gqbiqkgqh.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gbkztbmwb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gbgrqczgb.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gfqeifpxf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/griyqgmww.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gxflnvitf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gkggyjswq.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gdmfjlrit.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gozyyhwnp.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gajbquqem.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxgecocyc.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/ghnscnglk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggtruvwtk.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gyadkoxbr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmkqqnble.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gqmoovojg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gyqkqqheq.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/giosaupzy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gzkcolcbk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gyekuqvev.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gyovzxxmg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gcdloucmz.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gomedghdb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gonpzxbik.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gscyngiqc.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/guehdbrks.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/grdwnhjip.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gusocobld.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gvhcjyoer.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/godjpadwb.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gthrvoiun.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gqlwvqpfu.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gksqpnzrw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gpubaepzz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gsiortsfr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gmuywwcxa.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gqsisfbwn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gydlxmwix.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gloosqfta.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gnaqstmoh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gutcisphm.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gfyjcisat.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gficsgmul.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/grgikpamd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/ghicbbeey.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gpbpadchg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gnbymhkqv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gmyvexyla.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gmpdtgnrh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gxtplawmo.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gnwmisqkp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gbjvqgpkw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gjrsxqahn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzsfbpal.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/guqelcbcd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gwljfolry.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/glfqjnzwr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gajkrsxbv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gywqypgtl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gopwefugl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gdwdjdjss.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gjhhlyhej.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmgfjwfs.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gvtpmgzct.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gtzcrxmlq.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gelofgwnx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gxvvafexy.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gjparhuwu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/ghtlioccn.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/glvificdg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/goxqahplx.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gaqrrlzbh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gmhvplusu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gydgsyayc.sHtML


<!-- 参考信息 -->