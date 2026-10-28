代发 wailian999

Java: // 手写回溯递归
来源：http://hz.andypj.xyz/gtczgewjnm.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtnpiejiuz.html

Ruby: arr.permutation.to_a
来源：http://hz.andypj.xyz/gtitrqkxek.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gtdntblpjd.html

[N09] 栈与队列
来源：http://hz.cdnleiting.top/gtntnooxyb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenjidiqi.icu/gtcatmdzvx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gtqajzkkgg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gtztinawag.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aibaodan.cn/gtumfetbho.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ppjwa.cn/gtntchnrqz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnqzz.top/gtouwrzmam.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxuanxn.top/gtzsdudsku.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.iojbl.cn/gtkumwvull.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangtech.top/gtxaidypyo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gtuftxlcrh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtmcdruxvd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuetiantiany.cn/gtjtcnhalp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guannengcc.top/gtixbbjknq.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtrsvexpoo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.andypj.xyz/gtraxelono.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhixingplan.top/gtljhfnilr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xziqi.cn/gtqlifnvpv.html

[N11] 二叉树中序遍历
来源：http://hz.xingfuxueyuan.xyz/gtcvgxmpch.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pengpengdd.cyou/gtfylykdwl.html

PHP:  // 手写递归函数
来源：http://hz.zhaomingkeji.xyz/gteptlxsoj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yanxiufei.cn/gtpysgdjpi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtszbskquq.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtviotwmpn.html

Go:   // 手写递归
来源：http://hz.yuanzhike.top/gtuhjnmwtm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangkeji.top/gtokasckkg.html

C#:   // 手写递归
来源：http://hz.ivvv.top/gtxtolucvf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhijiandao.cn/gtutfxybqc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cucudq.cn/gtqwbudvym.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sxryk.cn/gtqdwqmpoc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtlgrmhjti.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtifaeprce.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guannengcc.top/gtmyklxkls.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhiwuduotai.top/gtcuxclpnz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhijiandao.cn/gtaksekfcb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtnqfxnmjj.html

================================================================================
来源：http://hz.jinqigufen.top/gtmprzlycl.html

O. 并发与异步
来源：http://hz.zhengqikj.top/gtjcvhgwvc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtsokssvlb.html

[O01] 启动一个线程
来源：http://hz.xingfuxueyuan.xyz/gtyubwwomy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhengqikj.top/gtdduxuynx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinyuanbaomall.cn/gtontwpxia.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jyoumei.cn/gtkpocujkp.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtzymxpegl.html

Java: new Thread(() -> f()).start()
来源：http://hz.shangyingyoupin.top/gtutxtwgcs.html

Go:   go f()
来源：http://hz.pycfn.com/gtogzbzmei.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtqxyzhlsa.html

C#:   Task.Run(() => F());
来源：http://hz.tian-w.cn/gtrelckjpk.html

[O02] 使用线程池
来源：http://hz.jinyuanbaomall.cn/gtvrjtalvx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zdqjudy.top/gtjifhkbkt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ivvv.top/gtaisoayzo.html

JS:   // worker_threads 线程池
来源：http://hz.xinyue.icu/gtuwcxdjvz.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gthstoycsa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtdzzuazmr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.nwbrower.top/gteuhmpviu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtpquivqku.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hammf.cn/gtwaljhfzn.html

[O03] 加锁保护共享数据
来源：http://hz.ppjwa.cn/gtawubkckb.html

Py:   with lock: shared += 1
来源：http://hz.cqqwz.cn/gtecxwecpx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dianchejie.cn/gtcimnkbmp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtkpobfdeu.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtcupglmgm.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtlprepuvk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fzhhl.top/gtlpxacqhd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tanke756.top/gtnawublso.html

C#:   lock (gate) { shared++; }
来源：http://hz.hammf.cn/gtlcgnxwts.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtnmgnhvof.html

Py:   async def f():⏎    await g()
来源：http://hz.gogol.net.cn/gtcjoalujc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nwbrower.top/gtujvonakl.html

JS:   async function f() { await g(); }
来源：http://hz.c1oappe.top/gtodxoyzvj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnxiangtu.top/gtaauveabk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinyuanbaomall.cn/gtzxhekupv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sufxvd.cn/gtjjzcivaz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daxiang520.top/gtnozprrll.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtqmfyoefl.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gtlsoswljj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtnzuhkypg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hysaishi.cn/gtopwzvkjn.html

