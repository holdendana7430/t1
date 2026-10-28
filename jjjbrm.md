代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuanzhike.top/gthsdiofvo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.svipenyu.cn/gtnvbwvrnh.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtrlumdnkt.html

Java: // 手写 HashMap
来源：http://hz.hammf.cn/gtrbhfgjmb.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtqpfksujm.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gtdjkhkgry.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fengsongda.top/gtxpexqxtb.html

[N08] 生成全排列
来源：http://hz.52xcode.cn/gtrrfvmfll.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gtyzjqetnx.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtcayfblir.html

JS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtvvckaxhd.html

TS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtmsudalvm.html

Java: // 手写回溯递归
来源：http://hz.mhx1999.top/gtbtttaebw.html

Go:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtpemsoahx.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gtlroykmka.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtgoqyrxsc.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtqhskntng.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zycfv.cn/gtypivbdzg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cqqwz.cn/gtfyzscnyg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtigqatoes.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ppjwa.cn/gtuhayauif.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hysaishi.cn/gtrtxkrtfz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtwyfutdsv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gtifycwdgj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuanzhike.top/gtdkqfmlpc.html

[N10] 链表节点定义
来源：http://hz.zhiwuduotai.top/gtjlxrafee.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtzupldoid.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hammf.cn/gtwlqeaoou.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.mhx1999.top/gtciobpxmr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj202588.top/gtpbqzqyzi.html

Java: class Node { int v; Node next; }
来源：http://hz.cucudq.cn/gtxwezfcez.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigufen.top/gtfjxxsjlx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtlyhixpre.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtvgyawjjs.html

[N11] 二叉树中序遍历
来源：http://hz.jinqigfzy.top/gtcakezigz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nwbrower.top/gtagwtervw.html

PHP:  // 手写递归函数
来源：http://hz.meibo888.top/gtokdmzeir.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtnddizmpe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtmbuxgjyt.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtpliifpqw.html

Go:   // 手写递归
来源：http://hz.kuanghao11.cn/gtogkgoyxb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cucudq.cn/gtydjdpehr.html

C#:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtywhluomy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gtencvxuvq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhoulong.xyz/gtotxlfdju.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gtrpodmpws.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258888.top/gtwhshpazi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shangyingyoupin.top/gtodaqvjxq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtwcaursnk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tianlin.xyz/gtvhncfhdc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jlsjyb.cn/gtytkdyxzk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtqnvarryb.html

================================================================================
来源：http://hz.fzhhl.top/gtfypdfktq.html

O. 并发与异步
来源：http://hz.xinyue.icu/gtliyqrwnl.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkcsgiruo.html

[O01] 启动一个线程
来源：http://hz.tian-w.cn/gtjmtkzypg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hongshengwenyu.top/gtwatzrkhm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxuanxn.top/gtjdqwyiwn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnqzz.top/gtqntxpdgs.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtvmnqgdvr.html

Java: new Thread(() -> f()).start()
来源：http://hz.ehwqpu.com/gtiykeylsi.html

Go:   go f()
来源：http://hz.zhijiandao.cn/gtmpgjxxmj.html

Ruby: Thread.new { f }
来源：http://hz.mhx1999.top/gtzsvjelxn.html

C#:   Task.Run(() => F());
来源：http://hz.cqqwz.cn/gtbzaahhyr.html

[O02] 使用线程池
来源：http://hz.nanxuanxn.top/gtrmitxypx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daria6918.cn/gtjeekddvn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.sxryk.cn/gtwhfqkujw.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtlobaonlf.html

TS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtqquhfrxz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuxming.cn/gtdtivltxl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.aibaodan.cn/gtzfvosnjh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yonumen.top/gtvcumgwzf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.feifeiyinyue.top/gtrltlnyrq.html

[O03] 加锁保护共享数据
来源：http://hz.aizwys.cn/gtuiquujhk.html

Py:   with lock: shared += 1
来源：http://hz.316326.xyz/gtaodciefo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtpwznyftj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jiagoushi.top/gtdhzdkfzh.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtrryzpyuz.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtoaeosnkl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtqxyhzpes.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cucudq.cn/gtylpfzsph.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhiwuduotai.top/gtchqzncwl.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtebvhmcpr.html

