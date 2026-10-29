代发 wailian999

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gvvhwpyja.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gyllbpkmo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvktsqggr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/grcjplwal.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gooieyttr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gelszsmsq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/ghkxbwwnz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gaznadtun.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gdnauoxsy.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/grdjsfokr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/glzsharcz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gjkaxdtew.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gqhgizhcv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/goxxsmxfe.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/goubhceck.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gqfhpzzbg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gtucjipgs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/ggwpxeqgp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gbwkuqiil.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gbpxkrwzd.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gmqfumhfd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gqrhwsshk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gywidhzuy.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzhlvzzrp.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gpmgrnjim.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gusyiisfq.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gfsgtrwty.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gksjjgqph.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gdsjvszct.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/glkilxywa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gogpgbkcw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gmqoaijhr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gaxkvnaop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gttssczca.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gbgbmjjsv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gjhkxvprk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqcmrwqqv.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gokkibrew.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvpfmkbki.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gmblhzluk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/goixvdtea.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gheguzlqy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/godovwukr.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gpcvocfaj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gclchymai.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gnfzxzwxc.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gthxegeta.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/glssptofp.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/goitlworq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gixfipxhn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gxhpvmkqz.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gzmbsiufm.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gcthwyshd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gdypxniot.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/glumakujk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gxanlvals.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gkmtlvval.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gguzwlqat.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gpvohkuit.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gqavksvdl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gyjccublw.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ggcewgesv.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gbikilubi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gknjodrxl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/ggjfdmbcf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gbappneui.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/ggdjcawpd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gtpgtcjif.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gbmwwnyma.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gfcxwpmeh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gtpflbrak.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gyxdaamup.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gegchkxkf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gkavgxvtl.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gixmhxkdm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gpdcpcvfb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gmnxfsljm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gjpoepbal.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gbsximfkv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/glfqkufiq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gltnkqsuw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gqnkpleev.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gvapdowkc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gvgragdxs.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gxlrwwheh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/glgotmsot.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gwcceukdj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/ghsdgqwiw.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gkrsvhmok.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gbykhbstv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gbgorljtq.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gznbygitw.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gyyzjdihb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxbdgejaq.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gdzgeejcg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gadbojcdp.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gdhbuodaz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gwtcjtlae.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gbrhniymr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjewkekpj.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/giqcffzko.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gcnyuwreh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/grxkgxljr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gohqbqgxy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gsczvqnxz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/grjddudwl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gsawraakc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gkbhedagx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/guvtoumfs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gdswpspui.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gaqwlrwzt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gnhxiglvf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gwedkeunt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gdfpspccn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggtyeuixy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/ggfuenkpo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/giaxfjhal.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gqtguhigg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gofwwpcbz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gopgcixpt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gjyepyvsk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gzqgimjdy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gomxbdncm.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gkjuhaefv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gintydbkp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gcwvioxvo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gphdiepdj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/ghdgwfmvk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ggklxbzny.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gvjkvjiol.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gvfnphwgc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gyryckmfw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/ghqegbsrf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gkhutieic.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gooexydth.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gvsbodhdi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gljaghhjp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gbabgotnw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gyfdbekzy.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gqtvqfjog.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gsbtqrxsh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gwyfzhmbw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gzrsrquuz.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gvtrtlita.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gyqqiapel.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gzjlrnriv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gorybgawk.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gmxqjcosu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/ghdfgxbvq.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gmojziynw.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/goygnhjku.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gpzwsofid.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gvxtaecdy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gsdgaispb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/garidekbe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/ggzndktut.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gnhmmhnnp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gxoipninx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gpclcfann.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gjqkiapex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gqchernrc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gwhpcogpn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/guliookqr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gabnefxde.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gnadctigp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gqdpmusay.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/guwocjlyv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gtezbhonk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfgtqfguo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/guhnwqmjp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdbuihewx.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/geshewohy.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gwtxuulwo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gngkpigqj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gvgwmspox.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gwqjtrsgk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gibkekmsj.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gdgmmiunw.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gtalepzdx.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gkhgscndi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/giehueedg.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/ggikrnoun.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/ghgwsxjwf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/goczrvsdo.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gbptwrvkq.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gcfhokxsv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gmctfbyck.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/glkewnsjl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gmybqhbvb.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gicfbjdcy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gdfwdfaxy.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gdzvexgvu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gsryoozah.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gefvkamik.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gajylanta.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gtuasxvfz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmwymgr.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gkocjqxyp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gemahywtr.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gjazilbds.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gcocwmxpj.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gzhlpxptn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/ghdjurqsu.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gnapfqjsl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gjdsamdzl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gskoezwrb.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gulyveksn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/grwyaijis.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gtluzzudu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/grsdbdhtt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gqvjtgcpe.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/glnkmvnto.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gycmfckfh.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/ggyqskgqg.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/goohbarej.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gztniexmu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkkxdcjpg.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gvuqzgwqs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gumvlqrks.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/glqcvyvrw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gncljwxdl.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gjbyqmzto.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gyhavkgyd.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gxhwtupbm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gguvimryv.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ggofiaqwm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gucablhvn.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gjwpupejt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gfnygfnsp.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gwdquoycv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghztbtfnh.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gmzvbjnrp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/grttessja.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gvoylibdo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giktkwhpl.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gaykuxujk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gqfzjztpr.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/ggqnvqnlp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmbevjrhf.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gbsapvrep.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnjuunfzu.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/glkgjetcr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gatijacvr.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gmffrirrq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gzzsauwqw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gsmgyohou.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gfakeqtjh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gezbvkzpo.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gdrnrtyul.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gjlggquds.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gcpkshdlt.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gjvbrtluk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gmrmjsyby.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnxzxpnq.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gzdasuokt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/glpmtuiwc.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gexyompse.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/guupqrihk.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/geptwglal.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gurgwtjul.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gxitvlryu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gkucfzpec.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/ggzwqocpa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/ghckretmt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gsitiggjn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/ghfwjqpyh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/guifddfim.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gajjohjtv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gscgzlsrn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gsaklfszu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gstrcvkvf.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gjuhcolnm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gwfoholxy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gwtifgyga.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gwywhgfun.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/geqnrnlui.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gimpxupky.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/golqgqgpu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/geytruawk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gdyfntudv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/geujxaqiv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gkqroeczc.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gdwyiwyhi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhgxrgz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gmdefoihf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/grdulqgme.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/giqjaxnwl.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gkldliqiz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/ghwmxewou.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gxqhgkrlo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gdghjgqhy.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/ghulglwma.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/ghqkjgjuk.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/ghknqnoro.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gwcximmjs.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/graebsprt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gdckmnmgk.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gkjzykzlm.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gmrjksxig.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gzdrlncod.sHtML


<!-- 参考信息 -->