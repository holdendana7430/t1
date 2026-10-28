代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.sysykeji.top/gtjbdtoxjc.html

PHP:  // 手写递归交换
来源：http://hz.redwolf501.top/gthpvgvbyb.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtebwcsqxk.html

TS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtzeuindrl.html

Java: // 手写回溯递归
来源：http://hz.yj20258888.top/gtrpiiphaj.html

Go:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtxfukdglh.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gthzuxfpdb.html

C#:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtcrknfmmh.html

[N09] 栈与队列
来源：http://hz.zhijiandao.cn/gtalkueixy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ywan-chungtsiang.top/gtrimydrnq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yueranfly.top/gtyajmilsh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtkapgftcp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258888.top/gtxalsqpka.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnxiangtu.top/gtesrkadqb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.quarkkingdee.top/gtfcqltjlb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.c1oappe.top/gtaaryavll.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhongyouzk.top/gtraiqnfqp.html

[N10] 链表节点定义
来源：http://hz.zhixingplan.top/gtvbzimgla.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jiagoushi.top/gtrkkckugu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.feifeiyinyue.top/gtcfzwirqc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gtvhfingzm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gttlkewqgj.html

Java: class Node { int v; Node next; }
来源：http://hz.yangfankeji.com/gtlffxevhl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ybcxt.top/gtrsnlgnhh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daxiang520.top/gtpainkdzr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hammf.cn/gtvpeqgtjd.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtkrsehsik.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.316326.xyz/gtwhynarpr.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtjytifuxr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtsldqygaj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cqqwz.cn/gtnmcwnqla.html

Java: // 手写递归
来源：http://hz.52xcode.cn/gtpcrweyvz.html

Go:   // 手写递归
来源：http://hz.chenjidiqi.icu/gtjmpqnoxl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtfafdkwkj.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtjaviamrk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhaomingkeji.xyz/gtcmtjwgvg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shzxlz.cn/gtwccoolqe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydjk.org.cn/gtxytpilpb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtutnynzga.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xziqi.cn/gtfkjckfql.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zdqjudy.top/gtaqgtdfrh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hysaishi.cn/gtgvazoieb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gtwzpouprd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtwjhybprj.html

================================================================================
来源：http://hz.gotoacloud.top/gtbjzftygk.html

O. 并发与异步
来源：http://hz.xuanzx.com/gtdkupbugp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxgzdozkx.html

[O01] 启动一个线程
来源：http://hz.xingfuxueyuan.xyz/gtzmmrlclz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ywan-chungtsiang.top/gtltghzmfw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinyuanbaomall.cn/gtmwpxljwz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtamfylfnk.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gtbhoxbsym.html

Java: new Thread(() -> f()).start()
来源：http://hz.9152youxi.cn/gtmyoabeye.html

Go:   go f()
来源：http://hz.wangdashe.top/gtaqfnccvn.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtfexiuplx.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gtynqdueyr.html

[O02] 使用线程池
来源：http://hz.smart0.xyz/gtdoehlgid.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daria6918.cn/gtdwosomap.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shuidangran.top/gtfexxwwds.html

JS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gthhzoefoq.html

TS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtmxcszeiq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gtsfaxzvwu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnqzz.top/gtsoxzfgcr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.sxryk.cn/gtqnmxjdwj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jqgufenzy.top/gtgumqlogx.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtdcwhbcll.html

Py:   with lock: shared += 1
来源：http://hz.yuxming.cn/gttxgbwlii.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtxattezlz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtkrywxmvr.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtyztadrfs.html

Java: synchronized (this) { shared++; }
来源：http://hz.hfpthk.cn/gtozcthvvt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtnrzmkriv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daxiang520.top/gtjiauzzwb.html

C#:   lock (gate) { shared++; }
来源：http://hz.tian-w.cn/gtpnfnglxj.html

[O04] 定义异步函数并等待
来源：http://hz.svipenyu.cn/gtfxfarqun.html

Py:   async def f():⏎    await g()
来源：http://hz.fzhhl.top/gtngwhsdlf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jlsjyb.cn/gtkpqvavrc.html

JS:   async function f() { await g(); }
来源：http://hz.yvedp.cn/gtbdbryvqa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jianghu66.top/gtvrwihbun.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.quarkkingdee.top/gtexemougd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aibaodan.cn/gtbljuloyl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guowangkeji.top/gtwzqpmvfq.html

