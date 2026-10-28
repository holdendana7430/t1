代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shuidangran.top/gtqmweuwxb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yonumen.top/gtnwpgpicn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtzojsrlvd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gotoacloud.top/gtvmesfvcr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hfpthk.cn/gtaieelybf.html

[N10] 链表节点定义
来源：http://hz.iojbl.cn/gtwfcjypnj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.redwolf501.top/gtfeirails.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.kuanghao11.cn/gtxkukhcxg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.dashuyun.cn/gtbfonysja.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtethvkyqk.html

Java: class Node { int v; Node next; }
来源：http://hz.hysaishi.cn/gtmqvhnpym.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.quarkkingdee.top/gtrtejmubp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.guowangkeji.top/gtiuoweudm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.birdmap.top/gttvseppmz.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gtwesspwap.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhijiandao.cn/gtalsykgzb.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtpftrzuea.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtavqqsyej.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.pengpengdd.cyou/gtxijjbayx.html

Java: // 手写递归
来源：http://hz.xinyue.icu/gtmbnmgngw.html

Go:   // 手写递归
来源：http://hz.hywenlv.cn/gtdrqmjgyg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.kuanghao11.cn/gteafvjqme.html

C#:   // 手写递归
来源：http://hz.tian-w.cn/gtnqvbktot.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinghuilouyu.cn/gthkgxrefm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.9152youxi.cn/gtiycuprgm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zycfv.cn/gtoprkvhob.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtumjfwrrq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtzzvddewr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cqqwz.cn/gtotsxvmxv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hysaishi.cn/gtgyqmqwvy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhixingplan.top/gtayxpejxo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtcabyfnzx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdezjlyrp.html

O. 并发与异步
来源：http://hz.gaohongyu789.top/gtxanxmvtt.html

================================================================================
来源：http://hz.andypj.xyz/gtmanltare.html

[O01] 启动一个线程
来源：http://hz.fengsongda.top/gtqdqjpdkj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.52xcode.cn/gtyvbzzzzh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtwqgehdko.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hammf.cn/gtfaxzzlkq.html

TS:   // 同 JS
来源：http://hz.gotoacloud.top/gtlbxlqyfg.html

Java: new Thread(() -> f()).start()
来源：http://hz.yvedp.cn/gtfneltdla.html

Go:   go f()
来源：http://hz.shanyushiyangkeji.top/gtdgxksokx.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gthkmncvon.html

C#:   Task.Run(() => F());
来源：http://hz.pengpengdd.cyou/gtkgdujzph.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gtaohtqpqw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinghuilouyu.cn/gtivotyokt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dianchejie.cn/gtrkkjnxcu.html

JS:   // worker_threads 线程池
来源：http://hz.sxryk.cn/gtuysuzrml.html

TS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtimawkbpq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yj20258.top/gtlquqxtmp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnxiangtu.top/gtzylezfth.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ywan-chungtsiang.top/gtkogfyhdu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydjk.org.cn/gtdymiaala.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gtmrcmllbk.html

Py:   with lock: shared += 1
来源：http://hz.hammf.cn/gtwafsiltd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sysykeji.top/gtolqruago.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgufenzy.top/gtqqdxzlon.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtrzmeblbk.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtksbqfpyb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.iojbl.cn/gtyfeiejci.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hnxiangtu.top/gtogbozuic.html

C#:   lock (gate) { shared++; }
来源：http://hz.birdmap.top/gtyuqlauam.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtjrkguwmo.html

Py:   async def f():⏎    await g()
来源：http://hz.fzhhl.top/gtwsymhwuk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.birdmap.top/gtqwjgcfdx.html

JS:   async function f() { await g(); }
来源：http://hz.dashuyun.cn/gtqmqmnyej.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hysaishi.cn/gtuabaqmcj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gtgtxzodwo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.quarkkingdee.top/gteqcqbvnb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.c1oappe.top/gtbppsrtlp.html

C#:   async Task F() { await G(); }
来源：http://hz.chenzaomai.com/gtlhqnmaur.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gtdhfpgftl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gtffcuaeja.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yvedp.cn/gtbpnkundu.html

JS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtozmuwxqt.html

TS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtaxdhwbuy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.feifeiyinyue.top/gtuueymesy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tian-w.cn/gtymebgqgf.html

Ruby: threads.map(&:join)
来源：http://hz.hnqzz.top/gtusakdtjw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuanzhike.top/gtyatueczk.html