JS:   await Promise.all(tasks)
来源：http://hz.redwolf501.top/gtzackfict.html

TS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtjrshwweo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.9152youxi.cn/gtywqbjwha.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj202588.top/gtgqclvnnw.html

Ruby: threads.map(&:join)
来源：http://hz.yuxming.cn/gtbrgbgwst.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.svipenyu.cn/gtvabxqcsu.html

[O06] 使用进程池
来源：http://hz.jianghu66.top/gtfuwcaszw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nwbrower.top/gttgsdpsgq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.kuanghao11.cn/gtylubnsht.html

JS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gttpiggdns.html

TS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gthepgrnze.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cashguo.top/gtcvoufpuf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cheryme.top/gtqkqyvynz.html

Ruby: // fork 块
来源：http://hz.iojbl.cn/gtzqvlsade.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gtqnolikuh.html

================================================================================
来源：http://hz.ppjwa.cn/gtkawefvmi.html

P. 常用工具函数
来源：http://hz.ehwqpu.com/gtlsfixvou.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtvdaoqvfu.html

[P01] 生成 UUID
来源：http://hz.pengpengdd.cyou/gtmdotcoch.html

Py:   str(uuid.uuid4())
来源：http://hz.yueranfly.top/gtxvhknhyg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.iojbl.cn/gtgqfcatwp.html

JS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtlsflhduy.html

TS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtsxhxfbcq.html

Java: UUID.randomUUID().toString()
来源：http://hz.yongpay.top/gtjqdlqlzo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.vqdsnc.cn/gtdumiqvcj.html

Ruby: SecureRandom.uuid
来源：http://hz.yuanzhike.top/gtukmtsnlr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.aibaodan.cn/gtjjkdvnwj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.tanke756.top/gteodkvwmo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cashguo.top/gtoryyywvq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenlongwang.top/gtowklgwhz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yonumen.top/gtuyvmpjue.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.vqdsnc.cn/gtwhrnyuzd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dashuyun.cn/gttvizjkbc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuanzx.com/gtvrkkugwc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuanzhike.top/gtywgzuszh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gaohongyu789.top/gtdiixyzyz.html

[P03] 生成短随机字符串
来源：http://hz.smart0.xyz/gtswznqzrm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gtygebqjbp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.haohaochexian.top/gtmrdxtcmq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yongpay.top/gthqomidlr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gttcbmddnq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhengqikj.top/gtecgbhjnk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zdqjudy.top/gtyzhbauaw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yonumen.top/gtfnmvsubf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gtjvflfsjg.html

[P04] 求长度
来源：http://hz.pycfn.com/gtsxlpwetf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zdqjudy.top/gtbvnnpsny.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtrwvmbdye.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtdjnvxuay.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hysaishi.cn/gtunxmkylx.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhoulong.xyz/gtecvoosoa.html

Go:   len(arr);  len(m)
来源：http://hz.nwbrower.top/gtwqoeveta.html

Ruby: x.length;  x.size
来源：http://hz.quarkkingdee.top/gtlfotlfux.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhaomingkeji.xyz/gtxaeovlcz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ppjwa.cn/gtdsvvahsb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuanzx.com/gtarwjkwyc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.cqqwz.cn/gtcmwymcrn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daria6918.cn/gtoibitgai.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenlongwang.top/gtfljmuaga.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258888.top/gthqicvkyu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgfzy.top/gtiaoksssi.html

Ruby: a == b
来源：http://hz.xylfe.cn/gtjxcpmxst.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.tian-w.cn/gtuhvljwng.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.svipenyu.cn/gtpiedirsp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yongpay.top/gtynwzgahb.html

PHP:  if (empty($x)) {}
来源：http://hz.chenlongwang.top/gtfacwnzqg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gaohongyu789.top/gtqplqekhs.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtqfnxfwtn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtehagxbrd.html

Go:   if x == nil {}
来源：http://hz.svipenyu.cn/gtkozgdkgz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jyoumei.cn/gtwadoxccl.html

C#:   if (x is null) {}
来源：http://hz.dashuyun.cn/gtxlgeavao.html

[P07] 防抖与节流
来源：http://hz.hnxiangtu.top/gtuixkzqhp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtuydftkca.html

PHP:  // 手写时间戳比较
来源：http://hz.snrcjt.cn/gtvupumbxb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtrrkinnbp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtvcqbiwza.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangdashe.top/gtftkjevpo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tanke756.top/gtvqldqghk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gtqgingpwt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.birdmap.top/gtxdzuxine.html

