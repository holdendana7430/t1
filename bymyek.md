代发 wailian999

[N09] 栈与队列
来源：http://hz.chenjidiqi.icu/gtordjuhot.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daxiang520.top/gtntvnyznp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtdhcacznz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtqufxegei.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aizwys.cn/gtglicjscz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhongyouzk.top/gtgkolzain.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtsyzsfenn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtrdguemgc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jqgfzy.top/gtcervvzyy.html

[N10] 链表节点定义
来源：http://hz.chenjidiqi.icu/gtluyxagpi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cqqwz.cn/gtgnjpnoke.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gtfgjvgpoj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ppjwa.cn/gtlqrvvexq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guowangkeji.top/gtgxjdpddy.html

Java: class Node { int v; Node next; }
来源：http://hz.dashuyun.cn/gtnatgzzhv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtcopfstfk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sxryk.cn/gtsdqimpgo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.birdmap.top/gtuhaahaze.html

[N11] 二叉树中序遍历
来源：http://hz.ydjk.org.cn/gtnvlpkapc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.birdmap.top/gtcktmzrjt.html

PHP:  // 手写递归函数
来源：http://hz.yj20258.top/gtgbrifedg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtgokjoxmn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtdcbiqwlm.html

Java: // 手写递归
来源：http://hz.xuetiantiany.cn/gttdelcxsg.html

Go:   // 手写递归
来源：http://hz.ybcxt.top/gtqrgogmgl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.feifeiyinyue.top/gtwrsisxhi.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gthzilgxby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gttamplbio.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gzhubu.top/gttsbrlepc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.fzhhl.top/gtmbbnkmfd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gtzztsoqol.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtmsbqlrbo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtiyfqgkgs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtekyqccqp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.quarkkingdee.top/gtdlcdxlat.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtqlgniivv.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnfkirhfv.html

O. 并发与异步
来源：http://hz.cheryme.top/gttsafdtiy.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnntcrsok.html

[O01] 启动一个线程
来源：http://hz.guannengcc.top/gtwtbnpbmz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydjk.org.cn/gtnglzabkm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.meibo888.top/gtzjmwgbig.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuanzhike.top/gtvqccmlvr.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtzxsahdyr.html

Java: new Thread(() -> f()).start()
来源：http://hz.ydzc1.top/gteqxrcqfm.html

Go:   go f()
来源：http://hz.sysykeji.top/gtbpjnprqc.html

Ruby: Thread.new { f }
来源：http://hz.cheryme.top/gtgdbrjblv.html

C#:   Task.Run(() => F());
来源：http://hz.hnxiangtu.top/gtmmkbaxna.html

[O02] 使用线程池
来源：http://hz.ybcxt.top/gtnixdmizm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydjk.org.cn/gtbuboacou.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.vqdsnc.cn/gtpupdxcaj.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtptcxkugt.html

TS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtqmerturw.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtwqevdzcu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hfpthk.cn/gttfafqfyf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daxiang520.top/gtsgbxngdu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258.top/gtjwnextsq.html

[O03] 加锁保护共享数据
来源：http://hz.zhongyouzk.top/gtpaasjocy.html

Py:   with lock: shared += 1
来源：http://hz.wangdashe.top/gtihbivfnk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zycfv.cn/gtnqmghxrb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.0kj1m.cn/gtnsxbpcco.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtwdtajrti.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gtfzpqaaox.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangkeji.top/gtmjcejaxe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtpcfzwppf.html

C#:   lock (gate) { shared++; }
来源：http://hz.havefunace.top/gtubqskbkp.html

[O04] 定义异步函数并等待
来源：http://hz.sysykeji.top/gtdjztnkxn.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gtepcmdvfv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.guowangkeji.top/gtbiowmpef.html

JS:   async function f() { await g(); }
来源：http://hz.nanxuanxn.top/gtcgaxktjg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xuetiantiany.cn/gtmdomusfd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.kuanghao11.cn/gtyvnwkeqs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtjntguxdz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jianghu66.top/gtwwijxneg.html

C#:   async Task F() { await G(); }
来源：http://hz.52xcode.cn/gtzqhqwhjg.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtixvwbupd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtrdyhnniq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.pycfn.com/gtqchmbzrq.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtwqgdeeqv.html

TS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtrnaswhxd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ybcxt.top/gtnwiijnbi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.bjfxy.top/gtsbceeilb.html