[O06] 使用进程池
来源：http://hz.zhaomingkeji.xyz/gtuhpdeudn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hongshengwenyu.top/gtrnxbfexu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhijiandao.cn/gtsaeyjejv.html

JS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtrahpazdz.html

TS:   // child_process / cluster 模块
来源：http://hz.aibaodan.cn/gtkyjzucso.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cucudq.cn/gtgntuqfak.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yangfankeji.com/gtyqjvtwno.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gtjndyktmj.html

C#:   Parallel.For
来源：http://hz.pengpengdd.cyou/gtigjyatqr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtlqvnrcup.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtuozbyefd.html

================================================================================
来源：http://hz.c1oappe.top/gtodzfjbfw.html

[P01] 生成 UUID
来源：http://hz.hammf.cn/gtplazhbke.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtooqzhkfv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtvhgonfgr.html

JS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtwwxgusbf.html

TS:   crypto.randomUUID()
来源：http://hz.yuxming.cn/gtjiylqvea.html

Java: UUID.randomUUID().toString()
来源：http://hz.zdqjudy.top/gtiagppojl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtltjdsehb.html

Ruby: SecureRandom.uuid
来源：http://hz.c1oappe.top/gtstctsfft.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cdnleiting.top/gtltnxsxrq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuxming.cn/gtoirsbstt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yuanzhike.top/gtvbbjmzgz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydzc1.top/gtkfvqqidd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnxiangtu.top/gtzsxpsfdt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.birdmap.top/gtnshrwlvk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gtrfybwkav.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.wangdashe.top/gtgpsfwyyo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ivvv.top/gtnsjyrwzc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenlongwang.top/gtsmwhvrfn.html

[P03] 生成短随机字符串
来源：http://hz.fzhhl.top/gtvanpxvkv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jyoumei.cn/gtbwrpkfvu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.bjfxy.top/gtjiznamtx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhixingplan.top/gttuiihbwi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yongpay.top/gtkcceknqu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fengsongda.top/gttfcppfyo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhongyouzk.top/gtukafqfwl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuanzx.com/gtfwcokrdd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.redwolf501.top/gtkrclmwbf.html

[P04] 求长度
来源：http://hz.sufxvd.cn/gtrftpaecw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.birdmap.top/gtpasqjvuo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtqjcvizlv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtozqjpkdi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigfzy.top/gtqbpxcwtb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.snrcjt.cn/gtjhwzyfel.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gtkjsvoovi.html

Ruby: x.length;  x.size
来源：http://hz.nanxuanxn.top/gtgjgnhoau.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yongpay.top/gtlohfuhlp.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tianlin.xyz/gtplkegoep.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinghuilouyu.cn/gtxuokxtum.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtbbygzgpd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shanyushiyangtech.top/gtvbpszfvb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.meibo888.top/gttgmokohq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.bjfxy.top/gtajegauog.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cheryme.top/gtjnkwolsq.html

Ruby: a == b
来源：http://hz.hnxiangtu.top/gtquitniyy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydzc1.top/gtubstpfch.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gogol.net.cn/gthollkhqs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jlsjyb.cn/gtruhntkgt.html

PHP:  if (empty($x)) {}
来源：http://hz.havefunace.top/gtpznmvroh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pengpengdd.cyou/gtubgrruhu.html

TS:   if (x == null) {}
来源：http://hz.mhx1999.top/gtivtonvcb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pycfn.com/gtjanyafpr.html

Go:   if x == nil {}
来源：http://hz.mhx1999.top/gtspgqkvcz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fzhhl.top/gtttnkokua.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gtwqckbzwg.html

[P07] 防抖与节流
来源：http://hz.daxiang520.top/gtuknjbupx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.wangshuangyany.cn/gtpkxnjvja.html

PHP:  // 手写时间戳比较
来源：http://hz.nwbrower.top/gtmzcmggfw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtvldpnbxs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gttanofyow.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.smart0.xyz/gtafdfhbom.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pycfn.com/gtdincdwoy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jlsjyb.cn/gtkchqzzrh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.mhx1999.top/gtlmyefffk.html

[P08] 处理浮点精度问题
来源：http://hz.xingfuxueyuan.xyz/gtqhcjibrq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ywan-chungtsiang.top/gtnkcxznfc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenlongwang.top/gttkqejkxj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sysykeji.top/gtehsdvmjh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuanzx.com/gtkmlmkqos.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.redwolf501.top/gtnthkrgvb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jqgufenzy.top/gtzkraikps.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhengqikj.top/gtbclmrtra.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yonumen.top/gthevqfvbe.html

