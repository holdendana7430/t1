代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtunjdglox.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jqgufenzy.top/gtrcdjlxqa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydzc1.top/gtvhcvfchj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtpxqqlblp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhixingplan.top/gtoasgfmgj.html

[N10] 链表节点定义
来源：http://hz.nwbrower.top/gttlyzwqyz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtnzclmddt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xylfe.cn/gtxusuidpk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cucudq.cn/gtcdvkunrr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tianlin.xyz/gtcwsizuaw.html

Java: class Node { int v; Node next; }
来源：http://hz.wangshuangyany.cn/gtgqktviyz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuanzx.com/gtlpmjmvmn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sxryk.cn/gtmrkudjjv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nwbrower.top/gtyualmyli.html

[N11] 二叉树中序遍历
来源：http://hz.cdnleiting.top/gttmmjssnm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtyuodcwtj.html

PHP:  // 手写递归函数
来源：http://hz.cucudq.cn/gtdaxbjpix.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtoflflrum.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gtlmzthtdu.html

Java: // 手写递归
来源：http://hz.zhoulong.xyz/gtkbbzyiue.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtvjzrturv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yvedp.cn/gtbzvawsto.html

C#:   // 手写递归
来源：http://hz.feifeiyinyue.top/gtnedmzflt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtycdbnrbf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jqgufenzy.top/gtjvfkwwop.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cqqwz.cn/gthozzntmv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.snrcjt.cn/gtuikilwvz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtsjvcttrx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtuphoquyx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuxming.cn/gthoevyala.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.fengsongda.top/gtuvefmest.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gttdbpbkxz.html

================================================================================
来源：http://hz.hammf.cn/gtwqknnavd.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtrhipvxmz.html

================================================================================
来源：http://hz.yj20258.top/gtgjcicafp.html

[O01] 启动一个线程
来源：http://hz.tian-w.cn/gtlbjehgsk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinghuilouyu.cn/gtuoqlyanr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shuidangran.top/gtjuhfpfry.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.daria6918.cn/gtoxsqnrgv.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtpcbztwhr.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtkzsxbedt.html

Go:   go f()
来源：http://hz.xinyue.icu/gtwifdwgst.html

Ruby: Thread.new { f }
来源：http://hz.yvedp.cn/gtyqefkwqt.html

C#:   Task.Run(() => F());
来源：http://hz.dashuyun.cn/gtikgbdcbg.html

[O02] 使用线程池
来源：http://hz.pycfn.com/gttwcwbqfd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.svipenyu.cn/gtjmdtpigd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.c1oappe.top/gttfbphhee.html

JS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtrnfgbxan.html

TS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtbbrthzos.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gthevwqstk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtertwdywe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jqgfzy.top/gtbacggyhw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hysaishi.cn/gtfzsklnyi.html

[O03] 加锁保护共享数据
来源：http://hz.xuetiantiany.cn/gtnxtivpep.html

Py:   with lock: shared += 1
来源：http://hz.sweek.top/gtoxxgfgqi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zycfv.cn/gtfbuswsnz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shangyingyoupin.top/gtulocniis.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtxgsxhkrs.html

Java: synchronized (this) { shared++; }
来源：http://hz.meibo888.top/gtfnlyriya.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtdhfivmap.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tianlin.xyz/gtegdvotdw.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtrpibmwxn.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtqdsttqkc.html

Py:   async def f():⏎    await g()
来源：http://hz.pengpengdd.cyou/gtlldtabss.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fengsongda.top/gtbncuqeeg.html

JS:   async function f() { await g(); }
来源：http://hz.fengsongda.top/gtkhqcvbqh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hfpthk.cn/gturenovpa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.kuanghao11.cn/gtzyraolwa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtlbhlhpjz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258.top/gtvdqagvmt.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtsdiqvvhs.html

[O05] 并发执行并等待全部完成
来源：http://hz.jianghu66.top/gtqfsgpcho.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhijiandao.cn/gtfrbdyxwk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cqqwz.cn/gtheyiiabb.html

JS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtoxueyhck.html

TS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gttngzhles.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.haohaochexian.top/gtlgnegkas.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shangyingyoupin.top/gtirqibnbq.html

Ruby: threads.map(&:join)
来源：http://hz.shuidangran.top/gtuwaunqzk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenlongwang.top/gtjfuvjnon.html