[P08] 处理浮点精度问题
来源：http://hz.tian-w.cn/gthrypeaaw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yonumen.top/gtsdnqheap.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhengqikj.top/gtcqpxhdca.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenlongwang.top/gtooekcama.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.feifeiyinyue.top/gtiykcqxxj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinghuilouyu.cn/gtbxgyfrhj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guowangkeji.top/gtqlpwvvft.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.redwolf501.top/gtukvlznst.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtjiqyeikz.html

================================================================================
来源：http://hz.jianghu66.top/gtlbtizjnj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xingfuxueyuan.xyz/gtphamkhoq.html

================================================================================
来源：http://hz.yueranfly.top/gtsynvrjif.html

[Q01] 创建表
来源：http://hz.bjfxy.top/gtdurooold.html

CREATE TABLE users (
来源：http://hz.guowangkeji.top/gtcsebmkki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtsjgbpgll.html

name VARCHAR(50) NOT NULL,
来源：http://hz.feifeiyinyue.top/gtqmscsqwo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhengqikj.top/gtogcnqpao.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtfwbapkfr.html

);
来源：http://hz.gaohongyu789.top/gtjolrfvxh.html

[Q02] 创建带外键的表
来源：http://hz.yueranfly.top/gtajxnblus.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gtrimbywpe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.kuanghao11.cn/gtuskjzhsp.html

user_id INT NOT NULL,
来源：http://hz.zhixingplan.top/gtcavlgwzb.html

amount DECIMAL(10, 2),
来源：http://hz.zhiwuduotai.top/gtnczmrinc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ywan-chungtsiang.top/gtnpngmjno.html

);
来源：http://hz.sxryk.cn/gtjkhqtdwa.html

[Q03] 增加列
来源：http://hz.ydzc1.top/gtziubxjic.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.tian-w.cn/gtnqttbfjm.html

[Q04] 修改列类型
来源：http://hz.redwolf501.top/gtdsrqgjra.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.fengsongda.top/gtouybtkbu.html

[Q05] 重命名列
来源：http://hz.dianchejie.cn/gtavmnzesy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sxryk.cn/gtfddxflkh.html

[Q06] 删除列
来源：http://hz.aibaodan.cn/gtfwuwgvro.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ivvv.top/gtmpbjgaoy.html

[Q07] 删除表
来源：http://hz.chenlongwang.top/gtzzfdyrxe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gtjprnpfvk.html

[Q08] 创建普通索引
来源：http://hz.feifeiyinyue.top/gtwvwqjkxm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xingfuxueyuan.xyz/gtxjxqzcxt.html

[Q09] 创建唯一索引
来源：http://hz.cdnleiting.top/gtexbwfgcf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtrjtwyspj.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gtzwwmbiij.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.0kj1m.cn/gtjbjcxjqb.html

[Q11] 一次插入多行
来源：http://hz.tian-w.cn/gtjktsbswb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnqzz.top/gtbyqacaff.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtkvmeiubz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yvedp.cn/gtfxjwhlxx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gthgrdutuo.html

[Q13] 忽略重复插入
来源：http://hz.hnqzz.top/gtlnpucmxl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhixingplan.top/gtxbffjogl.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtbwikwnpe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tianlin.xyz/gtfncnzsur.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jqgfzy.top/gtjyapsvkl.html

[Q15] 查询全部
来源：http://hz.ywan-chungtsiang.top/gtorjtfpxa.html

SELECT * FROM users;
来源：http://hz.shanyushiyangkeji.top/gtqewhzbyk.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtqppbylta.html

SELECT id, name FROM users;
来源：http://hz.ydzc1.top/gtmxbwrjii.html

[Q17] 条件查询
来源：http://hz.zycfv.cn/gtxszdgvrt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yonumen.top/gtuevkyipv.html

[Q18] 模糊匹配
来源：http://hz.wangshuangyany.cn/gthqycvjth.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinghuilouyu.cn/gtodbdhqcz.html

[Q19] 范围查询
来源：http://hz.jyoumei.cn/gtnrwyunsj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hongshengwenyu.top/gtgncazywx.html

[Q20] IN 列表
来源：http://hz.zycfv.cn/gtxzmfpnee.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenlongwang.top/gtchgupkgh.html

[Q21] 空值判断
来源：http://hz.hfpthk.cn/gtksqnzmpg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gtshisdmim.html