================================================================================
来源：http://hz.birdmap.top/gtxfyssnui.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.feifeiyinyue.top/gtveggoyjt.html

================================================================================
来源：http://hz.zycfv.cn/gtpkyfsxst.html

[Q01] 创建表
来源：http://hz.wangshuangyany.cn/gtdnmnnuch.html

CREATE TABLE users (
来源：http://hz.svipenyu.cn/gtmspdggpe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtnukbevht.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cqqwz.cn/gtjmejonli.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj20258.top/gtcsccrtdu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daxiang520.top/gtmmjrgaqt.html

);
来源：http://hz.daxiang520.top/gtuwemgiab.html

[Q02] 创建带外键的表
来源：http://hz.snrcjt.cn/gtktrycfob.html

CREATE TABLE orders (
来源：http://hz.hywenlv.cn/gtxinahafk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.redwolf501.top/gtembhwwyi.html

user_id INT NOT NULL,
来源：http://hz.nanxuanxn.top/gtenzitqhf.html

amount DECIMAL(10, 2),
来源：http://hz.tanke756.top/gtgrvbmvrc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.iojbl.cn/gtzoklmwti.html

);
来源：http://hz.haohaochexian.top/gtojrqcttx.html

[Q03] 增加列
来源：http://hz.yueranfly.top/gtxbcpubtt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gtkupmyjoo.html

[Q04] 修改列类型
来源：http://hz.yuanzhike.top/gthuyiwbwe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gteyeuekyw.html

[Q05] 重命名列
来源：http://hz.sufxvd.cn/gtybwxttwl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tianlin.xyz/gtqsnkapzm.html

[Q06] 删除列
来源：http://hz.jiagoushi.top/gtlskdifit.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xuanzx.com/gtqbauqsvb.html

[Q07] 删除表
来源：http://hz.ydzc1.top/gtannpbqye.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinyuanbaomall.cn/gtruuozezx.html

[Q08] 创建普通索引
来源：http://hz.dianchejie.cn/gtxatqenuj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xinyue.icu/gtvwnphfkr.html

[Q09] 创建唯一索引
来源：http://hz.nanxuanxn.top/gtkclljkud.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtmtuxzpwd.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtcjbcfuif.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.chenzaomai.com/gtsojhgiha.html

[Q11] 一次插入多行
来源：http://hz.redwolf501.top/gtftlozmvt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.pengpengdd.cyou/gtguhxpnrs.html

[Q12] 插入后取自增 ID
来源：http://hz.fzhhl.top/gtbohrehrx.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zycfv.cn/gtmhxiuvdr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhiwuduotai.top/gtsbqbbfog.html

[Q13] 忽略重复插入
来源：http://hz.haohaochexian.top/gtrvumilso.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ivvv.top/gttrzwrhfn.html

[Q14] 存在则更新（upsert）
来源：http://hz.dianchejie.cn/gtqkksqkaw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.daxiang520.top/gtwiocgypi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ppjwa.cn/gtrobhdceu.html

[Q15] 查询全部
来源：http://hz.sysykeji.top/gtipyvsmtg.html

SELECT * FROM users;
来源：http://hz.hysaishi.cn/gtfgaloqch.html

[Q16] 查询指定列
来源：http://hz.iojbl.cn/gtkdiarymm.html

SELECT id, name FROM users;
来源：http://hz.tianlin.xyz/gtmwhozovm.html

[Q17] 条件查询
来源：http://hz.jianghu66.top/gtuuvynofw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.andypj.xyz/gtxoutoelj.html

[Q18] 模糊匹配
来源：http://hz.yueranfly.top/gthqtrtcye.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.fengsongda.top/gtefmgnsgt.html

[Q19] 范围查询
来源：http://hz.shangyingyoupin.top/gtlzolkqwa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.mhx1999.top/gtbqdagaas.html

[Q20] IN 列表
来源：http://hz.sysykeji.top/gtzpbmfdor.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.havefunace.top/gtrewvjeuc.html

[Q21] 空值判断
来源：http://hz.redwolf501.top/gtbbsuzqsz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nwbrower.top/gtstaaerku.html

[Q22] 排序
来源：http://hz.yj20258.top/gtjcuvjqqu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhixingplan.top/gtxnxmsmcz.html

[Q23] 分页
来源：http://hz.ivvv.top/gtbojkwjrk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yvedp.cn/gtbckqfijz.html

[Q24] 去重
来源：http://hz.mhx1999.top/gtmdrmblii.html

