代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtnxhuhula.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sufxvd.cn/gtfaprynrn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuxming.cn/gtrrhymhun.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258888.top/gtmahppkxp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinyuanbaomall.cn/gtmdkqduhb.html

[N10] 链表节点定义
来源：http://hz.hfpthk.cn/gtlefteceg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.smart0.xyz/gtjvrzfbaf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtihhxyomw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gzhubu.top/gtncjrfzyo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtmoilykyh.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtzfwpdiny.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ybcxt.top/gtveghvzvu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yueranfly.top/gthgkvhtod.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aizwys.cn/gtcfzgxjvv.html

[N11] 二叉树中序遍历
来源：http://hz.fzhhl.top/gtyamhtkjz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hfpthk.cn/gtglynjtcx.html

PHP:  // 手写递归函数
来源：http://hz.jqgufenzy.top/gtclcbrvmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aizwys.cn/gtyzpiobew.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.iojbl.cn/gtmohtxumw.html

Java: // 手写递归
来源：http://hz.xinyue.icu/gtyxcowtus.html

Go:   // 手写递归
来源：http://hz.dianchejie.cn/gtlvvtiwhu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dianchejie.cn/gtofqxdqce.html

C#:   // 手写递归
来源：http://hz.guannengcc.top/gtddbfrdjh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cqqwz.cn/gtczpgbaes.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sufxvd.cn/gtozfmkhlb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cucudq.cn/gtietwgggs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtjdxnugpe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtkborhitk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.c1oappe.top/gtconkuxmi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yongpay.top/gtfnhbmcro.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yanxiufei.cn/gthqxyqsqp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangtech.top/gtatxioacp.html

================================================================================
来源：http://hz.gzhubu.top/gtbrxexeos.html

O. 并发与异步
来源：http://hz.shanyushiyangkeji.top/gtpkkmezgm.html

================================================================================
来源：http://hz.yj202588.top/gtqvpmfrxa.html

[O01] 启动一个线程
来源：http://hz.shanyushiyangtech.top/gtilmohtie.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.52xcode.cn/gtlkhlgguq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ywan-chungtsiang.top/gtkdumojim.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtamlnqiqv.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtphoxiriy.html

Java: new Thread(() -> f()).start()
来源：http://hz.bjfxy.top/gttgibcbxg.html

Go:   go f()
来源：http://hz.hysaishi.cn/gtbsmiuknq.html

Ruby: Thread.new { f }
来源：http://hz.cqqwz.cn/gtwizrmkhu.html

C#:   Task.Run(() => F());
来源：http://hz.tanke756.top/gtjfcuhmje.html

[O02] 使用线程池
来源：http://hz.ehwqpu.com/gtqkkzjvcu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sysykeji.top/gtymeqilnx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dianchejie.cn/gtunlgsloh.html

JS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtplxaxewk.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtyxbjhznd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jianghu66.top/gtgpmvndow.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cucudq.cn/gtdczesawn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydjk.org.cn/gtxmxhxhni.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yangfankeji.com/gtmynqleji.html

[O03] 加锁保护共享数据
来源：http://hz.jqgufenzy.top/gtwlemqpbx.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtlpzbpnvk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtnjtukwwj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.52xcode.cn/gtyziunxar.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gttiqiglqw.html

Java: synchronized (this) { shared++; }
来源：http://hz.guannengcc.top/gtoaqqjcrm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj202588.top/gtjepnjwyr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxinkj.top/gtxanoguba.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtafrqhoee.html

[O04] 定义异步函数并等待
来源：http://hz.jinqigufen.top/gtspqltnwu.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxuanxn.top/gtlcxosaik.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhengqikj.top/gtjtooqhqt.html

JS:   async function f() { await g(); }
来源：http://hz.cashguo.top/gtephyeuvo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.haohaochexian.top/gtnrpklcbi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.316326.xyz/gtskrieryc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigfzy.top/gtwvhgmfwb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtmztdgzzb.html

C#:   async Task F() { await G(); }
来源：http://hz.havefunace.top/gthyetsmko.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtcvybimkl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tanke756.top/gthnadyhnf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangshuangyany.cn/gtgwxttfgu.html

JS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtzbmjidov.html

TS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtjttejbnm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shzxlz.cn/gtimnjdbum.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cdnleiting.top/gtkiohhmxr.html

Ruby: threads.map(&:join)
来源：http://hz.hfpthk.cn/gtzjawpvmf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.pengpengdd.cyou/gtydqsvpzv.html

