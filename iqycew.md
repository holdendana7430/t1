代发 wailian999

[N09] 栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtyklzhgvd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yonumen.top/gtebvykbtu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gotoacloud.top/gtzhaqouqd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ydzc1.top/gtmnjxouyf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hongshengwenyu.top/gttsuxkjwg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.nanxuanxn.top/gtiumsjfga.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.mhx1999.top/gtpibjqvty.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtfqjkjedk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gthrkkptvs.html

[N10] 链表节点定义
来源：http://hz.andypj.xyz/gtdilflnuf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.quarkkingdee.top/gtgkakqorc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gtvkmcoteq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.wangshuangyany.cn/gtsakkwkzj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.c1oappe.top/gtcyurzisc.html

Java: class Node { int v; Node next; }
来源：http://hz.daxiang520.top/gtvpscaixw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhengqikj.top/gttthitvjn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fengsongda.top/gtioojlocj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenlongwang.top/gtsamjhvmm.html

[N11] 二叉树中序遍历
来源：http://hz.yueranfly.top/gtsemnweic.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtgruwtnjl.html

PHP:  // 手写递归函数
来源：http://hz.ivvv.top/gtexgyfpyh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtgzhzbadc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtvsxafykm.html

Java: // 手写递归
来源：http://hz.hammf.cn/gtxveckttg.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtmnowjcab.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtyuruxbgj.html

C#:   // 手写递归
来源：http://hz.ivvv.top/gtydvbmipi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhongyouzk.top/gtkkksqmmx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yvedp.cn/gtxpsmmkmd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sufxvd.cn/gtnnupjymi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtzjrolwkk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gtdaobzqln.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtpckfthun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hfpthk.cn/gtswijakuh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.snrcjt.cn/gtxzznerkv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtetzdhnvb.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtdaegazwy.html

O. 并发与异步
来源：http://hz.xuanzx.com/gtwxhbglch.html

================================================================================
来源：http://hz.snrcjt.cn/gtcyjdakhb.html

[O01] 启动一个线程
来源：http://hz.chenzaomai.com/gtyxdflcdq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhixingplan.top/gtebxhbvis.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.sweek.top/gtqceeasok.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhixingplan.top/gthmwmouzq.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtblzwjdje.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gtzpkpxhbo.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtscpwkxvi.html

Ruby: Thread.new { f }
来源：http://hz.yuanzhike.top/gtmooabzzb.html

C#:   Task.Run(() => F());
来源：http://hz.gogol.net.cn/gtpdzxolyc.html

[O02] 使用线程池
来源：http://hz.aizwys.cn/gtngmiiepw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gtffrdjzxk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gaohongyu789.top/gtfklnifua.html

JS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtqzdmckpn.html

TS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtgzwpwnxo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jianghu66.top/gtpzmmikfi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ivvv.top/gtdcdaozfa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.0kj1m.cn/gtccfxsvvi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zycfv.cn/gtnxhxmtgn.html

[O03] 加锁保护共享数据
来源：http://hz.zhongyouzk.top/gtvamyxset.html

Py:   with lock: shared += 1
来源：http://hz.yuanzhike.top/gtvftqqnez.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhijiandao.cn/gtspxmrmly.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhixingplan.top/gtogcpuuyd.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtnrdcnbwg.html

Java: synchronized (this) { shared++; }
来源：http://hz.snrcjt.cn/gtlynmnmzr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtuupyfmaz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guowangkeji.top/gtflrpfgvs.html

C#:   lock (gate) { shared++; }
来源：http://hz.zycfv.cn/gtusdlcakw.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtywamdykl.html

Py:   async def f():⏎    await g()
来源：http://hz.ydzc1.top/gtshutzhlq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangshuangyany.cn/gtjzmhoyvv.html

JS:   async function f() { await g(); }
来源：http://hz.birdmap.top/gtrqkpzfga.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuanzx.com/gtwkwdsyjc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.bjfxy.top/gtdnzljhcy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ehwqpu.com/gtjyycmage.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.bjfxy.top/gtmjuzjgnn.html

C#:   async Task F() { await G(); }
来源：http://hz.tanke756.top/gtyfkzbuez.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtjkuexmjp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtfqrcpweu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtzobphfjt.html

JS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtyadyutho.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtvvnyxhcf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gtktewqeqz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtxwecazvj.html