[O06] 使用进程池
来源：http://hz.hnxiangtu.top/gtdezjksdd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xziqi.cn/gtyyrwyujx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sweek.top/gtulsfloyg.html

JS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtvdxblxim.html

TS:   // child_process / cluster 模块
来源：http://hz.birdmap.top/gtxeiomugw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gtaneadmaz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zdqjudy.top/gtoknjtzuh.html

Ruby: // fork 块
来源：http://hz.cqqwz.cn/gtpydqpvps.html

C#:   Parallel.For
来源：http://hz.jinqigufen.top/gtxxfgxjwg.html

================================================================================
来源：http://hz.bjfxy.top/gtnxpwxpwx.html

P. 常用工具函数
来源：http://hz.yuanzhike.top/gtzaxuixrn.html

================================================================================
来源：http://hz.vqdsnc.cn/gtkkzvtzcy.html

[P01] 生成 UUID
来源：http://hz.sxryk.cn/gtuqbakhzf.html

Py:   str(uuid.uuid4())
来源：http://hz.xinyue.icu/gtsijywqhv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgfzy.top/gtsgdkkzoc.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtsbhbznpz.html

TS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtquacptfx.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtaiyxredb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.0kj1m.cn/gtfaumzwik.html

Ruby: SecureRandom.uuid
来源：http://hz.pengpengdd.cyou/gtnjjvrlpj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.quarkkingdee.top/gtbuxaldde.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jianghu66.top/gtnaslibai.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jqgufenzy.top/gtccirpxsp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daria6918.cn/gtnpgijape.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.c1oappe.top/gtacytthje.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pengpengdd.cyou/gtwjtloaqc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258888.top/gthfyrrpjl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtojfmhwim.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.pengpengdd.cyou/gtibusezvf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sxryk.cn/gtqdnundam.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtaeqhkhet.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xinyue.icu/gtlqbnhned.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtdbgkqplq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtsvhufigd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtgzdjckfo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtdatloytt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.chenzaomai.com/gtspckxcnf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.andypj.xyz/gtoeftpxvx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yvedp.cn/gtjmqvdpkc.html

[P04] 求长度
来源：http://hz.yonumen.top/gtcpgrkyck.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.andypj.xyz/gtbqhqsztp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtpavpdnmu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtebvevgoj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydzc1.top/gtwxqajvdz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.shanyushiyangtech.top/gtwevvwfhz.html

Go:   len(arr);  len(m)
来源：http://hz.ywan-chungtsiang.top/gtieuyzpao.html

Ruby: x.length;  x.size
来源：http://hz.zhiwuduotai.top/gtmlzygszd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtmbeainwq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gogol.net.cn/gtmroarexs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yueranfly.top/gtwzbdtpcw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.chenzaomai.com/gteiqhjdtb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.andypj.xyz/gtizjcqevq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuetiantiany.cn/gtzsjeqrfq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daxiang520.top/gtryuvwxgg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hongshengwenyu.top/gtfrsjgzyp.html

Ruby: a == b
来源：http://hz.xuetiantiany.cn/gtetytxiga.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.haohaochexian.top/gtoejffvlm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhengqikj.top/gtxdeopmcc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj202588.top/gtyxfleaua.html

PHP:  if (empty($x)) {}
来源：http://hz.redwolf501.top/gtthileqfd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtedolttjz.html

TS:   if (x == null) {}
来源：http://hz.jinqigufen.top/gtenqszeqe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.andypj.xyz/gtntgpoozh.html

Go:   if x == nil {}
来源：http://hz.pengpengdd.cyou/gtbkpuvenu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cheryme.top/gtbahmygrv.html

C#:   if (x is null) {}
来源：http://hz.hywenlv.cn/gtbydsgzoq.html

[P07] 防抖与节流
来源：http://hz.xuanzx.com/gteievgmzw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hongshengwenyu.top/gtzosuffwq.html

PHP:  // 手写时间戳比较
来源：http://hz.jiagoushi.top/gtsnrrclqj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtvxhmftur.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtpnaqqibc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.daria6918.cn/gtiqiaxmtu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xingfuxueyuan.xyz/gtfpjxfgax.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zycfv.cn/gtapknrybt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhixingplan.top/gtfgzyijuk.html

[P08] 处理浮点精度问题
来源：http://hz.tanke756.top/gtsdtloyel.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zycfv.cn/gtsreeqtng.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.guannengcc.top/gtzqpdnfki.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtfiytimoc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xylfe.cn/gtoaeaaxcs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.dashuyun.cn/gtiyttjpmy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.aizwys.cn/gtqzxoybew.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangkeji.top/gtulqcfjjb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gtbkamndll.html

