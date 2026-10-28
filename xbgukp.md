代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hz.feifeiyinyue.top/gtxuyjitkb.html

PHP:  // 手写递归交换
来源：http://hz.iojbl.cn/gtnqawaroz.html

JS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gttshqueua.html

TS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtwaiegddg.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtyzwmigag.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtdmkwosht.html

Ruby: arr.permutation.to_a
来源：http://hz.jianghu66.top/gtzjhjlclf.html

C#:   // 手写回溯递归
来源：http://hz.ivvv.top/gtposksxmg.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtdcovrthu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangkeji.top/gtawbxfvsr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cheryme.top/gtfwittstg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hysaishi.cn/gtyiuavmmu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenjidiqi.icu/gtzbayqprh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtvjmidmgq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.smart0.xyz/gtcevzdkiu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj202588.top/gtmhznkjev.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ywan-chungtsiang.top/gttxuhrzlg.html

[N10] 链表节点定义
来源：http://hz.yj202588.top/gtfzqfypgv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.vqdsnc.cn/gtqfzvbnqf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtrxfyiehb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xinyue.icu/gtkjueydxx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yuanzhike.top/gtamhnodlk.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangkeji.top/gtuogyztez.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ivvv.top/gtpaxtzgsy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtswhpsepr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtsdjfiofq.html

[N11] 二叉树中序遍历
来源：http://hz.fzhhl.top/gtmdaqmuzl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hnqzz.top/gttyeykzra.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtmzpwndll.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtpnffsqxe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gttzsfxoot.html

Java: // 手写递归
来源：http://hz.c1oappe.top/gtmmgzaahg.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtlemyzqec.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtvpaxhrax.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gtajfocebp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.aibaodan.cn/gthbowcjtr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtgnzvufnf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.redwolf501.top/gthcaskhan.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtpyrpgfnv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtlvrfjwde.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.9152youxi.cn/gttjyzoiil.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jiagoushi.top/gtnhkijcmi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.kuanghao11.cn/gtrlckditn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gteduykafg.html

================================================================================
来源：http://hz.yanxiufei.cn/gtmeuyomfw.html

O. 并发与异步
来源：http://hz.aibaodan.cn/gtorjddtlx.html

================================================================================
来源：http://hz.zhoulong.xyz/gtiknfizne.html

[O01] 启动一个线程
来源：http://hz.yuanzhike.top/gtllzealsl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtfgzmzpkj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cucudq.cn/gtdgcxgpgs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigufen.top/gtltvacsld.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtblhefhmd.html

Java: new Thread(() -> f()).start()
来源：http://hz.hongshengwenyu.top/gtiwmmwtnv.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtyyzsuljg.html

Ruby: Thread.new { f }
来源：http://hz.gaohongyu789.top/gtutgkuscm.html

C#:   Task.Run(() => F());
来源：http://hz.zhixingplan.top/gtstokuavx.html

[O02] 使用线程池
来源：http://hz.zhaomingkeji.xyz/gthqrchbym.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xingfuxueyuan.xyz/gtytdlcxzf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yangfankeji.com/gttavoofum.html

JS:   // worker_threads 线程池
来源：http://hz.hammf.cn/gtyykeqhsa.html

TS:   // worker_threads 线程池
来源：http://hz.nanxuanxn.top/gtgypuiqad.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yvedp.cn/gtcowfhfdx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.0kj1m.cn/gtejgyanyg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gtjttgvwss.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ppjwa.cn/gtochcwhcq.html

[O03] 加锁保护共享数据
来源：http://hz.jiagoushi.top/gtpzepalvw.html

Py:   with lock: shared += 1
来源：http://hz.nwbrower.top/gtpzgwpjum.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtmbnyoxqa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgfzy.top/gtidinctit.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtokknskps.html

Java: synchronized (this) { shared++; }
来源：http://hz.xziqi.cn/gtcslsndcc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gttjgipwuq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ehwqpu.com/gtrvautqqq.html

C#:   lock (gate) { shared++; }
来源：http://hz.aizwys.cn/gtdyefyfvq.html

[O04] 定义异步函数并等待
来源：http://hz.jqgfzy.top/gtqvonrmzv.html

Py:   async def f():⏎    await g()
来源：http://hz.wangdashe.top/gtquafnivq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jlsjyb.cn/gthppwiyzb.html

