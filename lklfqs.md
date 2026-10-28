代发 wailian999

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gtcfggvzbu.html

Ruby: // 手写 Hash
来源：http://hz.mhx1999.top/gtuumymzes.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cqqwz.cn/gtnlriuwnt.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gtfurdcesz.html

Py:   itertools.permutations(arr)
来源：http://hz.xuanzx.com/gtxgxocwpn.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gteuvuwsxx.html

JS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtdqenrywk.html

TS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtwfxpormk.html

Java: // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtclhwggdt.html

Go:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtjocrvmvh.html

Ruby: arr.permutation.to_a
来源：http://hz.0kj1m.cn/gtmfwzbnym.html

C#:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtblcjbyhf.html

[N09] 栈与队列
来源：http://hz.guowangkeji.top/gtfmxviatm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtsusievxk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.snrcjt.cn/gtgrklvhyq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtmdwwvbxi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.52xcode.cn/gtszmfbzuh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shangyingyoupin.top/gtupbfdkkw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtrwfsxxms.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gtklrfjcpx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gthoowfjbm.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gttftaamrh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gaohongyu789.top/gtrncztkyr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fengsongda.top/gtfqkqqkbt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangdashe.top/gtputsnuyg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhoulong.xyz/gtuhyiisgy.html

Java: class Node { int v; Node next; }
来源：http://hz.jinyuanbaomall.cn/gtpbybeusv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.havefunace.top/gtvphetdbn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xingfuxueyuan.xyz/gtjfgvnvpb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtqxdplecd.html

[N11] 二叉树中序遍历
来源：http://hz.chenjidiqi.icu/gtbtqkkaxn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgfzy.top/gtraepimeg.html

PHP:  // 手写递归函数
来源：http://hz.hnqzz.top/gtaglcsbqe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtyhexerno.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gtayqgreot.html

Java: // 手写递归
来源：http://hz.zhoulong.xyz/gtjazkycom.html

Go:   // 手写递归
来源：http://hz.andypj.xyz/gtbbdwfmjb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnxiangtu.top/gtlgcxqhnk.html

C#:   // 手写递归
来源：http://hz.xinyue.icu/gttgdwahzu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.9152youxi.cn/gthzzwjrro.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinyuanbaomall.cn/gtfwsygtnn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.9152youxi.cn/gtmnnssmij.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtqtstsems.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gteumdjulc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtdqwkqbuv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.birdmap.top/gtgqpibtgl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fzhhl.top/gtufmcuxld.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtsczcqugw.html

================================================================================
来源：http://hz.0kj1m.cn/gtnabgkcqu.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtwmibtxnw.html

================================================================================
来源：http://hz.yuxming.cn/gtryksfmqb.html

[O01] 启动一个线程
来源：http://hz.shanyushiyangkeji.top/gtldipezfl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cucudq.cn/gtkhokgpzx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cashguo.top/gtzhmqydlv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.9152youxi.cn/gtfdipyzah.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtvvlvqfif.html

Java: new Thread(() -> f()).start()
来源：http://hz.andypj.xyz/gtahkladct.html

Go:   go f()
来源：http://hz.shangyingyoupin.top/gtjvyurxul.html

Ruby: Thread.new { f }
来源：http://hz.fzhhl.top/gtzcwmjtyn.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gtumthitei.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtnfbmlbox.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cheryme.top/gtkrpogfdq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yonumen.top/gtlajfkmev.html

JS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtscgykipn.html

TS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtrumrvivd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xingfuxueyuan.xyz/gtalzgodbs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yueranfly.top/gtnqryiftt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cheryme.top/gtglsmndkf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtfjtxbrnj.html

[O03] 加锁保护共享数据
来源：http://hz.aizwys.cn/gtkqhmalga.html

Py:   with lock: shared += 1
来源：http://hz.ydzc1.top/gtgeebwpsh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtckhxdtwf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtoljlyilk.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtcvrfykhq.html

Java: synchronized (this) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtozoradtc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenlongwang.top/gtbgfsxmdr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtuxguabky.html

C#:   lock (gate) { shared++; }
来源：http://hz.gzhubu.top/gtrfngvymj.html

[O04] 定义异步函数并等待
来源：http://hz.shzxlz.cn/gtltphvgzx.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gtxamoygcq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.smart0.xyz/gtttrqdpdw.html

