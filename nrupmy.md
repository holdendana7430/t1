代发 wailian999

Java: // 手写回溯递归
来源：http://hz.meibo888.top/gtpgshgrcz.html

Go:   // 手写回溯递归
来源：http://hz.cdnleiting.top/gtqkwplbek.html

Ruby: arr.permutation.to_a
来源：http://hz.fzhhl.top/gtwdstrfqd.html

C#:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtfhqwukvl.html

[N09] 栈与队列
来源：http://hz.gotoacloud.top/gtkrztncvb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtbjjisozd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gtskqzmgng.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtbdknxarv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gotoacloud.top/gtmamkwhvw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.haohaochexian.top/gtwhqxpxlo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenlongwang.top/gtkwmgmaqg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cashguo.top/gtljihkokz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tian-w.cn/gtkhvtoszf.html

[N10] 链表节点定义
来源：http://hz.jyoumei.cn/gthnaknfnz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gtzyhxuggn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuxming.cn/gttjzhacdq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtnytmleen.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxuanxn.top/gtduiyysst.html

Java: class Node { int v; Node next; }
来源：http://hz.redwolf501.top/gttfifgytx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sweek.top/gtkecehgyu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangshuangyany.cn/gtpijvsgxg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.daxiang520.top/gtvjoohckz.html

[N11] 二叉树中序遍历
来源：http://hz.ehwqpu.com/gtzfbfkrth.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj202588.top/gtpwvjtdum.html

PHP:  // 手写递归函数
来源：http://hz.yj20258888.top/gtecegnifa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtxepddykl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtvcyxfvbl.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gttbszvutl.html

Go:   // 手写递归
来源：http://hz.0kj1m.cn/gttxxyulwg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258.top/gtacccyvlj.html

C#:   // 手写递归
来源：http://hz.meibo888.top/gtjrjpqkst.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.316326.xyz/gtccferyag.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtwxcojbtj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jiagoushi.top/gtdwisrldv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtsoueqfdr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guannengcc.top/gtvzvpmrbt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtujryxspz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhoulong.xyz/gttyaszxge.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxuanxn.top/gtyilydeom.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtnhpkefrj.html

================================================================================
来源：http://hz.ydzc1.top/gtslzwxqpd.html

O. 并发与异步
来源：http://hz.yuanzhike.top/gtbkrpazse.html

================================================================================
来源：http://hz.yuxming.cn/gtlczcpnto.html

[O01] 启动一个线程
来源：http://hz.cheryme.top/gtixpwlgtv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuanzhike.top/gtstdwjlzp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtaffmilxt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.redwolf501.top/gtxhjomdcy.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtzugfbiiy.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenlongwang.top/gtzfdzczsx.html

Go:   go f()
来源：http://hz.chenjidiqi.icu/gtmqkejitg.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtdczameao.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gthneewijb.html

[O02] 使用线程池
来源：http://hz.hongshengwenyu.top/gtatjjwmlz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.haohaochexian.top/gtzlgzthbm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.iojbl.cn/gtzvibcdiv.html

JS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtloterwqg.html

TS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gtlxifptqy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.birdmap.top/gthtryayut.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhongyouzk.top/gtbabjdugb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gthohpcfkr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hnxiangtu.top/gtxwjzmkar.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gttwrcgplx.html

Py:   with lock: shared += 1
来源：http://hz.cqqwz.cn/gtfkblxjsj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cheryme.top/gtbybgaiuf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xingfuxueyuan.xyz/gtkvozsyvx.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gthwbdifzp.html

Java: synchronized (this) { shared++; }
来源：http://hz.daria6918.cn/gtpecewmmr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtfmpvcvgo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtaonrcxyg.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtzimxkejk.html

[O04] 定义异步函数并等待
来源：http://hz.jianghu66.top/gtpuctuewq.html

Py:   async def f():⏎    await g()
来源：http://hz.birdmap.top/gtdmigjqfv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gtfpodotuy.html

JS:   async function f() { await g(); }
来源：http://hz.yvedp.cn/gtpgteiger.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sweek.top/gtdrsqoxnl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zdqjudy.top/gtraxlelre.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.redwolf501.top/gtijsgnwyw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.smart0.xyz/gtygpwcpyy.html

C#:   async Task F() { await G(); }
来源：http://hz.ydjk.org.cn/gtfgvbmzwh.html