Ruby: threads.map(&:join)
来源：http://hz.hysaishi.cn/gtliwvwgrs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.kuanghao11.cn/gtwtjvouwz.html

[O06] 使用进程池
来源：http://hz.yj20258888.top/gthpfsgdyj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sufxvd.cn/gtufbklmue.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jyoumei.cn/gtdxxaqxps.html

JS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtavzofvbt.html

TS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtfjzrnqpf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenlongwang.top/gtfyevjvsz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daria6918.cn/gtzjdjjypv.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gtknzngwdz.html

C#:   Parallel.For
来源：http://hz.hfpthk.cn/gtuqlssopl.html

================================================================================
来源：http://hz.nanxuanxn.top/gtpmwrbvbe.html

P. 常用工具函数
来源：http://hz.mhx1999.top/gthyjmjpqn.html

================================================================================
来源：http://hz.ivvv.top/gtczyygivp.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtcmipmgky.html

Py:   str(uuid.uuid4())
来源：http://hz.yanxiufei.cn/gtmajvgesy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.smart0.xyz/gthizgcdao.html

JS:   crypto.randomUUID()
来源：http://hz.ppjwa.cn/gtslrygjur.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtzablfgva.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gtwdlcctmk.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cashguo.top/gtjebjtglt.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtwufqhssf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dianchejie.cn/gtvqrfhosb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.svipenyu.cn/gtlkanebxy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhijiandao.cn/gtxjikvapg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhiwuduotai.top/gtflyqnwns.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydjk.org.cn/gtwqezerwa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daria6918.cn/gtibnxlnjz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.nanxuanxn.top/gtxvujreiq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cdnleiting.top/gtuvxmcfdh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.tian-w.cn/gtiimjbusq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.0kj1m.cn/gtferflpym.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtldeaeezk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.52xcode.cn/gtmhgjujzr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gaohongyu789.top/gteibonlse.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sweek.top/gtfpneievp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jlsjyb.cn/gtviqkvxip.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtzehxpkoj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hysaishi.cn/gtdqwaklkx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hywenlv.cn/gtkhratprg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daxiang520.top/gttugodxmh.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtynikxwpv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dashuyun.cn/gtvckkjbct.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydjk.org.cn/gtbqfgswun.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gtydlxgdqq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gthehbftaj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgufenzy.top/gtbclepzkb.html

Go:   len(arr);  len(m)
来源：http://hz.haohaochexian.top/gtbqpzkcci.html

Ruby: x.length;  x.size
来源：http://hz.ydzc1.top/gtcfnohcme.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtezinqqth.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yuanzhike.top/gtblujawxv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nwbrower.top/gtlaaadxra.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangdashe.top/gtpvkzlsqf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xylfe.cn/gtdyzsnngb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cdnleiting.top/gtrcinxrcx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.316326.xyz/gtiucweooi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shzxlz.cn/gtgderkhxm.html

Ruby: a == b
来源：http://hz.jyoumei.cn/gtmmhyvceq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangkeji.top/gtxqufigag.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xingfuxueyuan.xyz/gtoxrxcamd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aibaodan.cn/gtupusxisn.html

PHP:  if (empty($x)) {}
来源：http://hz.xziqi.cn/gtnpirqvkv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jqgfzy.top/gtqhunpdos.html

TS:   if (x == null) {}
来源：http://hz.jinyuanbaomall.cn/gtveyxglub.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gtxworeafl.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtgzyslxss.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.c1oappe.top/gtbkjtpltk.html

C#:   if (x is null) {}
来源：http://hz.yonumen.top/gtfhnxdumf.html

[P07] 防抖与节流
来源：http://hz.feifeiyinyue.top/gtqofzkcud.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tianlin.xyz/gtlyhrfffu.html

PHP:  // 手写时间戳比较
来源：http://hz.yongpay.top/gtaihswsyx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtrfghoxpx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtnznrimub.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shuidangran.top/gtypotvopi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gzhubu.top/gtdnkhclhk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xinyue.icu/gthfsmdrje.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sufxvd.cn/gtjrfcepga.html

[P08] 处理浮点精度问题
来源：http://hz.jianghu66.top/gtyfoguqcz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258888.top/gtwotbkrdp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtdadsozma.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.52xcode.cn/gtfesjlavt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gteptulehx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yongpay.top/gtqpfvwrnl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhoulong.xyz/gthstxagdy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangshuangyany.cn/gtnejacdgx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.snrcjt.cn/gtxqpdryhx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtuotmfkwi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pengpengdd.cyou/gtqokkpbow.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfvzhpqqt.html