Py:   async def f():⏎    await g()
来源：http://hz.chenzaomai.com/gtfbmqdisi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dashuyun.cn/gtxutknodf.html

JS:   async function f() { await g(); }
来源：http://hz.jinyuanbaomall.cn/gtxrxfogim.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ehwqpu.com/gtbtsxnaik.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tianlin.xyz/gtgyefemxg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.haohaochexian.top/gtuolbptur.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tianlin.xyz/gtjymmqkuq.html

C#:   async Task F() { await G(); }
来源：http://hz.chenlongwang.top/gtandkztzl.html

[O05] 并发执行并等待全部完成
来源：http://hz.hywenlv.cn/gtubabkwsr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xingfuxueyuan.xyz/gtxorkfdtm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yueranfly.top/gtvwjdkhwz.html

JS:   await Promise.all(tasks)
来源：http://hz.0kj1m.cn/gtaznbawqc.html

TS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtykfjtzfh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jiagoushi.top/gtcwzdpzfl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aibaodan.cn/gtdpjljwxz.html

Ruby: threads.map(&:join)
来源：http://hz.jianghu66.top/gtvbcoclqr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ydjk.org.cn/gtptqfpbqz.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gttdhdydcd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hywenlv.cn/gtryubolwi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.havefunace.top/gtdvsiqylg.html

JS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gthuhodirw.html

TS:   // child_process / cluster 模块
来源：http://hz.jinghuilouyu.cn/gtifzsuvva.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtrpxogial.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.havefunace.top/gtulslsudy.html

Ruby: // fork 块
来源：http://hz.jinyuanbaomall.cn/gtzjotwrzv.html

C#:   Parallel.For
来源：http://hz.feifeiyinyue.top/gtbdacyzzp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtbuwofzfz.html

P. 常用工具函数
来源：http://hz.ehwqpu.com/gtkqxpesxs.html

================================================================================
来源：http://hz.cucudq.cn/gtsenskdkc.html

[P01] 生成 UUID
来源：http://hz.mhx1999.top/gtudprpsih.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gtafgzitnl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pycfn.com/gtebcizhop.html

JS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtmiqrxkzy.html

TS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtdrevdjqm.html

Java: UUID.randomUUID().toString()
来源：http://hz.ydjk.org.cn/gtfkpzetbt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.iojbl.cn/gtdfrxromz.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtsbeyfjit.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ywan-chungtsiang.top/gtzmefaajr.html

[P02] MD5 / SHA256 摘要
来源：http://hz.daria6918.cn/gtdqnhtnhp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sysykeji.top/gtsrykgtpk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yvedp.cn/gtyvpvsywd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shangyingyoupin.top/gtoxmafnsm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtjbhuapqk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuanzhike.top/gtjjvdnngi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ywan-chungtsiang.top/gtmerbiqqy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xingfuxueyuan.xyz/gtlnlpvqyb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fzhhl.top/gtkrolqlom.html

[P03] 生成短随机字符串
来源：http://hz.zhijiandao.cn/gtgecalzhz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.feifeiyinyue.top/gthemprspj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gtbetnkwrf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtjkclukkt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtstcplxgs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenlongwang.top/gtmeqxnmim.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yvedp.cn/gtjgmnvmyl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xylfe.cn/gtuurwcpat.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yueranfly.top/gtkovokdir.html

[P04] 求长度
来源：http://hz.yueranfly.top/gtnuigcyyb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.meibo888.top/gtvafqxlwo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxinkj.top/gtfmdgmfgs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtekkezkvm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtbjhwxcox.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yuxming.cn/gtawswagxf.html

Go:   len(arr);  len(m)
来源：http://hz.nanxinkj.top/gtrptqxnnd.html

Ruby: x.length;  x.size
来源：http://hz.wangshuangyany.cn/gtrnnexgci.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhaomingkeji.xyz/gttnwuqvls.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hnqzz.top/gtmmskusqe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gtkxobgqlo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.mhx1999.top/gtghzaiqlx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.guowangkeji.top/gtfukisbpz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtxfhlpoyf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cqqwz.cn/gtndttvbzm.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shuidangran.top/gtjetsejfl.html