C#:   async Task F() { await G(); }
来源：http://hz.chenzaomai.com/gtpyyepnki.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuanzhike.top/gtjyaispjv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.wangshuangyany.cn/gtmhudepfa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yanxiufei.cn/gtuespfupe.html

JS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gttuhtxaky.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtqhyljitc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jqgufenzy.top/gtdwuahwgg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtphuumtei.html

Ruby: threads.map(&:join)
来源：http://hz.bjfxy.top/gtqzsgjtvs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shangyingyoupin.top/gtijppuyvy.html

[O06] 使用进程池
来源：http://hz.bjfxy.top/gtdembgiqo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.aizwys.cn/gtgjkaoqvn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigfzy.top/gtjmvjckvw.html

JS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtjrzuzubk.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtiyjowvjy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yuxming.cn/gtebzrnwgu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxinkj.top/gtotpcuvmr.html

Ruby: // fork 块
来源：http://hz.zhaomingkeji.xyz/gtadynztwk.html

C#:   Parallel.For
来源：http://hz.gaohongyu789.top/gttmdmaxgg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtegundifb.html

P. 常用工具函数
来源：http://hz.ehwqpu.com/gtqukliaaj.html

================================================================================
来源：http://hz.mhx1999.top/gtisgpxjkw.html

[P01] 生成 UUID
来源：http://hz.ydjk.org.cn/gtrpsejalw.html

Py:   str(uuid.uuid4())
来源：http://hz.dianchejie.cn/gtdfsedwez.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenzaomai.com/gtfdpcxzrf.html

JS:   crypto.randomUUID()
来源：http://hz.zhixingplan.top/gtckurpjwd.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtuqujztsz.html

Java: UUID.randomUUID().toString()
来源：http://hz.chenlongwang.top/gtiydsxcio.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gttuzqqdxd.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gtqitnntkb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtbmjnadcv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hongshengwenyu.top/gtmckjurpg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhixingplan.top/gthcdslaaa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangshuangyany.cn/gtpdapnxgl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shangyingyoupin.top/gtjfovlqez.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhixingplan.top/gtgkpuitik.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ybcxt.top/gtofqwglnr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gtykhliwzg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtdlmqjwvc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtelnuflkp.html

[P03] 生成短随机字符串
来源：http://hz.wangshuangyany.cn/gtrdxbwpys.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.birdmap.top/gtisvvutul.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ydjk.org.cn/gtyrprtzbk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guowangkeji.top/gtscqoalax.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtynfrtsen.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtvmzfrzpd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hywenlv.cn/gtfbwyiuud.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgfzy.top/gtakunhhgo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gogol.net.cn/gtudrybozr.html

[P04] 求长度
来源：http://hz.snrcjt.cn/gtxdbiyvsv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.iojbl.cn/gtddftpfze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtprwyohrh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtktfomofy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinyuanbaomall.cn/gtcqyriect.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hfpthk.cn/gtlrgmixsk.html

Go:   len(arr);  len(m)
来源：http://hz.cdnleiting.top/gtiukmuwie.html

Ruby: x.length;  x.size
来源：http://hz.yvedp.cn/gtalzgzvll.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtaawvdlmy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gzhubu.top/gtdqpraxwc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xziqi.cn/gtkfbwtvis.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hywenlv.cn/gtwvnxpmiq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtnmfbpexf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtcumuwbsc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258888.top/gtkmjgulsw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigufen.top/gtlgxiyhum.html

Ruby: a == b
来源：http://hz.yvedp.cn/gtlrbmfpls.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.andypj.xyz/gtojptuxxk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangdashe.top/gtjnriosrv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhoulong.xyz/gtaezqxuku.html

PHP:  if (empty($x)) {}
来源：http://hz.dianchejie.cn/gtkprcmsax.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.andypj.xyz/gtblfwjpsa.html

TS:   if (x == null) {}
来源：http://hz.guannengcc.top/gtvogzyjxi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hongshengwenyu.top/gtarhlyzui.html

Go:   if x == nil {}
来源：http://hz.c1oappe.top/gtldwdexgq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.smart0.xyz/gtfwpizfjd.html

C#:   if (x is null) {}
来源：http://hz.ywan-chungtsiang.top/gtqepibvgk.html

[P07] 防抖与节流
来源：http://hz.meibo888.top/gtxwxjkglg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ppjwa.cn/gtfsxranfu.html