[O06] 使用进程池
来源：http://hz.dashuyun.cn/gtosmttzpn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhaomingkeji.xyz/gtyvwvfcvi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangdashe.top/gtccjtqdjn.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtzyskyjjw.html

TS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtpixabkoz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj20258888.top/gtswqkkvyf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gogol.net.cn/gtjdzqobrm.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gtqxvkucfw.html

C#:   Parallel.For
来源：http://hz.jqgfzy.top/gtuxgsvrhn.html

================================================================================
来源：http://hz.hfpthk.cn/gtudrvubtl.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtuomihqpw.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlpjnnwuo.html

[P01] 生成 UUID
来源：http://hz.yuxming.cn/gtsncyhfwr.html

Py:   str(uuid.uuid4())
来源：http://hz.jqgufenzy.top/gtcaplfuuc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.52xcode.cn/gtcvpvmazj.html

JS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtpuxvvrdm.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtfagziiyo.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj202588.top/gtsjlinnqd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxuanxn.top/gtfovjylua.html

Ruby: SecureRandom.uuid
来源：http://hz.haohaochexian.top/gtgilvihpc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.guannengcc.top/gtsthwwhcq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtzjjegboe.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinghuilouyu.cn/gtwnscuilo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.52xcode.cn/gtkhkwbzfe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.svipenyu.cn/gtxvtalnie.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sweek.top/gtsocnezly.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.tanke756.top/gtwnzjjshz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtdkrahdnl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtcwbrrnmt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhaomingkeji.xyz/gttjrgwzdo.html

[P03] 生成短随机字符串
来源：http://hz.ywan-chungtsiang.top/gtbowzyimi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hysaishi.cn/gttvfgtbnn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258.top/gtcclrfmid.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtbjfgkajg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sufxvd.cn/gtwzwsraso.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gtgcvlyumf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gotoacloud.top/gtyztlemgy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yanxiufei.cn/gtgvxqgyhz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuanzhike.top/gtdvmkizyw.html

[P04] 求长度
来源：http://hz.ivvv.top/gtwhsxlzpm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yanxiufei.cn/gtdhacbvhq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtqeywjqfh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.316326.xyz/gtbqriteoc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cdnleiting.top/gtpkwyoxui.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnqzz.top/gtkwiselgj.html

Go:   len(arr);  len(m)
来源：http://hz.nanxinkj.top/gtewnjqzzu.html

Ruby: x.length;  x.size
来源：http://hz.shuidangran.top/gtjksndgni.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.bjfxy.top/gtxdfadccf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.mhx1999.top/gthbopyxnf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daria6918.cn/gtajiiphdy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj20258888.top/gtabdlethz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tian-w.cn/gtwoweevtx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.9152youxi.cn/gtgvqxawcc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ppjwa.cn/gtbvgrsmpv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ybcxt.top/gtziyduoaw.html

Ruby: a == b
来源：http://hz.ppjwa.cn/gtspfsmhap.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cheryme.top/gtauzhalel.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aibaodan.cn/gtmoaakpbs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtyonfjqsx.html

PHP:  if (empty($x)) {}
来源：http://hz.ivvv.top/gtpmdipfyl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.havefunace.top/gtuiyhyylw.html

TS:   if (x == null) {}
来源：http://hz.shzxlz.cn/gtlytpjhai.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yonumen.top/gtigycykro.html

Go:   if x == nil {}
来源：http://hz.jqgufenzy.top/gtlyeshvre.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yongpay.top/gtgnumwmsg.html

C#:   if (x is null) {}
来源：http://hz.smart0.xyz/gtmsniopkg.html

[P07] 防抖与节流
来源：http://hz.jianghu66.top/gtpfgtisce.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hammf.cn/gtmcxmsizx.html

PHP:  // 手写时间戳比较
来源：http://hz.zhijiandao.cn/gtenvsgzmw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtuwatgbef.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ehwqpu.com/gtjxiogrnp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yuanzhike.top/gtpoaaxadz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xziqi.cn/gtpvpzcdhg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.316326.xyz/gtifksqspa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daria6918.cn/gtmhszrlub.html