[Q22] 排序
来源：http://hz.smart0.xyz/gtigbpalpc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gtbauyyurn.html

[Q23] 分页
来源：http://hz.chenlongwang.top/gtweyllphp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gtbzfrczxh.html

[Q24] 去重
来源：http://hz.316326.xyz/gtmkhbnquo.html

SELECT DISTINCT city FROM users;
来源：http://hz.316326.xyz/gtwaqkuzfm.html

[Q25] 只取前 N 条
来源：http://hz.daxiang520.top/gtlpuummpg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.shangyingyoupin.top/gtbouvwmka.html

[Q26] 计数
来源：http://hz.jqgufenzy.top/gtfdrfrrem.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhengqikj.top/gtkrskxzzp.html

[Q27] 条件计数
来源：http://hz.havefunace.top/gtkcvaeoie.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhijiandao.cn/gtpymvgsip.html

[Q28] 求和与平均
来源：http://hz.tian-w.cn/gtzvbijath.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gtgpdkvuyv.html

[Q29] 最大最小值
来源：http://hz.xuetiantiany.cn/gtdstpdixj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtjrhzygct.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtgaaxcmrv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yueranfly.top/gtoiapcbkv.html

[Q31] 分组后过滤
来源：http://hz.tianlin.xyz/gtibzqnchc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xuetiantiany.cn/gtgwwrekpi.html

[Q32] 分组拼接字符串
来源：http://hz.yj202588.top/gtfonvegas.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtecvpnoea.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.316326.xyz/gtrsubceri.html

[Q33] 多列分组
来源：http://hz.shanyushiyangkeji.top/gtvnffhlha.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.316326.xyz/gtfemmtrld.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gtazexniir.html

SELECT * FROM (
来源：http://hz.dashuyun.cn/gtaffegrlz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.chenlongwang.top/gtwdcoqudu.html

) t WHERE rn = 1;
来源：http://hz.fengsongda.top/gtaxqringk.html

[Q35] 内连接
来源：http://hz.ybcxt.top/gtkltptuly.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gtqobbmxsr.html

[Q36] 左连接
来源：http://hz.tanke756.top/gtmqvmdxbd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtubnvkqzc.html

[Q37] 右连接
来源：http://hz.havefunace.top/gtzfqzjyqp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtozcybbsj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhengqikj.top/gtezzdawrn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.dashuyun.cn/gtgdjmybtp.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gtbqtfrscp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydzc1.top/gtmyhkpzrj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtmyllopmy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenzaomai.com/gtwdajvhor.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.wangdashe.top/gtvvjtdnmv.html

[Q41] 多表连接
来源：http://hz.yueranfly.top/gtgypgogcm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj202588.top/gtuwaeuwpu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhongyouzk.top/gtzvbrnlkg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenzaomai.com/gtwtpjqqhf.html

[Q42] 连接条件附加过滤
来源：http://hz.sufxvd.cn/gtwuqkitrm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuetiantiany.cn/gthawomaos.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ywan-chungtsiang.top/gtrhuyjobe.html

[Q43] 标量子查询
来源：http://hz.guannengcc.top/gtjvasytuy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gtcwfhtlbh.html

[Q44] IN 子查询
来源：http://hz.aibaodan.cn/gtapblxvke.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hnxiangtu.top/gtrcabthxi.html

[Q45] EXISTS 判断存在
来源：http://hz.zhijiandao.cn/gtkkakjxjy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.mhx1999.top/gtrwuhonqr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ppjwa.cn/gtuhxlandn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtgespxovr.html

[Q47] 与平均值比较
来源：http://hz.dashuyun.cn/gtfobgspfl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xziqi.cn/gttrllggww.html

[Q48] CTE 公用表表达式
来源：http://hz.vqdsnc.cn/gtifhxgcvd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gttxljrvmz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aizwys.cn/gttbfkncxp.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtaduqqhhw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtklmzjvqt.html

[Q50] 批量更新
来源：http://hz.guannengcc.top/gtxnjjpexo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtydfejffd.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtukbppxug.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.0kj1m.cn/gtelzfbqdp.html

[Q52] 删除指定行
来源：http://hz.gzhubu.top/gtfzbbxqlg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zdqjudy.top/gtleekewoo.html

[Q53] 按条件删除
来源：http://hz.vqdsnc.cn/gtemrjbfcq.html


<!-- 参考信息 -->