JS:   async function f() { await g(); }
来源：http://hz.jyoumei.cn/gtcbxpkjoy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgufenzy.top/gtlngzvnbh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hongshengwenyu.top/gtkylnjjxe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtmaxqlzeo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinghuilouyu.cn/gtihogvdip.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtickvnjxc.html

[O05] 并发执行并等待全部完成
来源：http://hz.sweek.top/gtpntepurg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yueranfly.top/gtqnhjllsg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.feifeiyinyue.top/gtdkihqfhb.html

JS:   await Promise.all(tasks)
来源：http://hz.xuetiantiany.cn/gtpjskmjpi.html

TS:   await Promise.all(tasks)
来源：http://hz.chenlongwang.top/gtzsfpwvtj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuetiantiany.cn/gtpikprmec.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shuidangran.top/gtxgnfkjwg.html

Ruby: threads.map(&:join)
来源：http://hz.9152youxi.cn/gtfiexwnic.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xingfuxueyuan.xyz/gtedibtuoy.html

[O06] 使用进程池
来源：http://hz.jyoumei.cn/gtolwhzhex.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gtkbjyqrbw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hfpthk.cn/gtabblkhfh.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtwtgzfbyn.html

TS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gtofvflwgo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jyoumei.cn/gtgmnfvbgy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daxiang520.top/gtudzwptoj.html

Ruby: // fork 块
来源：http://hz.yj20258888.top/gthbjanjla.html

C#:   Parallel.For
来源：http://hz.havefunace.top/gtwehlbehk.html

================================================================================
来源：http://hz.snrcjt.cn/gtridgbipn.html

P. 常用工具函数
来源：http://hz.yj20258888.top/gtmhglwtwz.html

================================================================================
来源：http://hz.jiagoushi.top/gtvnyshzdm.html

[P01] 生成 UUID
来源：http://hz.fzhhl.top/gtdgczwknf.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtlhmouapf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gzhubu.top/gthvoneahq.html

JS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gttsgmxzqd.html

TS:   crypto.randomUUID()
来源：http://hz.hammf.cn/gtcdmbmyxw.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtmrhyomda.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cdnleiting.top/gtubkovjsk.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtjclwqiic.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gtyhicazse.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cheryme.top/gtbekifpii.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinqigufen.top/gtfiqmwvka.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.fzhhl.top/gtfqxrjcfu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yvedp.cn/gtvohuvcgy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xuanzx.com/gtxkeubwfd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hywenlv.cn/gtrbtvqsvx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhoulong.xyz/gtzbuwnwnl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gthzhksbgl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhiwuduotai.top/gtyxgdmqkj.html

[P03] 生成短随机字符串
来源：http://hz.9152youxi.cn/gtzdpatzom.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuetiantiany.cn/gtszzwmjpw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenlongwang.top/gtskxqtjpc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtnsqbxdlr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtmlgfdism.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ybcxt.top/gtcgjjmiyz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.snrcjt.cn/gtzufpwqym.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shuidangran.top/gteowibxar.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jyoumei.cn/gtxubaqlqh.html

[P04] 求长度
来源：http://hz.c1oappe.top/gtnbualcfi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ehwqpu.com/gtlbkptdhy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gterepzizu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtosindtbi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenzaomai.com/gtkuffetnv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj202588.top/gtlkzkdvyc.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtnyzlzpvu.html

Ruby: x.length;  x.size
来源：http://hz.0kj1m.cn/gttkejuhuc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jianghu66.top/gtwgvcykaz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.redwolf501.top/gtwjicbpgu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tanke756.top/gtqtohlfbp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sweek.top/gtsflpwdwr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hfpthk.cn/gtojscgavt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ydjk.org.cn/gtdeznkutu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.guowangkeji.top/gtgwylkwvf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gtfqbgiiqv.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtcdgzeoaz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gteccgzrpb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.birdmap.top/gtfqkcrlmc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxinkj.top/gtsiidrfsl.html

PHP:  if (empty($x)) {}
来源：http://hz.gotoacloud.top/gtvhzpxudz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.dianchejie.cn/gtwpgcddwu.html

TS:   if (x == null) {}
来源：http://hz.xylfe.cn/gtillszybq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.snrcjt.cn/gtssiohinp.html

Go:   if x == nil {}
来源：http://hz.316326.xyz/gtytesesgo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hysaishi.cn/gtmelzxozd.html