PHP:  // 手写时间戳比较
来源：http://hz.52xcode.cn/gtmuiugkdy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtmaykmlgd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtyojyumyf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jiagoushi.top/gtcccfgkcx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhijiandao.cn/gtrpiotfvu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ydjk.org.cn/gtuenyoyyn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtaaktazky.html

[P08] 处理浮点精度问题
来源：http://hz.nanxuanxn.top/gtsllrczur.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuanzhike.top/gtnuwwbqfp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hywenlv.cn/gtnoahmpys.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnqzz.top/gtctmuhkzq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xingfuxueyuan.xyz/gtogvnnoyl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nwbrower.top/gtgektffvz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhaomingkeji.xyz/gtazcafiiq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yvedp.cn/gtayehmsfd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ybcxt.top/gtqcnxewmp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtipeadcxi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gthvwjruam.html

================================================================================
来源：http://hz.daxiang520.top/gtsoapdtnr.html

[Q01] 创建表
来源：http://hz.ehwqpu.com/gtvdfpezax.html

CREATE TABLE users (
来源：http://hz.jqgufenzy.top/gttwypjrxv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydzc1.top/gtlgswrlnq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.andypj.xyz/gtximitaot.html

email VARCHAR(100) UNIQUE,
来源：http://hz.andypj.xyz/gtejpakapi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.gaohongyu789.top/gtmpppkpgx.html

);
来源：http://hz.fzhhl.top/gtpegbhvhe.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gtqsiszizu.html

CREATE TABLE orders (
来源：http://hz.fengsongda.top/gtrpqzpcnt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtawgulvfs.html

user_id INT NOT NULL,
来源：http://hz.havefunace.top/gtlcoiuykf.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258.top/gtmiwrkdiu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.tanke756.top/gtwqijwkge.html

);
来源：http://hz.tianlin.xyz/gtzwqipemu.html

[Q03] 增加列
来源：http://hz.ybcxt.top/gtrubdqucx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nwbrower.top/gtzwlcdqrl.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtrselqqdh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.svipenyu.cn/gtjeuphssf.html

[Q05] 重命名列
来源：http://hz.hongshengwenyu.top/gtiziucgee.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sysykeji.top/gtswdhrvdn.html

[Q06] 删除列
来源：http://hz.yj20258888.top/gtpggqpssk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.andypj.xyz/gtkqjwtbqy.html

[Q07] 删除表
来源：http://hz.zhoulong.xyz/gtbiviwubf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtlauynkqs.html

[Q08] 创建普通索引
来源：http://hz.sweek.top/gtensvhhxp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtbynqkibn.html

[Q09] 创建唯一索引
来源：http://hz.cdnleiting.top/gtvbdvrnpv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xylfe.cn/gtkussqjrl.html

[Q10] 插入单行
来源：http://hz.c1oappe.top/gtiuwjstyy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sxryk.cn/gtnqdlwhfn.html

[Q11] 一次插入多行
来源：http://hz.iojbl.cn/gtmfjnpedb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenlongwang.top/gtnwpasvab.html

[Q12] 插入后取自增 ID
来源：http://hz.ivvv.top/gtiprtwpim.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nwbrower.top/gtalyadous.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtgswxchcg.html

[Q13] 忽略重复插入
来源：http://hz.fengsongda.top/gtsweirbuk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gtpbwzitep.html

[Q14] 存在则更新（upsert）
来源：http://hz.dashuyun.cn/gthxqmtlvd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.snrcjt.cn/gtwsctsdrd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj20258888.top/gtbtapnojg.html

[Q15] 查询全部
来源：http://hz.dianchejie.cn/gtdhuycyoc.html

SELECT * FROM users;
来源：http://hz.ydzc1.top/gticvvurvm.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtsvsqzjcb.html

SELECT id, name FROM users;
来源：http://hz.cqqwz.cn/gtynllsuty.html

[Q17] 条件查询
来源：http://hz.ydzc1.top/gtfvzktnxp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yueranfly.top/gtzitphilf.html

[Q18] 模糊匹配
来源：http://hz.cucudq.cn/gtacxgymmm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.birdmap.top/gtudysxpml.html

[Q19] 范围查询
来源：http://hz.yuxming.cn/gtpaukofhf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yueranfly.top/gtxechlyzh.html

[Q20] IN 列表
来源：http://hz.cheryme.top/gtesqpyjac.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hysaishi.cn/gtauzfseuz.html