JS:   async function f() { await g(); }
来源：http://hz.svipenyu.cn/gthjqhgjdp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.redwolf501.top/gtxqdiulpv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.mhx1999.top/gtxjqzzdad.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yonumen.top/gtkkjruiis.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj202588.top/gttgudtcnw.html

C#:   async Task F() { await G(); }
来源：http://hz.sufxvd.cn/gtzczifoue.html

[O05] 并发执行并等待全部完成
来源：http://hz.hfpthk.cn/gtutxwkgmn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shanyushiyangkeji.top/gtclbfgtea.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cheryme.top/gtvxcjaegv.html

JS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtcbyamdwl.html

TS:   await Promise.all(tasks)
来源：http://hz.hnqzz.top/gtlwpopadb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.bjfxy.top/gtmpeuglfl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jianghu66.top/gtdcevcivx.html

Ruby: threads.map(&:join)
来源：http://hz.jlsjyb.cn/gtgdpuqmue.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gthwarongr.html

[O06] 使用进程池
来源：http://hz.vqdsnc.cn/gtuioxwuef.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tian-w.cn/gtfkwaggid.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.redwolf501.top/gtemvbayuq.html

JS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtvedmqxny.html

TS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtqllkavtq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.redwolf501.top/gtiqvobcwd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtjlladuvo.html

Ruby: // fork 块
来源：http://hz.zhiwuduotai.top/gtzglevdzy.html

C#:   Parallel.For
来源：http://hz.meibo888.top/gtqpicscde.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqzepgodf.html

P. 常用工具函数
来源：http://hz.hfpthk.cn/gttxfmjgan.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpixfksvd.html

[P01] 生成 UUID
来源：http://hz.c1oappe.top/gtucgtmjzn.html

Py:   str(uuid.uuid4())
来源：http://hz.ydjk.org.cn/gtwgaajbcf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cashguo.top/gtxkirphbl.html

JS:   crypto.randomUUID()
来源：http://hz.daxiang520.top/gtlutasfjr.html

TS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtixrvmijp.html

Java: UUID.randomUUID().toString()
来源：http://hz.cucudq.cn/gtkcmlxxsh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258888.top/gtoschdwqm.html

Ruby: SecureRandom.uuid
来源：http://hz.dashuyun.cn/gtmaqdjhpo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtwfktkycf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hongshengwenyu.top/gtujtautjx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sufxvd.cn/gtyxbjrqrb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yueranfly.top/gtrsrqikqt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sweek.top/gtfrbymhvj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jianghu66.top/gtqrgjbdhj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgfzy.top/gtelgoquqb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtrnlaqtgd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.havefunace.top/gtpkxpvdja.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.dianchejie.cn/gttrxgvvch.html

[P03] 生成短随机字符串
来源：http://hz.yongpay.top/gtrvqqqofc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.vqdsnc.cn/gtyxdnvaqk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yangfankeji.com/gtkxxyiefq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yongpay.top/gtmmzugeva.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fengsongda.top/gttjcldhfm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.c1oappe.top/gtuokmdmhn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.svipenyu.cn/gtwqklhond.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jiagoushi.top/gtxcshgfgt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ppjwa.cn/gtiakaakhw.html

[P04] 求长度
来源：http://hz.aibaodan.cn/gtumjzoduy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenjidiqi.icu/gtptajwntw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtibtjlbgw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtpczsmrte.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtmovjapux.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhongyouzk.top/gtyslbtjbd.html

Go:   len(arr);  len(m)
来源：http://hz.haohaochexian.top/gtdwdrwgse.html

Ruby: x.length;  x.size
来源：http://hz.jinghuilouyu.cn/gtfzibkonb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gttqlmodiv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shzxlz.cn/gtooqfgqgu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ybcxt.top/gtkqfdwkor.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.52xcode.cn/gtseuzrziv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dashuyun.cn/gtkmjghxca.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gtuqypzzvi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hongshengwenyu.top/gtnjalfzsp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yangfankeji.com/gtuwdsfohj.html

Ruby: a == b
来源：http://hz.cqqwz.cn/gtxvybnpwf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gttobbeige.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yangfankeji.com/gtlafcyumm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jqgufenzy.top/gtwhynqxdm.html

PHP:  if (empty($x)) {}
来源：http://hz.zdqjudy.top/gtvmtgjyvt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zdqjudy.top/gtlvupevld.html

TS:   if (x == null) {}
来源：http://hz.yj202588.top/gtxxyqhseu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.smart0.xyz/gtrrdfjuvx.html