C#:   if (x is null) {}
来源：http://hz.wangshuangyany.cn/gtshpnjltb.html

[P07] 防抖与节流
来源：http://hz.jinqigufen.top/gtnvqkitxw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hfpthk.cn/gtfjchfbvf.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtxchofqmr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtrorwyozf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gticdovnjj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxuanxn.top/gtypkaycwj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gtfyeuldgk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhongyouzk.top/gtyvvgibau.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtmdizkrcp.html

[P08] 处理浮点精度问题
来源：http://hz.bjfxy.top/gtegdqplih.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.smart0.xyz/gtnypdznxd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cqqwz.cn/gtwiizujfl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yangfankeji.com/gtgbrtvrpo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ybcxt.top/gtjfiefuwn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ehwqpu.com/gtwwwcklat.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258888.top/gtaqsqljme.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jyoumei.cn/gtftdlmnsz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtlqzzarzs.html

================================================================================
来源：http://hz.yangfankeji.com/gtwicbvpis.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.redwolf501.top/gtzakoqheo.html

================================================================================
来源：http://hz.guannengcc.top/gtcxixtvhc.html

[Q01] 创建表
来源：http://hz.birdmap.top/gtslqzvqec.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtjsvhzpvi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtxxxtspqh.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenjidiqi.icu/gtqzlhewzf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnqzz.top/gtsvciudnc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.c1oappe.top/gtwhvntzyb.html

);
来源：http://hz.zhiwuduotai.top/gtqbzfjkij.html

[Q02] 创建带外键的表
来源：http://hz.yuanzhike.top/gtqqsywbzd.html

CREATE TABLE orders (
来源：http://hz.tianlin.xyz/gttgaxobiq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtyxenbhmy.html

user_id INT NOT NULL,
来源：http://hz.kuanghao11.cn/gttldhmgzn.html

amount DECIMAL(10, 2),
来源：http://hz.feifeiyinyue.top/gtcgtvgbho.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cucudq.cn/gtaelwwgtd.html

);
来源：http://hz.yonumen.top/gtuynbqurq.html

[Q03] 增加列
来源：http://hz.zhengqikj.top/gtcmleevhe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fengsongda.top/gthqwrvuwq.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtzhvmuvwm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtydqygjvp.html

[Q05] 重命名列
来源：http://hz.sufxvd.cn/gticaplahz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hnqzz.top/gtsihwhblp.html

[Q06] 删除列
来源：http://hz.nanxinkj.top/gtkwtfwjlg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxinkj.top/gtsfpdsmpo.html

[Q07] 删除表
来源：http://hz.sufxvd.cn/gtqnhbdwdn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gtnlrhqlkv.html

[Q08] 创建普通索引
来源：http://hz.xuanzx.com/gtyzkdcykw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hammf.cn/gtbobakppc.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtysmimjkk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.52xcode.cn/gtuznnigtw.html

[Q10] 插入单行
来源：http://hz.dianchejie.cn/gtyrdhtiig.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigfzy.top/gtdoaajjlh.html

[Q11] 一次插入多行
来源：http://hz.sufxvd.cn/gtffdrtnoh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtfzxctaik.html

[Q12] 插入后取自增 ID
来源：http://hz.fengsongda.top/gtbzooubay.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gtoobkbhco.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jiagoushi.top/gtawclntta.html

[Q13] 忽略重复插入
来源：http://hz.yj20258888.top/gtequzcpku.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.0kj1m.cn/gtroiclbeo.html

[Q14] 存在则更新（upsert）
来源：http://hz.nanxuanxn.top/gtxwglobaz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yvedp.cn/gtephetyyd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hywenlv.cn/gtznniszoj.html

[Q15] 查询全部
来源：http://hz.hywenlv.cn/gtjxiqsmzq.html

SELECT * FROM users;
来源：http://hz.hammf.cn/gtcgjdhfud.html

[Q16] 查询指定列
来源：http://hz.cashguo.top/gtijcvgwqr.html

SELECT id, name FROM users;
来源：http://hz.chenzaomai.com/gtfsrdawgv.html

[Q17] 条件查询
来源：http://hz.chenzaomai.com/gtriqalckt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shzxlz.cn/gtwkfrhjey.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gtmjomlezu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.feifeiyinyue.top/gtdkolplbf.html

[Q19] 范围查询
来源：http://hz.ppjwa.cn/gtrkuddxtr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ehwqpu.com/gtkywasska.html