[O05] 并发执行并等待全部完成
来源：http://hz.jyoumei.cn/gtjrwjqcby.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhixingplan.top/gtefrgrxph.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinyuanbaomall.cn/gtkcthzeak.html

JS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtdbfegrdr.html

TS:   await Promise.all(tasks)
来源：http://hz.ydjk.org.cn/gtakzqlimm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fzhhl.top/gtszmjfgpl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtyifwqmyw.html

Ruby: threads.map(&:join)
来源：http://hz.tanke756.top/gtvrcjvusr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cheryme.top/gtiwwzaepo.html

[O06] 使用进程池
来源：http://hz.jqgfzy.top/gtfvedebgj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xylfe.cn/gtnhsdygpf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jiagoushi.top/gtbsyykbzf.html

JS:   // child_process / cluster 模块
来源：http://hz.zhengqikj.top/gtmobvirem.html

TS:   // child_process / cluster 模块
来源：http://hz.gotoacloud.top/gtdqwddbvi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.9152youxi.cn/gtcplqvvmb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangkeji.top/gtlebxpoov.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gtxoowxobu.html

C#:   Parallel.For
来源：http://hz.ywan-chungtsiang.top/gtyykesgwo.html

================================================================================
来源：http://hz.havefunace.top/gtqtevsqvv.html

P. 常用工具函数
来源：http://hz.ivvv.top/gtysjqphwd.html

================================================================================
来源：http://hz.mhx1999.top/gtxxzmxpjw.html

[P01] 生成 UUID
来源：http://hz.yonumen.top/gtaaeethna.html

Py:   str(uuid.uuid4())
来源：http://hz.zhengqikj.top/gtupgpkpqi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shuidangran.top/gtkpeaokwi.html

JS:   crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtbdgenxng.html

TS:   crypto.randomUUID()
来源：http://hz.hfpthk.cn/gtntrxwiso.html

Java: UUID.randomUUID().toString()
来源：http://hz.shuidangran.top/gtyrvgwjad.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aibaodan.cn/gtmathgjda.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtwxjldgdo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.birdmap.top/gtnfwnutam.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtpulrjvsv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aibaodan.cn/gtlmezskgm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenzaomai.com/gtoaddvjxj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hammf.cn/gtlnzonmnc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gtrqitgbni.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenlongwang.top/gtfkejdawj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shzxlz.cn/gtmavpyegy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtxgbxpokx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nwbrower.top/gtmtmzqtkj.html

[P03] 生成短随机字符串
来源：http://hz.pycfn.com/gtdsfuvghb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.kuanghao11.cn/gtjshsxegf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yuanzhike.top/gtkujpobzt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.iojbl.cn/gtwntdetqv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtlgxqcqzk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenjidiqi.icu/gttgbdqmyt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ehwqpu.com/gtzjwrhryp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.svipenyu.cn/gtfmjkopbt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuanzx.com/gtrlnnduoa.html

[P04] 求长度
来源：http://hz.jinqigfzy.top/gthaclwgbv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.smart0.xyz/gttcxfsole.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtuqaowemq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtoqaitzya.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtvxyqxveo.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daxiang520.top/gtkeznzdzc.html

Go:   len(arr);  len(m)
来源：http://hz.daxiang520.top/gtjdtqoivu.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtaddlgwrr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtmutofama.html

[P05] 判断两个对象内容是否相等
来源：http://hz.havefunace.top/gtroywtrds.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hysaishi.cn/gtntiezfnv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gtatioaauq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hongshengwenyu.top/gtcxhtoxhx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.svipenyu.cn/gtcpbedqpe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnqzz.top/gtpqgkphoy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tianlin.xyz/gtkjnvplum.html

Ruby: a == b
来源：http://hz.hammf.cn/gtqedrsdlt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yangfankeji.com/gtognytqkk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hfpthk.cn/gtpcdvtnsf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yangfankeji.com/gtvdfxsowr.html

PHP:  if (empty($x)) {}
来源：http://hz.aizwys.cn/gtevdfbokr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gzhubu.top/gtsqrhkjsq.html

TS:   if (x == null) {}
来源：http://hz.yanxiufei.cn/gtrqcihape.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sysykeji.top/gtcycocsxq.html

Go:   if x == nil {}
来源：http://hz.xuetiantiany.cn/gtpxbmfcue.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.andypj.xyz/gtlwexzksh.html

C#:   if (x is null) {}
来源：http://hz.tanke756.top/gtlvlfcqfe.html