Ruby: threads.map(&:join)
来源：http://hz.zhengqikj.top/gtyuibzcdc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yanxiufei.cn/gttdbcmfmf.html

[O06] 使用进程池
来源：http://hz.guowangkeji.top/gtpyasqkfm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cqqwz.cn/gtwxvpkbrj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtqdnsjrmm.html

JS:   // child_process / cluster 模块
来源：http://hz.yj20258.top/gtbzbahoax.html

TS:   // child_process / cluster 模块
来源：http://hz.daria6918.cn/gtonypwuut.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangdashe.top/gtnijxeqdg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yuxming.cn/gtfbipkgep.html

Ruby: // fork 块
来源：http://hz.cdnleiting.top/gtlthqquoo.html

C#:   Parallel.For
来源：http://hz.bjfxy.top/gtvuapjrpb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdselwiev.html

P. 常用工具函数
来源：http://hz.ehwqpu.com/gtcuwlhqri.html

================================================================================
来源：http://hz.yj20258.top/gtvmwneyfu.html

[P01] 生成 UUID
来源：http://hz.sufxvd.cn/gtrcsmcbco.html

Py:   str(uuid.uuid4())
来源：http://hz.gotoacloud.top/gtdnlnebea.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.wangdashe.top/gtpiyzhkyj.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtxgjzhyvb.html

TS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtzjluszeo.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtmvnugjhc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fengsongda.top/gthflpdaaz.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gtjjvnmygl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258.top/gtfrlsumsp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.vqdsnc.cn/gtuasganno.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258888.top/gtscupjeey.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pycfn.com/gtuyibwnpj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ppjwa.cn/gtwvlvlyao.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xinyue.icu/gtltmqjkeb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hnxiangtu.top/gtfvsrwjtl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangkeji.top/gtfwtpkdok.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ybcxt.top/gtrmjcmbgi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hongshengwenyu.top/gtslsqydjc.html

[P03] 生成短随机字符串
来源：http://hz.xinyue.icu/gtcexoyucm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.bjfxy.top/gtagfacqpx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yangfankeji.com/gtgqrbsuxa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fzhhl.top/gtvlyeqniy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhijiandao.cn/gtmmsreudz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aibaodan.cn/gtndplopbb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangdashe.top/gtowzhxuiw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sufxvd.cn/gtsoazkqbk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daxiang520.top/gttcgxbaje.html

[P04] 求长度
来源：http://hz.cashguo.top/gtnnaabhsc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.quarkkingdee.top/gtehvlbbhm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtkwrswwen.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtywcnyeai.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gttizwassv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuxming.cn/gtbtayvrkp.html

Go:   len(arr);  len(m)
来源：http://hz.tanke756.top/gtmirvnvas.html

Ruby: x.length;  x.size
来源：http://hz.smart0.xyz/gtmphdoreg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtguvbcvnp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dashuyun.cn/gtqodgoyfv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.zdqjudy.top/gtdakbvlra.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tanke756.top/gtdpmbgtik.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gtcgfcpvvk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtzmoueqft.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xziqi.cn/gtywtjlrer.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xinyue.icu/gtqjjytuto.html

Ruby: a == b
来源：http://hz.fzhhl.top/gtwtgjlvlx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gtznwsprkw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gotoacloud.top/gtrrlhgkcu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigfzy.top/gtafvjceyy.html

PHP:  if (empty($x)) {}
来源：http://hz.jianghu66.top/gtvziekifv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.daxiang520.top/gtllaihqcv.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtkzfehmxl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtmswmpwmx.html

Go:   if x == nil {}
来源：http://hz.meibo888.top/gtrnrtganp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.andypj.xyz/gtyyvykjtc.html

C#:   if (x is null) {}
来源：http://hz.yj20258888.top/gtwllfdbkc.html

[P07] 防抖与节流
来源：http://hz.meibo888.top/gtlswfnsuv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guannengcc.top/gtfvwircir.html

PHP:  // 手写时间戳比较
来源：http://hz.0kj1m.cn/gtkfyoyvkv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gterakrewq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guannengcc.top/gtmybkadee.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zycfv.cn/gtqcauuohp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ivvv.top/gtwbdwster.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sufxvd.cn/gtvobeobpj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yonumen.top/gtfcvwrtbp.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtqvbvkimr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gtaqgzwiyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnxiangtu.top/gtkguzejed.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jlsjyb.cn/gtqpaymoxz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtyiocsypi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gtbrqopdtk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnxiangtu.top/gtfyyfwxpp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hysaishi.cn/gtgqtvhvns.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.vqdsnc.cn/gtrpzdcqpa.html