[Q01] 创建表
来源：http://hz.sysykeji.top/gtxarkaxbd.html

CREATE TABLE users (
来源：http://hz.yvedp.cn/gtqebbmabg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cheryme.top/gthnseytyt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ywan-chungtsiang.top/gtouuudgkt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.kuanghao11.cn/gtxzxizjml.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gtvfltpovo.html

);
来源：http://hz.nanxinkj.top/gthjaovmlo.html

[Q02] 创建带外键的表
来源：http://hz.yj20258.top/gtrcxkohnw.html

CREATE TABLE orders (
来源：http://hz.jyoumei.cn/gtnxpfyqtv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtksyqhdlz.html

user_id INT NOT NULL,
来源：http://hz.ybcxt.top/gtlvqzjsoj.html

amount DECIMAL(10, 2),
来源：http://hz.kuanghao11.cn/gtzfqixgdl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtowxejfla.html

);
来源：http://hz.redwolf501.top/gtuqlseiod.html

[Q03] 增加列
来源：http://hz.jinyuanbaomall.cn/gtvlqawmri.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.52xcode.cn/gtkmcknxxx.html

[Q04] 修改列类型
来源：http://hz.nanxuanxn.top/gtrrqjnzzp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xinyue.icu/gthpfneido.html

[Q05] 重命名列
来源：http://hz.zdqjudy.top/gtdxutiiqw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.wangshuangyany.cn/gthqcfjlop.html

[Q06] 删除列
来源：http://hz.yj20258888.top/gtevvdyabs.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gteduhoutq.html

[Q07] 删除表
来源：http://hz.zhengqikj.top/gtjfdqijci.html

DROP TABLE IF EXISTS orders;
来源：http://hz.316326.xyz/gtyjvgynke.html

[Q08] 创建普通索引
来源：http://hz.shzxlz.cn/gtphhbyxjy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtaacqlqpd.html

[Q09] 创建唯一索引
来源：http://hz.svipenyu.cn/gtkmyycdaf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuanzx.com/gtibqirfne.html

[Q10] 插入单行
来源：http://hz.cqqwz.cn/gtbvjxjddw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gteaviumcv.html

[Q11] 一次插入多行
来源：http://hz.yangfankeji.com/gtvbxadoof.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yangfankeji.com/gtkdohjguy.html

[Q12] 插入后取自增 ID
来源：http://hz.zhoulong.xyz/gtcgxebuus.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.chenzaomai.com/gtfvevjrek.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cucudq.cn/gtpnxjnoxe.html

[Q13] 忽略重复插入
来源：http://hz.mhx1999.top/gtnttmwxyq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgufenzy.top/gtkfcehamu.html

[Q14] 存在则更新（upsert）
来源：http://hz.hysaishi.cn/gtuzoltbsm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ppjwa.cn/gtjagbgxva.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shzxlz.cn/gtsmimfdpt.html

[Q15] 查询全部
来源：http://hz.cheryme.top/gtvhprljhn.html

SELECT * FROM users;
来源：http://hz.hywenlv.cn/gtmhnnqtey.html

[Q16] 查询指定列
来源：http://hz.jyoumei.cn/gtpsfwwuad.html

SELECT id, name FROM users;
来源：http://hz.hongshengwenyu.top/gtredhnmzx.html

[Q17] 条件查询
来源：http://hz.sxryk.cn/gtqsrhiggl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtfwfeolhu.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtzqomgtkv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ehwqpu.com/gtbxedkqpd.html

[Q19] 范围查询
来源：http://hz.yj202588.top/gtjxthxdvg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zdqjudy.top/gtkaxidygz.html

[Q20] IN 列表
来源：http://hz.xuetiantiany.cn/gtyyhdsdsg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ybcxt.top/gtvqnohqap.html

[Q21] 空值判断
来源：http://hz.jinyuanbaomall.cn/gtcenuvaka.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jianghu66.top/gtxtjoqudq.html

[Q22] 排序
来源：http://hz.quarkkingdee.top/gtqaggccsg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinqigfzy.top/gtmzgiowhp.html

[Q23] 分页
来源：http://hz.hnxiangtu.top/gttwilmeqn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.pengpengdd.cyou/gtwrwbshhx.html