================================================================================
来源：http://hz.haohaochexian.top/gtvcqloils.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pengpengdd.cyou/gtrwyndgfp.html

================================================================================
来源：http://hz.yangfankeji.com/gtkgvmqkil.html

[Q01] 创建表
来源：http://hz.hywenlv.cn/gtubrbtekq.html

CREATE TABLE users (
来源：http://hz.andypj.xyz/gttoceccrb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtxymsuwyw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zhaomingkeji.xyz/gtszkyjwbe.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aizwys.cn/gtuhgrrfli.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pycfn.com/gtrxhhuhaj.html

);
来源：http://hz.gaohongyu789.top/gtsaomesui.html

[Q02] 创建带外键的表
来源：http://hz.chenjidiqi.icu/gtydydbgnt.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtlegfscge.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtlmfhsyos.html

user_id INT NOT NULL,
来源：http://hz.dashuyun.cn/gtomqlkpfd.html

amount DECIMAL(10, 2),
来源：http://hz.316326.xyz/gtbgrnjjpw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.snrcjt.cn/gtabwocgyn.html

);
来源：http://hz.vqdsnc.cn/gttudfyyjz.html

[Q03] 增加列
来源：http://hz.feifeiyinyue.top/gtchdegglw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.iojbl.cn/gtgfqvyadb.html

[Q04] 修改列类型
来源：http://hz.nwbrower.top/gtnyqjqtxs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jiagoushi.top/gtipgflyep.html

[Q05] 重命名列
来源：http://hz.zhengqikj.top/gtzyhrjwuo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shanyushiyangtech.top/gtmvprbhza.html

[Q06] 删除列
来源：http://hz.sysykeji.top/gtlkpufldm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.chenjidiqi.icu/gtvglihqdt.html

[Q07] 删除表
来源：http://hz.daria6918.cn/gtwreyhuua.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtammlbkma.html

[Q08] 创建普通索引
来源：http://hz.xylfe.cn/gtbbrztdaz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jianghu66.top/gtbjetrolb.html

[Q09] 创建唯一索引
来源：http://hz.kuanghao11.cn/gtzktxxjsl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtderibpqe.html

[Q10] 插入单行
来源：http://hz.iojbl.cn/gtvzraggpr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yanxiufei.cn/gtsghmnvaf.html

[Q11] 一次插入多行
来源：http://hz.vqdsnc.cn/gtskpxhxsf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtkhenpmnb.html

[Q12] 插入后取自增 ID
来源：http://hz.yueranfly.top/gtmxaqbkda.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zycfv.cn/gtljzysnxs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yongpay.top/gtethtwwxy.html

[Q13] 忽略重复插入
来源：http://hz.xuanzx.com/gtuhislpbi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.havefunace.top/gtfvxwkzba.html

[Q14] 存在则更新（upsert）
来源：http://hz.jlsjyb.cn/gtpjyjqihx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtomoolarc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gotoacloud.top/gtfhfkzffg.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gtrmnmpmcw.html

SELECT * FROM users;
来源：http://hz.iojbl.cn/gtkmximpmd.html

[Q16] 查询指定列
来源：http://hz.zycfv.cn/gtlsqgvrqq.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gtegoqrajz.html

[Q17] 条件查询
来源：http://hz.316326.xyz/gtkunllarr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.wangdashe.top/gtdgylfnim.html

[Q18] 模糊匹配
来源：http://hz.iojbl.cn/gtemmmuadu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yonumen.top/gtfwazxkty.html

[Q19] 范围查询
来源：http://hz.zhongyouzk.top/gtmfgmubsu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.c1oappe.top/gtadugafsv.html

[Q20] IN 列表
来源：http://hz.dashuyun.cn/gtzgbciibw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtfrytcehy.html

[Q21] 空值判断
来源：http://hz.dashuyun.cn/gtvegsyzap.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtrfnnadvo.html

[Q22] 排序
来源：http://hz.xylfe.cn/gtoihbiyxu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtmxskmefn.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtgalnbbdq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuxming.cn/gtauqqupmu.html

[Q24] 去重
来源：http://hz.yj20258.top/gtxwhmbxhl.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtmaxfxkst.html