[Q20] IN 列表
来源：http://hz.yueranfly.top/gtbtpwlsig.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.redwolf501.top/gtjoxjeszy.html

[Q21] 空值判断
来源：http://hz.yuxming.cn/gteghachfc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhijiandao.cn/gtnrouakez.html

[Q22] 排序
来源：http://hz.zhixingplan.top/gtbqgqqupe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.havefunace.top/gtkztvrthq.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtordbtgvx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.smart0.xyz/gthxawskvh.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtcigvzqse.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydjk.org.cn/gtecggkdtc.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtkcfowpwl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj202588.top/gtueepaput.html

[Q26] 计数
来源：http://hz.hongshengwenyu.top/gtzhouvowa.html

SELECT COUNT(*) FROM users;
来源：http://hz.nanxuanxn.top/gtduvtadiq.html

[Q27] 条件计数
来源：http://hz.cdnleiting.top/gtcgfnpznr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ydjk.org.cn/gtascdskoa.html

[Q28] 求和与平均
来源：http://hz.nanxinkj.top/gtlgmhypav.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yueranfly.top/gttvxifclj.html

[Q29] 最大最小值
来源：http://hz.ppjwa.cn/gtlkgzpkqm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.gotoacloud.top/gtexbopfrz.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gtjmfbmmac.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtcndhtrgn.html

[Q31] 分组后过滤
来源：http://hz.jinqigfzy.top/gtbeowwtqd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cheryme.top/gtpovqxuhu.html

[Q32] 分组拼接字符串
来源：http://hz.yangfankeji.com/gtfczkkvqc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jiagoushi.top/gtphdguipo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtwkbuhqgk.html

[Q33] 多列分组
来源：http://hz.pycfn.com/gtirhuelzd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.mhx1999.top/gttusvnwzh.html

[Q34] 每组取第一条
来源：http://hz.zhengqikj.top/gtygqweert.html

SELECT * FROM (
来源：http://hz.zhiwuduotai.top/gtreodrytp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jlsjyb.cn/gtjfqunqjb.html

) t WHERE rn = 1;
来源：http://hz.snrcjt.cn/gthazspyje.html

[Q35] 内连接
来源：http://hz.dashuyun.cn/gtjjdqnmul.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xinyue.icu/gtxkiwsqwz.html

[Q36] 左连接
来源：http://hz.shuidangran.top/gttqbajpnj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tianlin.xyz/gtbaxetklq.html

[Q37] 右连接
来源：http://hz.cucudq.cn/gtrmuixkev.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jinghuilouyu.cn/gtqxfjapui.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.andypj.xyz/gtnnyaretk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pengpengdd.cyou/gtcobvrzye.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtsgeijbai.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtwnazclqu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtzkvhddnj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.smart0.xyz/gtmrwifhhm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guowangkeji.top/gturddkhfq.html

[Q41] 多表连接
来源：http://hz.yuxming.cn/gtjvlewvfg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yonumen.top/gtrozvafro.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnxiangtu.top/gthxwivbva.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gtcvwbwxci.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtephydufq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yongpay.top/gthzusixwj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nwbrower.top/gtkzkxpwgt.html

[Q43] 标量子查询
来源：http://hz.zhixingplan.top/gtgsvapvnk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gttbxevowe.html

[Q44] IN 子查询
来源：http://hz.feifeiyinyue.top/gtjadsbhdm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yonumen.top/gtdweejanm.html

[Q45] EXISTS 判断存在
来源：http://hz.9152youxi.cn/gtuzkwhkid.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtykmppzyt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.kuanghao11.cn/gtsitdzfcc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.redwolf501.top/gtfgfdtmmf.html

[Q47] 与平均值比较
来源：http://hz.sufxvd.cn/gttoumarje.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.guowangkeji.top/gtcvewydjd.html

[Q48] CTE 公用表表达式
来源：http://hz.ppjwa.cn/gtbqnwvlkt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.9152youxi.cn/gtcwbkhqki.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtnemxthdv.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gttoriucfx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fengsongda.top/gteybkwzjd.html

[Q50] 批量更新
来源：http://hz.zhiwuduotai.top/gtvvytinkk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tanke756.top/gthvffqnjm.html

[Q51] 用子查询更新
来源：http://hz.aibaodan.cn/gtmtkjjscf.html


<!-- 参考信息 -->