[P07] 防抖与节流
来源：http://hz.bjfxy.top/gtyzsjmrpc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.quarkkingdee.top/gtevowhzjy.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gtmtvkbnpq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gotoacloud.top/gtekzpgsfn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gtmsfvhvpc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj20258888.top/gtuaerscmv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhixingplan.top/gtozehekoq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cdnleiting.top/gtlegasetk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangshuangyany.cn/gttgwynmfn.html

[P08] 处理浮点精度问题
来源：http://hz.yj202588.top/gtvnwajncd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ehwqpu.com/gtiejgdlhg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gaohongyu789.top/gtvoemftdz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gtabrrrzfv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgfzy.top/gtjkvygbrr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangshuangyany.cn/gtnsfrqige.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nwbrower.top/gtvzcwpxbe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.kuanghao11.cn/gtxhrctndp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xziqi.cn/gtezpivyif.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxmbqbede.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yueranfly.top/gtrqecvbxq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtkuwemgxx.html

[Q01] 创建表
来源：http://hz.wangshuangyany.cn/gtitrewybx.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtedowyixd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gtlemmyvov.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gtorypgtdp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hfpthk.cn/gtnlerauin.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sysykeji.top/gtcatldqvu.html

);
来源：http://hz.0kj1m.cn/gtzgosjokv.html

[Q02] 创建带外键的表
来源：http://hz.wangshuangyany.cn/gtdtesxacu.html

CREATE TABLE orders (
来源：http://hz.hnxiangtu.top/gtqljtgynn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gtkuvurmgn.html

user_id INT NOT NULL,
来源：http://hz.wangdashe.top/gtkbunleni.html

amount DECIMAL(10, 2),
来源：http://hz.guannengcc.top/gtyghilcqz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.kuanghao11.cn/gtzzzyshdk.html

);
来源：http://hz.jyoumei.cn/gtqvsxxghy.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtqzrfvryc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nanxuanxn.top/gttsiakhqq.html

[Q04] 修改列类型
来源：http://hz.jqgufenzy.top/gtvdmmgzmi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tanke756.top/gtguowiaig.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtegyebfgl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtyuuevlod.html

[Q06] 删除列
来源：http://hz.zhoulong.xyz/gtszjahidv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fzhhl.top/gtpyzzhfvl.html

[Q07] 删除表
来源：http://hz.redwolf501.top/gtujleibnh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zdqjudy.top/gtgcepujbx.html

[Q08] 创建普通索引
来源：http://hz.shzxlz.cn/gtftvnipkc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tianlin.xyz/gtlwpkxllv.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gtmdiiysur.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.iojbl.cn/gtrbypfvzi.html

[Q10] 插入单行
来源：http://hz.aizwys.cn/gtksgmhqoo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ybcxt.top/gtfqfwnxlk.html

[Q11] 一次插入多行
来源：http://hz.ywan-chungtsiang.top/gtwkteiwcq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yonumen.top/gtqrywvvld.html

[Q12] 插入后取自增 ID
来源：http://hz.cdnleiting.top/gtcygjdxht.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sysykeji.top/gtilbdhmtp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhongyouzk.top/gtaxkxoeok.html

[Q13] 忽略重复插入
来源：http://hz.snrcjt.cn/gtttllxgwg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nwbrower.top/gtgmivxawc.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtdmkkrfeh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cdnleiting.top/gtokmegjtu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ydjk.org.cn/gtpinyfmdx.html

[Q15] 查询全部
来源：http://hz.guowangkeji.top/gtjuhtpjfy.html

SELECT * FROM users;
来源：http://hz.xinyue.icu/gtcwudokja.html

[Q16] 查询指定列
来源：http://hz.shzxlz.cn/gtjqciscdh.html

SELECT id, name FROM users;
来源：http://hz.hnxiangtu.top/gtchfhelbj.html

[Q17] 条件查询
来源：http://hz.smart0.xyz/gtuivpcora.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gtzjeliyxd.html

[Q18] 模糊匹配
来源：http://hz.fzhhl.top/gtcgjkqvpk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.smart0.xyz/gtduthtowe.html

[Q19] 范围查询
来源：http://hz.meibo888.top/gtxqnvtkly.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenzaomai.com/gtfevnyovn.html

[Q20] IN 列表
来源：http://hz.daria6918.cn/gtoqyvbddp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.iojbl.cn/gtumqxnlos.html