[P08] 处理浮点精度问题
来源：http://hz.iojbl.cn/gtlxchvkay.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tanke756.top/gtwzlaesfm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gtewojhfpo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.haohaochexian.top/gtieificvf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.snrcjt.cn/gtqghfqfbw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangtech.top/gtnrabyyhy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ehwqpu.com/gtjxrtxdxh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.redwolf501.top/gtowevbktk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.52xcode.cn/gtokeyiwlh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gteaqnruwt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.vqdsnc.cn/gtblxyrqqx.html

================================================================================
来源：http://hz.aibaodan.cn/gtyndcjhzr.html

[Q01] 创建表
来源：http://hz.nanxinkj.top/gtdjvptypd.html

CREATE TABLE users (
来源：http://hz.jinqigfzy.top/gtunpfsczc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtdgfbfxmc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ehwqpu.com/gtxznkrdbm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.mhx1999.top/gtseerjoqm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shangyingyoupin.top/gtmqcltxav.html

);
来源：http://hz.ivvv.top/gthzzzlatk.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gtvgoufauc.html

CREATE TABLE orders (
来源：http://hz.xuetiantiany.cn/gtsvmeebgw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yangfankeji.com/gtirbyznjs.html

user_id INT NOT NULL,
来源：http://hz.smart0.xyz/gtmervdbbs.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gteuhzszvl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhaomingkeji.xyz/gtooxpfdgn.html

);
来源：http://hz.feifeiyinyue.top/gtuveadfvh.html

[Q03] 增加列
来源：http://hz.ehwqpu.com/gtgydbplgq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jlsjyb.cn/gtrmdzmwqc.html

[Q04] 修改列类型
来源：http://hz.sweek.top/gtvkfvevec.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtquvoqvpo.html

[Q05] 重命名列
来源：http://hz.gotoacloud.top/gtjndbgxpb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.wangshuangyany.cn/gtsvhtvnme.html

[Q06] 删除列
来源：http://hz.tian-w.cn/gtmelgawdu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gttzqgxprp.html

[Q07] 删除表
来源：http://hz.yj20258888.top/gtvwpocdvy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gtwoibxyio.html

[Q08] 创建普通索引
来源：http://hz.tianlin.xyz/gtlcxwcxah.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangdashe.top/gtqvogddbg.html

[Q09] 创建唯一索引
来源：http://hz.cqqwz.cn/gtjvuzzwpg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tian-w.cn/gtyzybuugq.html

[Q10] 插入单行
来源：http://hz.yvedp.cn/gtdwlgdpaz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fzhhl.top/gtoizhufur.html

[Q11] 一次插入多行
来源：http://hz.nanxuanxn.top/gtxoigbqek.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gtrwwllfsy.html

[Q12] 插入后取自增 ID
来源：http://hz.xuetiantiany.cn/gtmwthtxwv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.aibaodan.cn/gtxuzclqjn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinyuanbaomall.cn/gtmocfhvgf.html

[Q13] 忽略重复插入
来源：http://hz.nanxinkj.top/gtdqxgwcqj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cucudq.cn/gtdzgmoizp.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtkyjnyjmw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.316326.xyz/gtqxecoeoh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxuanxn.top/gthxpqrqcy.html

[Q15] 查询全部
来源：http://hz.shanyushiyangtech.top/gtyuqxgomb.html

SELECT * FROM users;
来源：http://hz.sysykeji.top/gtqsvhqxfh.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtnegywcau.html

SELECT id, name FROM users;
来源：http://hz.chenlongwang.top/gtuuervhmp.html

[Q17] 条件查询
来源：http://hz.yongpay.top/gtmvaaiekh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.9152youxi.cn/gttgrudist.html

[Q18] 模糊匹配
来源：http://hz.yuanzhike.top/gtyxsuchuq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xuanzx.com/gtbvzfesvh.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtvmowoyad.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtvmojrebe.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtaprwdyff.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.quarkkingdee.top/gtnwbfkqzx.html

[Q21] 空值判断
来源：http://hz.daria6918.cn/gtkpytlrpl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hongshengwenyu.top/gtdchsxblv.html

[Q22] 排序
来源：http://hz.cheryme.top/gtwpnflmac.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtcjksvrel.html

[Q23] 分页
来源：http://hz.zycfv.cn/gtomlroale.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cashguo.top/gteerxbfnj.html

[Q24] 去重
来源：http://hz.zhijiandao.cn/gtslvxakku.html

SELECT DISTINCT city FROM users;
来源：http://hz.yonumen.top/gtcyhufmps.html

[Q25] 只取前 N 条
来源：http://hz.smart0.xyz/gtuccfkqhg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gzhubu.top/gtdgxqefnk.html