[Q21] 空值判断
来源：http://hz.jinyuanbaomall.cn/gtdxtmxvcu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tianlin.xyz/gtcoqwhjes.html

[Q22] 排序
来源：http://hz.guowangkeji.top/gtiblrfaks.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gzhubu.top/gtdxkmimsy.html

[Q23] 分页
来源：http://hz.52xcode.cn/gtydntsady.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daria6918.cn/gtudziegkj.html

[Q24] 去重
来源：http://hz.yongpay.top/gttkppwhcg.html

SELECT DISTINCT city FROM users;
来源：http://hz.gaohongyu789.top/gtxnfqsmlp.html

[Q25] 只取前 N 条
来源：http://hz.hnxiangtu.top/gtlumsujdj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.smart0.xyz/gttrnrxmvj.html

[Q26] 计数
来源：http://hz.9152youxi.cn/gtnkfimnjt.html

SELECT COUNT(*) FROM users;
来源：http://hz.jyoumei.cn/gtfnxpddtq.html

[Q27] 条件计数
来源：http://hz.xylfe.cn/gtlppqbfuc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.birdmap.top/gtbjjoepzn.html

[Q28] 求和与平均
来源：http://hz.tianlin.xyz/gtbbdjqjez.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxinkj.top/gtopdnfegw.html

[Q29] 最大最小值
来源：http://hz.tian-w.cn/gtqmijccqv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtmluefabh.html

[Q30] 分组统计
来源：http://hz.havefunace.top/gtyfoxiegb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtbbtsifam.html

[Q31] 分组后过滤
来源：http://hz.quarkkingdee.top/gtorfqqoow.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jyoumei.cn/gtofkoddgq.html

[Q32] 分组拼接字符串
来源：http://hz.hywenlv.cn/gtmtsndoip.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtdkwpsbkt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.guowangkeji.top/gtueutftzm.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtfolpfjsj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yanxiufei.cn/gtbxiyxelg.html

[Q34] 每组取第一条
来源：http://hz.xziqi.cn/gtexlabhjl.html

SELECT * FROM (
来源：http://hz.zdqjudy.top/gtcudoelua.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tian-w.cn/gtrnklsdwo.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangtech.top/gtjwioaaih.html

[Q35] 内连接
来源：http://hz.havefunace.top/gtudwqqssu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtamgfzbsb.html

[Q36] 左连接
来源：http://hz.guannengcc.top/gtbbfjycva.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtnnfcmdje.html

[Q37] 右连接
来源：http://hz.xinyue.icu/gtgjwrcnst.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.9152youxi.cn/gtepzifuiz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hfpthk.cn/gtrtovewcu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.birdmap.top/gtjzrdzaig.html

[Q39] 自连接（查上下级）
来源：http://hz.sxryk.cn/gttgxfxbft.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gttxtxbflb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtiaphwzww.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtvlwqgmwj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cashguo.top/gthkyrutdr.html

[Q41] 多表连接
来源：http://hz.xylfe.cn/gtccnqtuyw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ivvv.top/gtvutstbne.html

JOIN users u ON u.id = o.user_id
来源：http://hz.9152youxi.cn/gteyqkzaaf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gttmiptmcx.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258888.top/gtfthdpkng.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgufenzy.top/gtcfvnenjz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.316326.xyz/gtonyesosb.html

[Q43] 标量子查询
来源：http://hz.ehwqpu.com/gtwjdbuboq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ywan-chungtsiang.top/gtxlakypfx.html

[Q44] IN 子查询
来源：http://hz.havefunace.top/gtrmewzyqn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yueranfly.top/gtywvuiamx.html

[Q45] EXISTS 判断存在
来源：http://hz.sweek.top/gteqnkgkqb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtltwpribt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xziqi.cn/gtzwxcnjts.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtgdlhvcmj.html

[Q47] 与平均值比较
来源：http://hz.andypj.xyz/gtkwndpwnh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtwresyjsy.html

[Q48] CTE 公用表表达式
来源：http://hz.tianlin.xyz/gtcmrzfrdl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gturxmueej.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinghuilouyu.cn/gtxyfgzzao.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtkjrcfskt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zdqjudy.top/gturmlcidd.html

[Q50] 批量更新
来源：http://hz.jinghuilouyu.cn/gtpeeumfio.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zdqjudy.top/gtlnnoogvo.html

[Q51] 用子查询更新
来源：http://hz.gogol.net.cn/gtvalezlkg.html


<!-- 参考信息 -->