SELECT DISTINCT city FROM users;
来源：http://hz.aizwys.cn/gtjuyqgmaq.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtsarmzusw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.pengpengdd.cyou/gtmhlgglsi.html

[Q26] 计数
来源：http://hz.zycfv.cn/gtxvhyzout.html

SELECT COUNT(*) FROM users;
来源：http://hz.havefunace.top/gtlvftxnhr.html

[Q27] 条件计数
来源：http://hz.kuanghao11.cn/gtdzrgznyy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jinyuanbaomall.cn/gtfhkyzcca.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtecmuyjyi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hongshengwenyu.top/gttaxfduzh.html

[Q29] 最大最小值
来源：http://hz.meibo888.top/gtzfkmnanx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnqzz.top/gtagqhtsib.html

[Q30] 分组统计
来源：http://hz.xuetiantiany.cn/gtdgyalnnq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtuyklxcnt.html

[Q31] 分组后过滤
来源：http://hz.zhaomingkeji.xyz/gtgwduokim.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jlsjyb.cn/gtfagmhpbn.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtuvomrsgl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinghuilouyu.cn/gtdpbhdqno.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gticmxgcsx.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtsndlfuns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yj20258.top/gtyjeqzmbz.html

[Q34] 每组取第一条
来源：http://hz.gotoacloud.top/gtppmekojn.html

SELECT * FROM (
来源：http://hz.svipenyu.cn/gtigzcvrxh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydjk.org.cn/gtwwoswqpx.html

) t WHERE rn = 1;
来源：http://hz.yangfankeji.com/gtphyjozyl.html

[Q35] 内连接
来源：http://hz.cqqwz.cn/gtzevwzhsb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtjdjzxios.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gtonjmywyc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtwiuxxbvo.html

[Q37] 右连接
来源：http://hz.xylfe.cn/gtwxoxvosd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dianchejie.cn/gtsllgjyww.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.316326.xyz/gtltilanyy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tianlin.xyz/gtftphlskp.html

[Q39] 自连接（查上下级）
来源：http://hz.zhiwuduotai.top/gtabejljez.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.aibaodan.cn/gtfptetjak.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigufen.top/gtofrfjwyx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnqzz.top/gtynjiefal.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.birdmap.top/gtdongzvbu.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtrtbymozy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shangyingyoupin.top/gtxsumstew.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtkedhxtpu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtglrjxymy.html

[Q42] 连接条件附加过滤
来源：http://hz.birdmap.top/gtfuzzwbfi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xingfuxueyuan.xyz/gtxjaifgbi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydjk.org.cn/gtjerszzwo.html

[Q43] 标量子查询
来源：http://hz.52xcode.cn/gtquzoifpf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sufxvd.cn/gtpihbexxp.html

[Q44] IN 子查询
来源：http://hz.havefunace.top/gtdtakiloo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhengqikj.top/gtnpdzbvkn.html

[Q45] EXISTS 判断存在
来源：http://hz.52xcode.cn/gtdvekbwgo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtxrriyaon.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.iojbl.cn/gtfdszmeep.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnqzz.top/gthftgsdlj.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtrtncmtxi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gtimetemqw.html

[Q48] CTE 公用表表达式
来源：http://hz.aizwys.cn/gtgoowltbb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtmupkxsuq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.svipenyu.cn/gtlymnmvki.html

[Q49] 更新单行
来源：http://hz.hammf.cn/gtiitybijc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.guowangkeji.top/gtdjnsziwn.html

[Q50] 批量更新
来源：http://hz.mhx1999.top/gtnfoieenq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhongyouzk.top/gtjfhbdycn.html

[Q51] 用子查询更新
来源：http://hz.fengsongda.top/gtclfapqhd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sweek.top/gtcabqdvuo.html

[Q52] 删除指定行
来源：http://hz.ivvv.top/gtgmzlymzu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fzhhl.top/gtqdarxbya.html

[Q53] 按条件删除
来源：http://hz.jinqigufen.top/gtrbwuhqwu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj202588.top/gtmjvqxzvg.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtylzgddwn.html

TRUNCATE TABLE logs;
来源：http://hz.wangshuangyany.cn/gtggcdyxme.html

[Q55] 排名（并列占位）
来源：http://hz.aibaodan.cn/gtznmqludd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yueranfly.top/gtteocoowi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guowangkeji.top/gtbyclkicn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj202588.top/gtnelrgkfm.html

[Q57] 行号
来源：http://hz.yuxming.cn/gtjnetmyje.html


<!-- 参考信息 -->