[Q21] 空值判断
来源：http://hz.aibaodan.cn/gtjwfxmoxi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sysykeji.top/gtkwxbghgk.html

[Q22] 排序
来源：http://hz.yuxming.cn/gtykyjiqpl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangtech.top/gticelvgfm.html

[Q23] 分页
来源：http://hz.kuanghao11.cn/gtdjpykjcy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gthsfwrcfx.html

[Q24] 去重
来源：http://hz.zhoulong.xyz/gtcjqhdwge.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydjk.org.cn/gtplhocauk.html

[Q25] 只取前 N 条
来源：http://hz.jlsjyb.cn/gtyouyqykw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.316326.xyz/gtsymbykmo.html

[Q26] 计数
来源：http://hz.xinyue.icu/gtifxdespl.html

SELECT COUNT(*) FROM users;
来源：http://hz.gzhubu.top/gtvsuthpsn.html

[Q27] 条件计数
来源：http://hz.sufxvd.cn/gtgamlisyo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangdashe.top/gtucnktznv.html

[Q28] 求和与平均
来源：http://hz.cheryme.top/gtefofkgax.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtldzyrphl.html

[Q29] 最大最小值
来源：http://hz.fzhhl.top/gtsbbocgzz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sweek.top/gtbhniltbd.html

[Q30] 分组统计
来源：http://hz.nanxuanxn.top/gtmlaqilev.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtsdtrnvqt.html

[Q31] 分组后过滤
来源：http://hz.xziqi.cn/gtzmotkbzl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hammf.cn/gtqgcujsdn.html

[Q32] 分组拼接字符串
来源：http://hz.yanxiufei.cn/gtregrweht.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtkuqtyjtp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.smart0.xyz/gtxboafykx.html

[Q33] 多列分组
来源：http://hz.hfpthk.cn/gtrlelbagf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hongshengwenyu.top/gtvfhhgzbq.html

[Q34] 每组取第一条
来源：http://hz.cashguo.top/gtmzethpvw.html

SELECT * FROM (
来源：http://hz.sysykeji.top/gttafmdoxu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gotoacloud.top/gthtkwdhim.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtflfjubsc.html

[Q35] 内连接
来源：http://hz.zhijiandao.cn/gtwpermyxr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtagurdqeu.html

[Q36] 左连接
来源：http://hz.yuanzhike.top/gthzfwqfnx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ehwqpu.com/gtvhtugtvi.html

[Q37] 右连接
来源：http://hz.chenjidiqi.icu/gthlkeuzzh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.9152youxi.cn/gtxzfjqtdp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtnwgtgygg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tianlin.xyz/gtmyaykvra.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gtvjxzytnr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ivvv.top/gtooekhkbf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cucudq.cn/gtououcozc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.9152youxi.cn/gtsvnnhyxs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gtsqejokvv.html

[Q41] 多表连接
来源：http://hz.redwolf501.top/gtqvdlycfk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pengpengdd.cyou/gtpxiyvvsb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtbokkcmwk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.svipenyu.cn/gtdkpeswmf.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtbbacehvc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xziqi.cn/gthfpngoit.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtfjihkssb.html

[Q43] 标量子查询
来源：http://hz.hnxiangtu.top/gteuclpwex.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtawwyauwi.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtuvcodteb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gtdvvgzzep.html

[Q45] EXISTS 判断存在
来源：http://hz.zhongyouzk.top/gtyvagurdx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtjesxmdbb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hywenlv.cn/gtfinwname.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtjjelbeoz.html

[Q47] 与平均值比较
来源：http://hz.iojbl.cn/gtlbnevziz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtgaswnzck.html

[Q48] CTE 公用表表达式
来源：http://hz.gzhubu.top/gtmrxfnwdr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinghuilouyu.cn/gtvxvbkbhw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cqqwz.cn/gtmdiwdxzt.html

[Q49] 更新单行
来源：http://hz.tianlin.xyz/gtagzufbrw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtjypnjtcs.html

[Q50] 批量更新
来源：http://hz.tian-w.cn/gtfzjvofjx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtiuqciilc.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtreeoycvr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhoulong.xyz/gtkfwnjnkd.html

[Q52] 删除指定行
来源：http://hz.chenjidiqi.icu/gtymtlsgmg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.iojbl.cn/gtvnaxcgfe.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gtgtwzkeiw.html


<!-- 参考信息 -->