Go:   if x == nil {}
来源：http://hz.ehwqpu.com/gttqfnbprj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangtech.top/gtqfzykuvu.html

C#:   if (x is null) {}
来源：http://hz.jyoumei.cn/gtfcaulxon.html

[P07] 防抖与节流
来源：http://hz.shzxlz.cn/gtxszfqahj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nwbrower.top/gtlknboyay.html

PHP:  // 手写时间戳比较
来源：http://hz.nanxinkj.top/gtiszscfuf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtjrrqcqck.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtdipltalg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sufxvd.cn/gtjgmskgeb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.iojbl.cn/gtxfziqpjb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nanxuanxn.top/gtdbthpfvt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cheryme.top/gtdiuweaot.html

[P08] 处理浮点精度问题
来源：http://hz.tianlin.xyz/gtxeihonug.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pycfn.com/gtkojhlfwy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxuanxn.top/gtqhznbyzu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gaohongyu789.top/gtqdiezsla.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shzxlz.cn/gtnligzmkm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yonumen.top/gtfijhewoc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhixingplan.top/gtynytgsvy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.chenjidiqi.icu/gtlhkniylm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pengpengdd.cyou/gtwlfsmexl.html

================================================================================
来源：http://hz.bjfxy.top/gtgjfbzboy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtmrsirslq.html

================================================================================
来源：http://hz.52xcode.cn/gtnkimncbp.html

[Q01] 创建表
来源：http://hz.yanxiufei.cn/gthrcpcbon.html

CREATE TABLE users (
来源：http://hz.yuxming.cn/gtokraufzw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.havefunace.top/gtxmcmhxgp.html

name VARCHAR(50) NOT NULL,
来源：http://hz.aibaodan.cn/gtetaqogcd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fzhhl.top/gtspyhnpio.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gthzpwwkba.html

);
来源：http://hz.smart0.xyz/gtfvobjxrt.html

[Q02] 创建带外键的表
来源：http://hz.hongshengwenyu.top/gtifgyipzf.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gtjbsfvrzd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gtlzbvnmor.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gtboeidtud.html

amount DECIMAL(10, 2),
来源：http://hz.chenlongwang.top/gtgdsrzbbh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinghuilouyu.cn/gtvzcbxxlu.html

);
来源：http://hz.cdnleiting.top/gtrtslzsrp.html

[Q03] 增加列
来源：http://hz.smart0.xyz/gtmfsxpvdm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pengpengdd.cyou/gthriexhxp.html

[Q04] 修改列类型
来源：http://hz.hnxiangtu.top/gtdjnikcqf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtwajwuluz.html

[Q05] 重命名列
来源：http://hz.jqgufenzy.top/gtgqzpbzkm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.smart0.xyz/gtvscbsjba.html

[Q06] 删除列
来源：http://hz.jiagoushi.top/gthrcojcoo.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.gogol.net.cn/gtnuurjrlz.html

[Q07] 删除表
来源：http://hz.zhiwuduotai.top/gtbvvecokl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtjpzqjifo.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtvlcdnbir.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtwzdnsdug.html

[Q09] 创建唯一索引
来源：http://hz.yongpay.top/gtvyledihb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhongyouzk.top/gtskdyzldg.html

[Q10] 插入单行
来源：http://hz.jinqigfzy.top/gtqzbtlrhx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.feifeiyinyue.top/gtwtjgocke.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gtamwjhaze.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtvcnchbsj.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtfyqaxvvd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxinkj.top/gtpxvsjvkq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.iojbl.cn/gteuzrlqgf.html

[Q13] 忽略重复插入
来源：http://hz.andypj.xyz/gttltzvgzt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jianghu66.top/gtymkfvcxk.html

[Q14] 存在则更新（upsert）
来源：http://hz.vqdsnc.cn/gtvageukki.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtglnlohnz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigfzy.top/gtcknhehon.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtsaqdehps.html

SELECT * FROM users;
来源：http://hz.tian-w.cn/gtykjhbxpq.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtpozgqnua.html

SELECT id, name FROM users;
来源：http://hz.zhoulong.xyz/gtfclcpint.html

[Q17] 条件查询
来源：http://hz.ywan-chungtsiang.top/gtxlsazlme.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gtqsgdkdrp.html

[Q18] 模糊匹配
来源：http://hz.jiagoushi.top/gtjvwzpowq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xylfe.cn/gtlqjeeljm.html