Ruby: a == b
来源：http://hz.fengsongda.top/gtqnkkveua.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jyoumei.cn/gthrsyckbk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtcwibtcts.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydjk.org.cn/gtemoabmth.html

PHP:  if (empty($x)) {}
来源：http://hz.jyoumei.cn/gtlqfoqjvw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.52xcode.cn/gtfijmysed.html

TS:   if (x == null) {}
来源：http://hz.yj20258.top/gtxtvrhhri.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.havefunace.top/gtuunswpei.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtoqfsrord.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenzaomai.com/gtufqtjnce.html

C#:   if (x is null) {}
来源：http://hz.zycfv.cn/gteijnhxoa.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtwoszvozn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.mhx1999.top/gtmryfaptk.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gtumvljctj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pengpengdd.cyou/gtccsqayry.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtntbfvkds.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtfilmhdto.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhaomingkeji.xyz/gtfozafytg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gtmpcpqzbu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dianchejie.cn/gtyootfiws.html

[P08] 处理浮点精度问题
来源：http://hz.9152youxi.cn/gtdeyzacie.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.havefunace.top/gtjptbasqw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yonumen.top/gtuwwnzecu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cashguo.top/gtnmjcqjhp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sxryk.cn/gtjoenlkbi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.birdmap.top/gtwnmwzayx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sysykeji.top/gtoummxitc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.bjfxy.top/gtssgtbjqd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtrhklichv.html

================================================================================
来源：http://hz.gogol.net.cn/gttzsojmiz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ywan-chungtsiang.top/gtlshnoqtp.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttdzkdaqc.html

[Q01] 创建表
来源：http://hz.andypj.xyz/gtfuelsvcm.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtqdmojcpp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jianghu66.top/gtzeoidaja.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yonumen.top/gthvkyjufd.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hysaishi.cn/gtipploacs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinghuilouyu.cn/gtedpiceio.html

);
来源：http://hz.wangdashe.top/gthtwboolm.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtfxaopyok.html

CREATE TABLE orders (
来源：http://hz.hnxiangtu.top/gtrajfotye.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtiyovooat.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gtyjvsjpda.html

amount DECIMAL(10, 2),
来源：http://hz.feifeiyinyue.top/gtvnzytfig.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.mhx1999.top/gtwyijwpsf.html

);
来源：http://hz.yangfankeji.com/gtkkrapreh.html

[Q03] 增加列
来源：http://hz.hywenlv.cn/gtuvyiqanw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtobcfnupu.html

[Q04] 修改列类型
来源：http://hz.kuanghao11.cn/gtnkaomxgz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fzhhl.top/gtvvlfpfpx.html

[Q05] 重命名列
来源：http://hz.ywan-chungtsiang.top/gtztoljqwx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hfpthk.cn/gtofvtvazf.html

[Q06] 删除列
来源：http://hz.wangshuangyany.cn/gtctpxzihc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zycfv.cn/gtarmbbonh.html

[Q07] 删除表
来源：http://hz.guannengcc.top/gtrxreazwd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shangyingyoupin.top/gtoqlvbrww.html

[Q08] 创建普通索引
来源：http://hz.wangshuangyany.cn/gtyjuniyiv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtznpitfyb.html

[Q09] 创建唯一索引
来源：http://hz.0kj1m.cn/gtjzbdctae.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.daxiang520.top/gtjdnsyaar.html

[Q10] 插入单行
来源：http://hz.hfpthk.cn/gtaokwkohd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aizwys.cn/gtkzlaijmq.html

[Q11] 一次插入多行
来源：http://hz.aibaodan.cn/gtgmwcjzbn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dianchejie.cn/gtxbwpfelo.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gttfnbobmf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xuetiantiany.cn/gtvnuzziss.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yonumen.top/gtmuooqypq.html

[Q13] 忽略重复插入
来源：http://hz.yongpay.top/gtdjokyjgy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shanyushiyangkeji.top/gtfszidluk.html

[Q14] 存在则更新（upsert）
来源：http://hz.dianchejie.cn/gtcaaqnmfe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jinqigufen.top/gteynphawy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xylfe.cn/gtwupchpdo.html

[Q15] 查询全部
来源：http://hz.ydzc1.top/gtidddlimy.html