================================================================================
来源：http://hz.ydzc1.top/gtwqnpnfvb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.tianlin.xyz/gtkmufrynd.html

================================================================================
来源：http://hz.gzhubu.top/gtxirzspfh.html

[Q01] 创建表
来源：http://hz.cdnleiting.top/gtlonuoukx.html

CREATE TABLE users (
来源：http://hz.zhongyouzk.top/gtbxcuouuy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.quarkkingdee.top/gtxztbkurc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yj20258.top/gtewwtfsst.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtnreewfbu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.mhx1999.top/gtnaheioyz.html

);
来源：http://hz.cucudq.cn/gtropbaswn.html

[Q02] 创建带外键的表
来源：http://hz.snrcjt.cn/gtmjycizzq.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gtjdceuktz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhaomingkeji.xyz/gtcalpznbp.html

user_id INT NOT NULL,
来源：http://hz.yonumen.top/gtxpdqhbkj.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigfzy.top/gtxpyvnuyw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.vqdsnc.cn/gtchicpepy.html

);
来源：http://hz.chenlongwang.top/gtvfrovigw.html

[Q03] 增加列
来源：http://hz.sufxvd.cn/gtjssuulfp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ywan-chungtsiang.top/gtkamwhiqs.html

[Q04] 修改列类型
来源：http://hz.xziqi.cn/gtkzpvlphe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shanyushiyangtech.top/gtxpdvchnr.html

[Q05] 重命名列
来源：http://hz.shangyingyoupin.top/gtkvostpjg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtesdbjnoy.html

[Q06] 删除列
来源：http://hz.aibaodan.cn/gtjsqjuixs.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.meibo888.top/gtccqtvmgh.html

[Q07] 删除表
来源：http://hz.hnqzz.top/gtnfrnetvl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.52xcode.cn/gttsiliajd.html

[Q08] 创建普通索引
来源：http://hz.hnqzz.top/gtakxztsom.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gtqitkqrva.html

[Q09] 创建唯一索引
来源：http://hz.hongshengwenyu.top/gtitwbijky.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.316326.xyz/gthiznipyt.html

[Q10] 插入单行
来源：http://hz.jinqigfzy.top/gtdsgitcgz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.mhx1999.top/gtngihefeq.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtygapzlsx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.svipenyu.cn/gtfyiqkunf.html

[Q12] 插入后取自增 ID
来源：http://hz.quarkkingdee.top/gtpzenwbwq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fzhhl.top/gtkudgekey.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ivvv.top/gtnjgnomhh.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtallvqwvu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.redwolf501.top/gtwyppxtoi.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinghuilouyu.cn/gtkrrkpxae.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtkfgstiso.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.quarkkingdee.top/gtnhtnphzg.html

[Q15] 查询全部
来源：http://hz.tian-w.cn/gtjcfkmwtv.html

SELECT * FROM users;
来源：http://hz.jqgfzy.top/gtaxapjqym.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangtech.top/gtxgbztmqd.html

SELECT id, name FROM users;
来源：http://hz.jianghu66.top/gtcqkfzytr.html

[Q17] 条件查询
来源：http://hz.quarkkingdee.top/gthkkfkpmr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxinkj.top/gtcwflidin.html

[Q18] 模糊匹配
来源：http://hz.xuetiantiany.cn/gtuntytzkx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shzxlz.cn/gtwipkzmgd.html

[Q19] 范围查询
来源：http://hz.aizwys.cn/gtcydwuwwp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shangyingyoupin.top/gtpqxpegfx.html

[Q20] IN 列表
来源：http://hz.svipenyu.cn/gtwfdpzjmt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gtkkvvsepy.html

[Q21] 空值判断
来源：http://hz.yj20258888.top/gtguckpcdc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hywenlv.cn/gtiwnbmfwq.html

[Q22] 排序
来源：http://hz.xinyue.icu/gtnudfskud.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yuxming.cn/gtrgeqaumt.html

[Q23] 分页
来源：http://hz.feifeiyinyue.top/gtwitqddtl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daxiang520.top/gtunqvoqzw.html