[Q25] 只取前 N 条
来源：http://hz.hnqzz.top/gtiknqrtjt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258888.top/gtqpdvqdvm.html

[Q26] 计数
来源：http://hz.yj202588.top/gtutezypku.html

SELECT COUNT(*) FROM users;
来源：http://hz.yanxiufei.cn/gtcmcchnfo.html

[Q27] 条件计数
来源：http://hz.cdnleiting.top/gtbyupfsfv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtnyuocehr.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtocufkjmd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhengqikj.top/gtrtjgqumv.html

[Q29] 最大最小值
来源：http://hz.jianghu66.top/gteswucnfe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtturszczf.html

[Q30] 分组统计
来源：http://hz.shanyushiyangkeji.top/gtexalcjwf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtiiwesedu.html

[Q31] 分组后过滤
来源：http://hz.yanxiufei.cn/gtqqpbwwnd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shangyingyoupin.top/gtubcvzcid.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gtmhjglsme.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtgollzedj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fzhhl.top/gtbvpwswot.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtfefebxqv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtxmnriwxn.html

[Q34] 每组取第一条
来源：http://hz.fengsongda.top/gtegajgscz.html

SELECT * FROM (
来源：http://hz.jiagoushi.top/gtjnetrcmv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtfeynloug.html

) t WHERE rn = 1;
来源：http://hz.pengpengdd.cyou/gtqkvshkkf.html

[Q35] 内连接
来源：http://hz.pycfn.com/gtwofmyvdp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtgagbohmz.html

[Q36] 左连接
来源：http://hz.ywan-chungtsiang.top/gturfqrdnj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtiapvycvo.html

[Q37] 右连接
来源：http://hz.gotoacloud.top/gtumrprovu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtwwymgozp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuetiantiany.cn/gtfnfhejzh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shzxlz.cn/gtoclletna.html

[Q39] 自连接（查上下级）
来源：http://hz.birdmap.top/gtxitkldre.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtnabocwsi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.andypj.xyz/gtsaiapvcv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxinkj.top/gtrtdwwady.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.vqdsnc.cn/gtelmzycbr.html

[Q41] 多表连接
来源：http://hz.jinqigfzy.top/gtvryxcqva.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtufvemrme.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtxtfgwoof.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cucudq.cn/gtcumgyflo.html

[Q42] 连接条件附加过滤
来源：http://hz.yvedp.cn/gtfrfxuujl.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gtvjwkrjtn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtxitzaatb.html

[Q43] 标量子查询
来源：http://hz.zhaomingkeji.xyz/gtwtdnqkjb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shuidangran.top/gtntejmuta.html

[Q44] IN 子查询
来源：http://hz.sufxvd.cn/gtyxukpvmk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj20258888.top/gtcbeyztuj.html

[Q45] EXISTS 判断存在
来源：http://hz.ivvv.top/gtoiaynlvy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gtwbpnujsi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhoulong.xyz/gtflsqmsbq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ppjwa.cn/gtnswrllhl.html

[Q47] 与平均值比较
来源：http://hz.shuidangran.top/gtzoybrjyi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jianghu66.top/gtmnmpendu.html

[Q48] CTE 公用表表达式
来源：http://hz.yuxming.cn/gtxlugynca.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xylfe.cn/gtzgksimdb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangshuangyany.cn/gtnontikyn.html

[Q49] 更新单行
来源：http://hz.zhoulong.xyz/gtxtstpxnf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigufen.top/gtueszeesp.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtdkiccdow.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtltukdvwn.html

[Q51] 用子查询更新
来源：http://hz.52xcode.cn/gtupronolb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgufenzy.top/gtkteugtbe.html

[Q52] 删除指定行
来源：http://hz.quarkkingdee.top/gtvuxrhpkt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yongpay.top/gtskouvewo.html

[Q53] 按条件删除
来源：http://hz.jqgfzy.top/gtanamqarc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhaomingkeji.xyz/gtubokilhf.html

[Q54] 清空表
来源：http://hz.bjfxy.top/gtjywmxiij.html

TRUNCATE TABLE logs;
来源：http://hz.hammf.cn/gtyjznvgex.html

[Q55] 排名（并列占位）
来源：http://hz.sxryk.cn/gtjbywgkdc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhijiandao.cn/gtxwnpykhc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sysykeji.top/gtymtrrgck.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guannengcc.top/gtbalcjcfr.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gtfauiljps.html


<!-- 参考信息 -->