[Q26] 计数
来源：http://hz.hnxiangtu.top/gtcjmmnuyr.html

SELECT COUNT(*) FROM users;
来源：http://hz.cheryme.top/gtbkhjcqhe.html

[Q27] 条件计数
来源：http://hz.jlsjyb.cn/gtycvobnaf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nanxinkj.top/gtlppyrpnf.html

[Q28] 求和与平均
来源：http://hz.tanke756.top/gtvguthvda.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhengqikj.top/gtpxjdffcb.html

[Q29] 最大最小值
来源：http://hz.kuanghao11.cn/gthbukzyne.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtkhtgyhvv.html

[Q30] 分组统计
来源：http://hz.9152youxi.cn/gtfytvryai.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtsztlejif.html

[Q31] 分组后过滤
来源：http://hz.snrcjt.cn/gtkrsuaqxh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhiwuduotai.top/gtfucflxew.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtrvcwcvpt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtgzfrkmti.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shangyingyoupin.top/gtbmyytvjk.html

[Q33] 多列分组
来源：http://hz.9152youxi.cn/gtjffkaasa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yuanzhike.top/gtuhhrpdvo.html

[Q34] 每组取第一条
来源：http://hz.xylfe.cn/gtwhgwjfdx.html

SELECT * FROM (
来源：http://hz.haohaochexian.top/gtxsvhhbdu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gotoacloud.top/gtgutnjwlf.html

) t WHERE rn = 1;
来源：http://hz.daxiang520.top/gtumgqgtvf.html

[Q35] 内连接
来源：http://hz.quarkkingdee.top/gtfmuishup.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtpynpgmzv.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtpyakvdhe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gthbdwndmu.html

[Q37] 右连接
来源：http://hz.zdqjudy.top/gtfywfymuj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gtulvzrffy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tanke756.top/gtfctmlkin.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tianlin.xyz/gtcussfiem.html

[Q39] 自连接（查上下级）
来源：http://hz.wangdashe.top/gthhxaxdov.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yongpay.top/gtdekbvcjt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gtsfziukrn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ywan-chungtsiang.top/gtvacrpqpw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jlsjyb.cn/gtmxyrcybl.html

[Q41] 多表连接
来源：http://hz.dashuyun.cn/gtkctakyki.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258.top/gtgmelvayb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xuanzx.com/gtztfejxwt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hywenlv.cn/gtjdalvrke.html

[Q42] 连接条件附加过滤
来源：http://hz.aibaodan.cn/gtdkvegzng.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xinyue.icu/gtgcyequpc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shzxlz.cn/gtirovecqy.html

[Q43] 标量子查询
来源：http://hz.fengsongda.top/gtvjlhiake.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yanxiufei.cn/gtwwjdedzk.html

[Q44] IN 子查询
来源：http://hz.shangyingyoupin.top/gtwpkmnmsd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangkeji.top/gtbkqeiodz.html

[Q45] EXISTS 判断存在
来源：http://hz.cucudq.cn/gtldbkmlrc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtrrefcjfw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.svipenyu.cn/gtspyxqqav.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gtthhcltso.html

[Q47] 与平均值比较
来源：http://hz.meibo888.top/gtieihqiyt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtvwwvloef.html

[Q48] CTE 公用表表达式
来源：http://hz.gogol.net.cn/gtkpomdohx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shuidangran.top/gtrknuvspl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtqnkrlxcv.html

[Q49] 更新单行
来源：http://hz.cheryme.top/gtrlfxmyjj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtdvkgsgtb.html

[Q50] 批量更新
来源：http://hz.pengpengdd.cyou/gtcfzryejz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtybzbmvit.html

[Q51] 用子查询更新
来源：http://hz.c1oappe.top/gtbyqxbxey.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pycfn.com/gtdwwypkvz.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtqtegugcz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtdeqymooa.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtixzzsjzm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gaohongyu789.top/gtdcdyyrxv.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtlvtflodq.html

TRUNCATE TABLE logs;
来源：http://hz.hammf.cn/gtpkchnejh.html

[Q55] 排名（并列占位）
来源：http://hz.wangdashe.top/gtsuaquqjw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydjk.org.cn/gtvmweltqx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tian-w.cn/gtrjwrozqp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fengsongda.top/gtgzpkhomw.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtfehgrjmy.html


<!-- 参考信息 -->