[Q24] 去重
来源：http://hz.cashguo.top/gtvdzibtla.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhiwuduotai.top/gtjhurhbjy.html

[Q25] 只取前 N 条
来源：http://hz.gzhubu.top/gtanvnjifp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.52xcode.cn/gtlqnzxusv.html

[Q26] 计数
来源：http://hz.tianlin.xyz/gtxsashstl.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtzfhuvbmk.html

[Q27] 条件计数
来源：http://hz.yuxming.cn/gtxghtaiyk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zdqjudy.top/gtvqurgmhb.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gtllulmhqs.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhiwuduotai.top/gtwphkqftp.html

[Q29] 最大最小值
来源：http://hz.shuidangran.top/gtoqgjhfgn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gogol.net.cn/gtjizrbtmn.html

[Q30] 分组统计
来源：http://hz.zhijiandao.cn/gtyqluvurx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtppwbkxei.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtyptspory.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.meibo888.top/gtrwnvvcfo.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtxgzezkku.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtcpzwezxp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.nanxinkj.top/gtzksrtkka.html

[Q33] 多列分组
来源：http://hz.xinyue.icu/gtuujdzumy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenzaomai.com/gtijzkybdd.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtuiobxrks.html

SELECT * FROM (
来源：http://hz.haohaochexian.top/gtdvqxpnvv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ivvv.top/gtgwxzvejr.html

) t WHERE rn = 1;
来源：http://hz.xinyue.icu/gtfqtrxbqa.html

[Q35] 内连接
来源：http://hz.xuetiantiany.cn/gtfcsbmxti.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtbrsyastq.html

[Q36] 左连接
来源：http://hz.yuxming.cn/gtibtwfzyi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangkeji.top/gtzxwrexkj.html

[Q37] 右连接
来源：http://hz.vqdsnc.cn/gtsdpidbav.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xinyue.icu/gtgsrhvyev.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sufxvd.cn/gtvjgtdlyk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nwbrower.top/gtseuqdbsc.html

[Q39] 自连接（查上下级）
来源：http://hz.fengsongda.top/gtikqigwzh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yvedp.cn/gtserekzjs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gogol.net.cn/gtntcpnbmb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhijiandao.cn/gtekvnvghr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jianghu66.top/gtanebgjwy.html

[Q41] 多表连接
来源：http://hz.gotoacloud.top/gtvaxhosst.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dianchejie.cn/gtituohred.html

JOIN users u ON u.id = o.user_id
来源：http://hz.9152youxi.cn/gtncaiwudx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtvbelgwoo.html

[Q42] 连接条件附加过滤
来源：http://hz.hysaishi.cn/gtucrfpddr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.316326.xyz/gtwqkhudxa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yuanzhike.top/gtzqpwgilm.html

[Q43] 标量子查询
来源：http://hz.jinqigufen.top/gtlucuidpo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gtiadbzgaf.html

[Q44] IN 子查询
来源：http://hz.yj202588.top/gtopxfadau.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtimcrcfix.html

[Q45] EXISTS 判断存在
来源：http://hz.c1oappe.top/gtqirjkxig.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtdxerpuuq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtgjrlcsrg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtzlujkxwz.html

[Q47] 与平均值比较
来源：http://hz.xingfuxueyuan.xyz/gtzbaemodi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtumoyxgmw.html

[Q48] CTE 公用表表达式
来源：http://hz.haohaochexian.top/gtcxuobric.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sysykeji.top/gtjdetxmqn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sufxvd.cn/gtzxwpqyfu.html

[Q49] 更新单行
来源：http://hz.vqdsnc.cn/gtirlllodd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jyoumei.cn/gtuyhkxqas.html

[Q50] 批量更新
来源：http://hz.xylfe.cn/gtdqwceyvl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hongshengwenyu.top/gtjanaurps.html

[Q51] 用子查询更新
来源：http://hz.svipenyu.cn/gtxmtlssvu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gttuwmzwgt.html

[Q52] 删除指定行
来源：http://hz.chenzaomai.com/gtxrdqkknb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhaomingkeji.xyz/gtiupvkrvx.html

[Q53] 按条件删除
来源：http://hz.yangfankeji.com/gtwhnikhhf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yonumen.top/gtrxjlwjvu.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtmkbwvyhw.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gtweaqlptb.html

[Q55] 排名（并列占位）
来源：http://hz.zhijiandao.cn/gtzkmjvhes.html


<!-- 参考信息 -->