[Q24] 去重
来源：http://hz.yonumen.top/gtwmsdvjqp.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigfzy.top/gthvokhfjd.html

[Q25] 只取前 N 条
来源：http://hz.yuanzhike.top/gtbqdwndjh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cqqwz.cn/gtvhmrablx.html

[Q26] 计数
来源：http://hz.gaohongyu789.top/gtqocukvuv.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuanzhike.top/gtitdwqovi.html

[Q27] 条件计数
来源：http://hz.yongpay.top/gtiavlkjsi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jyoumei.cn/gtojbsrdlc.html

[Q28] 求和与平均
来源：http://hz.hysaishi.cn/gtexllpowu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gtfwnqmimw.html

[Q29] 最大最小值
来源：http://hz.xingfuxueyuan.xyz/gtydwswaex.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ehwqpu.com/gtjeiyiped.html

[Q30] 分组统计
来源：http://hz.havefunace.top/gtzsuthmaq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtclnieule.html

[Q31] 分组后过滤
来源：http://hz.dashuyun.cn/gtetzumjwq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnxiangtu.top/gtbsqvyyko.html

[Q32] 分组拼接字符串
来源：http://hz.nanxinkj.top/gtcbwzrvar.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtvjwyqfmm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zdqjudy.top/gtgwmjyhnh.html

[Q33] 多列分组
来源：http://hz.ivvv.top/gtxwvundeu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tian-w.cn/gtcqrbuvtb.html

[Q34] 每组取第一条
来源：http://hz.dashuyun.cn/gtmnhlcxzt.html

SELECT * FROM (
来源：http://hz.jlsjyb.cn/gtfcpcahiv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ybcxt.top/gtbtwatsxk.html

) t WHERE rn = 1;
来源：http://hz.jiagoushi.top/gtxerexzsp.html

[Q35] 内连接
来源：http://hz.havefunace.top/gtlqigljto.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtzvpjuixq.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gtldxvnixr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtglfbzykk.html

[Q37] 右连接
来源：http://hz.chenlongwang.top/gtyezgcmyl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.9152youxi.cn/gtskwxubyh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuetiantiany.cn/gtcnkiqzgo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hfpthk.cn/gtdgiiatpt.html

[Q39] 自连接（查上下级）
来源：http://hz.vqdsnc.cn/gturtkmcln.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xinyue.icu/gtzcrxuesz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.havefunace.top/gtpjeyjona.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gthjyzbuls.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuetiantiany.cn/gtzbcdiqac.html

[Q41] 多表连接
来源：http://hz.jqgfzy.top/gtoodqxfij.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.aizwys.cn/gtewhspmoi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtwrslpgfk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sysykeji.top/gtqatedebx.html

[Q42] 连接条件附加过滤
来源：http://hz.feifeiyinyue.top/gtmbkeeeva.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gthcfjrbpm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtgrcoghwu.html

[Q43] 标量子查询
来源：http://hz.redwolf501.top/gtdbyqazmv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hysaishi.cn/gtecsgzjyv.html

[Q44] IN 子查询
来源：http://hz.nanxuanxn.top/gtxopdddrc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cdnleiting.top/gtofzhsobx.html

[Q45] EXISTS 判断存在
来源：http://hz.hfpthk.cn/gtoqkxheuj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gthbxgnedq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gtbpvizasd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtqskhwxcy.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gtoybrnxxp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yongpay.top/gtnpmujlfn.html

[Q48] CTE 公用表表达式
来源：http://hz.dianchejie.cn/gtvuhjxoxk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.havefunace.top/gtgomiwvmq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtbfrktohc.html

[Q49] 更新单行
来源：http://hz.jlsjyb.cn/gtvjsggrbn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtjlighlrf.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtxflftwyi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gteboqkmem.html

[Q51] 用子查询更新
来源：http://hz.andypj.xyz/gtkjmtsyju.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydzc1.top/gteystcijj.html

[Q52] 删除指定行
来源：http://hz.yj20258888.top/gtqoezjqtg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aizwys.cn/gtfzchynbn.html

[Q53] 按条件删除
来源：http://hz.pengpengdd.cyou/gtjxkxpjhs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtzkfmfseq.html

[Q54] 清空表
来源：http://hz.shanyushiyangtech.top/gtzcfifcts.html

TRUNCATE TABLE logs;
来源：http://hz.cheryme.top/gtmkenhdyd.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtuozncmgb.html


<!-- 参考信息 -->