SELECT * FROM users;
来源：http://hz.gogol.net.cn/gtuvevqoei.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtqggmkemb.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtoiifiqep.html

[Q17] 条件查询
来源：http://hz.chenlongwang.top/gtpatvfelz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.daria6918.cn/gtqypmhuyx.html

[Q18] 模糊匹配
来源：http://hz.tanke756.top/gtvovefaiu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.dashuyun.cn/gtpalagfpo.html

[Q19] 范围查询
来源：http://hz.9152youxi.cn/gtsgzpqyqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.vqdsnc.cn/gtofmajphx.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtqtgrkyid.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gtpycituem.html

[Q21] 空值判断
来源：http://hz.xuetiantiany.cn/gthhxtddsd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guannengcc.top/gtavnukexn.html

[Q22] 排序
来源：http://hz.sweek.top/gtxlrvvsgi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.316326.xyz/gtasztnyoi.html

[Q23] 分页
来源：http://hz.hnxiangtu.top/gtltgeacrz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yvedp.cn/gtpyvssutm.html

[Q24] 去重
来源：http://hz.birdmap.top/gtuvxkyhny.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtprxdogyf.html

[Q25] 只取前 N 条
来源：http://hz.daxiang520.top/gttigfjmkq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhixingplan.top/gtwdurdrmz.html

[Q26] 计数
来源：http://hz.jqgfzy.top/gtszvcxuxh.html

SELECT COUNT(*) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtrlsarppd.html

[Q27] 条件计数
来源：http://hz.bjfxy.top/gtnvonwfys.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.andypj.xyz/gtptfcuwpd.html

[Q28] 求和与平均
来源：http://hz.xziqi.cn/gtbkwylwsx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtnvgxgopl.html

[Q29] 最大最小值
来源：http://hz.haohaochexian.top/gtdeaxbifr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtfbqwbvlx.html

[Q30] 分组统计
来源：http://hz.tian-w.cn/gtnvtrzede.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtjngiqtvb.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtvriamche.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gtcyliaizq.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtyysozxgb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtkkrtnwmn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jlsjyb.cn/gtfpmmlydk.html

[Q33] 多列分组
来源：http://hz.andypj.xyz/gtzccrchww.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtjoiuobck.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtdeaatxuj.html

SELECT * FROM (
来源：http://hz.smart0.xyz/gtorjkexkj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.316326.xyz/gtafqiukqn.html

) t WHERE rn = 1;
来源：http://hz.shzxlz.cn/gtyboirias.html

[Q35] 内连接
来源：http://hz.fengsongda.top/gtkjwfznzg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yangfankeji.com/gtiltgqqhn.html

[Q36] 左连接
来源：http://hz.wangshuangyany.cn/gtpfmzrqwd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yueranfly.top/gttjaxooay.html

[Q37] 右连接
来源：http://hz.zycfv.cn/gtscqxutja.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.feifeiyinyue.top/gtmkbjisjj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hywenlv.cn/gtqngaypnp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtgkeoadhi.html

[Q39] 自连接（查上下级）
来源：http://hz.tianlin.xyz/gtzocnpqys.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fengsongda.top/gtsovetcdj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258.top/gtohiepjkt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj202588.top/gtmxfatufj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.svipenyu.cn/gtszpaagik.html

[Q41] 多表连接
来源：http://hz.tian-w.cn/gtjgmrrvaw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sysykeji.top/gtluyzskns.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cdnleiting.top/gtoeauhlwk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gzhubu.top/gtcwnmuuyf.html

[Q42] 连接条件附加过滤
来源：http://hz.andypj.xyz/gtimeepqta.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtulhzbdud.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dashuyun.cn/gtxcbcafgn.html

[Q43] 标量子查询
来源：http://hz.ppjwa.cn/gtfnpmbtpi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinyuanbaomall.cn/gtzpqvssyl.html

[Q44] IN 子查询
来源：http://hz.jiagoushi.top/gtjhkfrzrf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ppjwa.cn/gtsapkuoqb.html

[Q45] EXISTS 判断存在
来源：http://hz.cucudq.cn/gtlptrezzo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtbctxelfb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtolzkzfat.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtmnldtxeo.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtofxoocpb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenjidiqi.icu/gtxkhtmlfb.html


<!-- 参考信息 -->