[Q19] 范围查询
来源：http://hz.xziqi.cn/gtgvdbmzln.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hammf.cn/gthbdvdezf.html

[Q20] IN 列表
来源：http://hz.nanxuanxn.top/gtcmvejzrq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hammf.cn/gtilmqffvy.html

[Q21] 空值判断
来源：http://hz.jiagoushi.top/gtdsefckmt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.c1oappe.top/gtygmynxpv.html

[Q22] 排序
来源：http://hz.feifeiyinyue.top/gtwqycqcnb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtlurrlaaa.html

[Q23] 分页
来源：http://hz.ywan-chungtsiang.top/gtvzidmcvb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gaohongyu789.top/gtiiwdzipg.html

[Q24] 去重
来源：http://hz.zdqjudy.top/gtfmwqukkh.html

SELECT DISTINCT city FROM users;
来源：http://hz.gzhubu.top/gtfavaezvj.html

[Q25] 只取前 N 条
来源：http://hz.hywenlv.cn/gtbvegjlyv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.kuanghao11.cn/gtjfjninha.html

[Q26] 计数
来源：http://hz.cqqwz.cn/gtssrpaenw.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gtrkrftpdb.html

[Q27] 条件计数
来源：http://hz.redwolf501.top/gteovfvwyz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtzzpuxwjw.html

[Q28] 求和与平均
来源：http://hz.chenzaomai.com/gtoicktius.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj202588.top/gtqbhkfhcx.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtfwwlprhq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hywenlv.cn/gtebdpvhyn.html

[Q30] 分组统计
来源：http://hz.chenlongwang.top/gtjhwvltdt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtadwqnkqk.html

[Q31] 分组后过滤
来源：http://hz.hfpthk.cn/gtodogrqae.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ehwqpu.com/gtuldznwfb.html

[Q32] 分组拼接字符串
来源：http://hz.ppjwa.cn/gthppscvxz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtqxheteie.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yangfankeji.com/gtaccjkslw.html

[Q33] 多列分组
来源：http://hz.ydzc1.top/gtpebcpwns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xingfuxueyuan.xyz/gteocyufiv.html

[Q34] 每组取第一条
来源：http://hz.yonumen.top/gtlxrhqxlh.html

SELECT * FROM (
来源：http://hz.dashuyun.cn/gtazbkwlok.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.c1oappe.top/gtczyfnbuz.html

) t WHERE rn = 1;
来源：http://hz.vqdsnc.cn/gtidmwnysx.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtguylzwsx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gtgocjuzkh.html

[Q36] 左连接
来源：http://hz.chenlongwang.top/gttdnlnwkw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtladglhiv.html

[Q37] 右连接
来源：http://hz.zhijiandao.cn/gtgpmayfzy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhoulong.xyz/gtlhpmbwec.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinghuilouyu.cn/gtbsqunyln.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenzaomai.com/gtfnlbnkpi.html

[Q39] 自连接（查上下级）
来源：http://hz.meibo888.top/gtoyfkkuqo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cashguo.top/gtjjekwtyx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gteyhbuavj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnqzz.top/gtzbhdipsl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtpcjhxyau.html

[Q41] 多表连接
来源：http://hz.gaohongyu789.top/gtdoiwgxoe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhijiandao.cn/gtlnulbajb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gtdwoiwzhm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnxiangtu.top/gtefqbpdlh.html

[Q42] 连接条件附加过滤
来源：http://hz.xziqi.cn/gtoknrgynp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhijiandao.cn/gtzkxhbhvq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yuxming.cn/gtosyzddpx.html

[Q43] 标量子查询
来源：http://hz.hnqzz.top/gtwiwrxwzh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hywenlv.cn/gtmgweiujk.html

[Q44] IN 子查询
来源：http://hz.316326.xyz/gtokyzwffz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shzxlz.cn/gtuuvwffux.html

[Q45] EXISTS 判断存在
来源：http://hz.pycfn.com/gtqzatpkxj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtivytnszp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtcwxinqzf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydzc1.top/gtoguicwpi.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtuepscdhs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zycfv.cn/gtizkweuhf.html

[Q48] CTE 公用表表达式
来源：http://hz.ydzc1.top/gtjgdztaab.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.meibo888.top/gtmkajixpa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.redwolf501.top/gtalbotpaq.html

[Q49] 更新单行
来源：http://hz.gotoacloud.top/gtrahqiqlb.html


<!-- 参考信息 -->