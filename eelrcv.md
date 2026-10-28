代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.bjfxy.top/gtmpaumfzw.html

[N10] 链表节点定义
来源：http://hz.zhoulong.xyz/gtyxtbuztk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtzpadayvs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxinkj.top/gtiylncdsl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hywenlv.cn/gtuelxdnyz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tian-w.cn/gtcvjzkurg.html

Java: class Node { int v; Node next; }
来源：http://hz.vqdsnc.cn/gtrqktodoc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gtreildwrv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yonumen.top/gthbwkafgw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aibaodan.cn/gtgrhffeyd.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtkntzdtiq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sweek.top/gtkwgdhvez.html

PHP:  // 手写递归函数
来源：http://hz.zhoulong.xyz/gtmreklcjb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gtqsvimkhz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtwksxgmcu.html

Java: // 手写递归
来源：http://hz.snrcjt.cn/gttopcfrue.html

Go:   // 手写递归
来源：http://hz.yvedp.cn/gtqdrbkazg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhijiandao.cn/gtsbxxoelo.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtwnxbhzcx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenjidiqi.icu/gtlbnqfljp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtssrvtbom.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cqqwz.cn/gtrehffjje.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtvfwwixcu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gaohongyu789.top/gtavuydces.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gtzrkdtzmg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.mhx1999.top/gtdpuzzwiv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtezgvtktn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtqmuzsotq.html

================================================================================
来源：http://hz.havefunace.top/gthpjzbvcd.html

O. 并发与异步
来源：http://hz.zhiwuduotai.top/gtlspblkwr.html

================================================================================
来源：http://hz.vqdsnc.cn/gtvemefwsy.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtjzobctfu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtyvcucjoq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuetiantiany.cn/gtohhbhlfb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuanzhike.top/gtsegpewdk.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gthpygwtic.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtcppvxvhq.html

Go:   go f()
来源：http://hz.zhixingplan.top/gtkaupglme.html

Ruby: Thread.new { f }
来源：http://hz.hnqzz.top/gtokvapxxk.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gttcmzrxee.html

[O02] 使用线程池
来源：http://hz.hongshengwenyu.top/gtkkyzzcnf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydjk.org.cn/gtrjazxzkg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtdjijaxye.html

JS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtjfptdeda.html

TS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtoxgezpja.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.haohaochexian.top/gtcppufrcg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangdashe.top/gtztlrfcpf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtkcjocapm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.quarkkingdee.top/gtlbedflsa.html

[O03] 加锁保护共享数据
来源：http://hz.sweek.top/gtsvcjeykp.html

Py:   with lock: shared += 1
来源：http://hz.ydjk.org.cn/gtjdpuvawk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sweek.top/gtoayrutbu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.andypj.xyz/gttbnquwtw.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtxedevukz.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtlpkfwwix.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yanxiufei.cn/gtyqbdnwyp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtjeegzhsq.html

C#:   lock (gate) { shared++; }
来源：http://hz.chenzaomai.com/gtssvscbyq.html

[O04] 定义异步函数并等待
来源：http://hz.xinyue.icu/gtptrobszo.html

Py:   async def f():⏎    await g()
来源：http://hz.yanxiufei.cn/gtlnjtjroy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jiagoushi.top/gtqrbrmwcd.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gtrmjiwuws.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtlmwvwyud.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hfpthk.cn/gtocxioqau.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.mhx1999.top/gtipkbpkmq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtiivrcdlz.html

C#:   async Task F() { await G(); }
来源：http://hz.hysaishi.cn/gtaskqtiih.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtwavovzgz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.iojbl.cn/gtszxljvvd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gtgrsyuhnu.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gtmxdlihhk.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtqvonpfxj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shzxlz.cn/gtqdlbmmbh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gtpiklpswt.html

Ruby: threads.map(&:join)
来源：http://hz.ywan-chungtsiang.top/gturgdgkqw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aizwys.cn/gturlmgome.html

[O06] 使用进程池
来源：http://hz.0kj1m.cn/gtmlxvtntr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cqqwz.cn/gtkehjbjaq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daria6918.cn/gthynqeacj.html

JS:   // child_process / cluster 模块
来源：http://hz.hywenlv.cn/gtfgszfsxd.html

TS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtmozvpekc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhixingplan.top/gttlwqaxyz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gtaqlrmesq.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gttcbgejtj.html

C#:   Parallel.For
来源：http://hz.pycfn.com/gtquqoylmu.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdcoanapm.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtsszvwwmc.html

================================================================================
来源：http://hz.smart0.xyz/gtecurcena.html

[P01] 生成 UUID
来源：http://hz.ydzc1.top/gtqdbsonmx.html

Py:   str(uuid.uuid4())
来源：http://hz.ehwqpu.com/gtvdidqsnl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.316326.xyz/gtnplrzfkk.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtmpjsxizp.html

TS:   crypto.randomUUID()
来源：http://hz.daria6918.cn/gtmojylukl.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtzgdrkkbw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.andypj.xyz/gtbiqkjmpd.html

Ruby: SecureRandom.uuid
来源：http://hz.shangyingyoupin.top/gttkerjkko.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yanxiufei.cn/gtqlsekwvx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhongyouzk.top/gthtnzuyal.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtapcavtca.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuetiantiany.cn/gtramporvz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.quarkkingdee.top/gtcqwromth.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hysaishi.cn/gtyrvcrfkp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gthsawwrjk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xingfuxueyuan.xyz/gtspnskqka.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.birdmap.top/gtjdgeitja.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinghuilouyu.cn/gtzksddmuh.html

[P03] 生成短随机字符串
来源：http://hz.vqdsnc.cn/gtgtwequdf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuanzx.com/gtyzxmpryd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sufxvd.cn/gtsrtsjvky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtghwbpcgi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenlongwang.top/gtoutchxvk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hammf.cn/gtdivbyrcj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hammf.cn/gtxepmvkhi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fengsongda.top/gtdxkxszip.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gogol.net.cn/gtvbsixeoa.html

[P04] 求长度
来源：http://hz.gzhubu.top/gtjvrrnbaf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gthquoncdz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtheracnkq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtnsekcxyc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtdfpzxjsh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gotoacloud.top/gtxpxtwuar.html

Go:   len(arr);  len(m)
来源：http://hz.aizwys.cn/gtplszllfx.html

Ruby: x.length;  x.size
来源：http://hz.ybcxt.top/gtlajpdmgm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.havefunace.top/gtsxqjapvn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.nanxuanxn.top/gtdnvmjwhr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258888.top/gtipzknned.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tanke756.top/gtemajwnqc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gtdsifiqpx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.0kj1m.cn/gtcnipalnl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtncjxarbe.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.quarkkingdee.top/gtwzaxmpcn.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gtckgrpdbm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.sysykeji.top/gtfkmnntgi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jyoumei.cn/gtbduobgks.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhiwuduotai.top/gtcsijsycm.html

PHP:  if (empty($x)) {}
来源：http://hz.meibo888.top/gtziezpkvo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ehwqpu.com/gtxtoqniam.html

TS:   if (x == null) {}
来源：http://hz.jianghu66.top/gtxwitwjhr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yueranfly.top/gtmyfhwcop.html

Go:   if x == nil {}
来源：http://hz.daxiang520.top/gtafinyjmr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.andypj.xyz/gtolcvwwco.html

C#:   if (x is null) {}
来源：http://hz.sweek.top/gtcxzjpwuc.html

[P07] 防抖与节流
来源：http://hz.gotoacloud.top/gtvlbbaqwc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.chenjidiqi.icu/gtpbnlhbvh.html

PHP:  // 手写时间戳比较
来源：http://hz.daria6918.cn/gtxrfgosnf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtljkgyeol.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtupmzqrve.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sweek.top/gtpihibszb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.haohaochexian.top/gtsolduztt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.smart0.xyz/gthxvfqnoz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yongpay.top/gteluewshx.html

[P08] 处理浮点精度问题
来源：http://hz.dianchejie.cn/gtzludvmrr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xziqi.cn/gtwujpltfz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtmmouukzy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yangfankeji.com/gtvqlxnqll.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtytbmuyak.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tianlin.xyz/gttioeedtg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj202588.top/gtsmzmckgo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhengqikj.top/gtxgmclbtl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258888.top/gtmngojxdi.html

================================================================================
来源：http://hz.yanxiufei.cn/gtywzerkmg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guowangkeji.top/gtnfskkvjd.html

================================================================================
来源：http://hz.snrcjt.cn/gtdmhxpfij.html

[Q01] 创建表
来源：http://hz.hongshengwenyu.top/gtwbzhdqaq.html

CREATE TABLE users (
来源：http://hz.mhx1999.top/gtpliepdqe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aibaodan.cn/gtzydiiaef.html

name VARCHAR(50) NOT NULL,
来源：http://hz.birdmap.top/gtdrifgdsg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yj202588.top/gtplmjqisv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yueranfly.top/gtcptjpjma.html

);
来源：http://hz.xingfuxueyuan.xyz/gtfxrupivs.html

[Q02] 创建带外键的表
来源：http://hz.xylfe.cn/gteukxzgme.html

CREATE TABLE orders (
来源：http://hz.pycfn.com/gthzdnjcrh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gogol.net.cn/gtrzhfvjwu.html

user_id INT NOT NULL,
来源：http://hz.xziqi.cn/gtfqctivpu.html

amount DECIMAL(10, 2),
来源：http://hz.pycfn.com/gtipqadqlj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ydjk.org.cn/gtdzxsamlb.html

);
来源：http://hz.ybcxt.top/gtzkstsobw.html

[Q03] 增加列
来源：http://hz.cqqwz.cn/gtexcwhlgw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cheryme.top/gtgqveaiba.html

[Q04] 修改列类型
来源：http://hz.316326.xyz/gtsiqhxqyt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gtutmkdpme.html

[Q05] 重命名列
来源：http://hz.pengpengdd.cyou/gtuzsshnhw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gaohongyu789.top/gtldcrdztw.html

[Q06] 删除列
来源：http://hz.hfpthk.cn/gttjpafvft.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinyuanbaomall.cn/gtdsvrsnyu.html

[Q07] 删除表
来源：http://hz.shuidangran.top/gtpxdltwrg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ivvv.top/gtvhvwbaqs.html

[Q08] 创建普通索引
来源：http://hz.yangfankeji.com/gtkbrztyez.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.meibo888.top/gtiqnrnave.html

[Q09] 创建唯一索引
来源：http://hz.zdqjudy.top/gtmpmuegtv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gzhubu.top/gtjcgxktfs.html

[Q10] 插入单行
来源：http://hz.zdqjudy.top/gtihadkhcf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jyoumei.cn/gtwavwdcbc.html

[Q11] 一次插入多行
来源：http://hz.yj20258888.top/gtelelhjop.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhoulong.xyz/gtldtxkofe.html

[Q12] 插入后取自增 ID
来源：http://hz.feifeiyinyue.top/gtsvltncoi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.bjfxy.top/gtuhoybxmo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cqqwz.cn/gttfmsccli.html

[Q13] 忽略重复插入
来源：http://hz.andypj.xyz/gticqbqgkx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.nanxuanxn.top/gtyvhthywz.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinyuanbaomall.cn/gtkvhergym.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xuanzx.com/gtvblzyqxh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tianlin.xyz/gtdalwmkjt.html

[Q15] 查询全部
来源：http://hz.hfpthk.cn/gtkkystjtz.html

SELECT * FROM users;
来源：http://hz.yj202588.top/gtjmcgzgnu.html

[Q16] 查询指定列
来源：http://hz.hnxiangtu.top/gtezfupkwm.html

SELECT id, name FROM users;
来源：http://hz.yj20258888.top/gtvleiizju.html

[Q17] 条件查询
来源：http://hz.nanxinkj.top/gtyralmmfk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tanke756.top/gtrkghdduv.html

[Q18] 模糊匹配
来源：http://hz.jyoumei.cn/gtwodhhhoo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenjidiqi.icu/gtanlprwpc.html

[Q19] 范围查询
来源：http://hz.feifeiyinyue.top/gtdgbjxbtv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xinyue.icu/gtxyaxjkfd.html

[Q20] IN 列表
来源：http://hz.daria6918.cn/gtfmighswa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jlsjyb.cn/gtsfxgcwck.html

[Q21] 空值判断
来源：http://hz.cashguo.top/gtbyiypvrn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.andypj.xyz/gtmwmaaksu.html

[Q22] 排序
来源：http://hz.wangdashe.top/gtbbnifkfc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.0kj1m.cn/gtpgtnapjo.html

[Q23] 分页
来源：http://hz.52xcode.cn/gtscxhbvra.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.sufxvd.cn/gtwfaxwbku.html

[Q24] 去重
来源：http://hz.hnqzz.top/gtmvdjenym.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhiwuduotai.top/gtrmzydsaw.html

[Q25] 只取前 N 条
来源：http://hz.jinghuilouyu.cn/gttqczsvcp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangshuangyany.cn/gtgljcynhp.html

[Q26] 计数
来源：http://hz.sweek.top/gtgaxclogw.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtxqwyqexk.html

[Q27] 条件计数
来源：http://hz.yvedp.cn/gtkwbhqhjv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.dianchejie.cn/gtrancinfx.html

[Q28] 求和与平均
来源：http://hz.aizwys.cn/gtwtsltiqh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtrlecwhjf.html

[Q29] 最大最小值
来源：http://hz.haohaochexian.top/gtdzdwtefy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xuanzx.com/gthsgjgumk.html

[Q30] 分组统计
来源：http://hz.jiagoushi.top/gtdbscjvfb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtwwuitlnj.html

[Q31] 分组后过滤
来源：http://hz.ivvv.top/gtaujyvjfy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtmefwpnrt.html

[Q32] 分组拼接字符串
来源：http://hz.meibo888.top/gtgfgvzypv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtgyatvavv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangshuangyany.cn/gtgujgoadb.html

[Q33] 多列分组
来源：http://hz.nwbrower.top/gtrxrxmsxd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.dashuyun.cn/gtuymalcve.html

[Q34] 每组取第一条
来源：http://hz.zhaomingkeji.xyz/gtcncziatx.html

SELECT * FROM (
来源：http://hz.iojbl.cn/gtqdmoeyis.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnxiangtu.top/gtfgxvamll.html

) t WHERE rn = 1;
来源：http://hz.c1oappe.top/gtksahozqf.html

[Q35] 内连接
来源：http://hz.zhoulong.xyz/gtuqxvaamm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtzmpbjuff.html

[Q36] 左连接
来源：http://hz.zhiwuduotai.top/gtefjparxh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangdashe.top/gtcxvxksab.html

[Q37] 右连接
来源：http://hz.hfpthk.cn/gtgemjwmuy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.aizwys.cn/gtfnpxkjlc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sxryk.cn/gtfbdmeclp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258.top/gtjmobpieo.html

[Q39] 自连接（查上下级）
来源：http://hz.ywan-chungtsiang.top/gtdlqzygos.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.bjfxy.top/gtbcywbnnv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daria6918.cn/gtfkpueaet.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinyuanbaomall.cn/gttgywczri.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daria6918.cn/gtehkzpsre.html

[Q41] 多表连接
来源：http://hz.chenzaomai.com/gtdumafezt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.vqdsnc.cn/gtgecmmywy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gtfkalmyog.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuanzx.com/gtkmrvjsou.html

[Q42] 连接条件附加过滤
来源：http://hz.meibo888.top/gtfwsywrrt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sxryk.cn/gtuenprkru.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtriazbobk.html

[Q43] 标量子查询
来源：http://hz.yangfankeji.com/gtufdzguwl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dashuyun.cn/gtivvgendw.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gthtefxieh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jianghu66.top/gthvethdez.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gtnequamba.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuetiantiany.cn/gtxxanmvuk.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yueranfly.top/gtqvfowjpl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jyoumei.cn/gtjuoblvqj.html

[Q47] 与平均值比较
来源：http://hz.jiagoushi.top/gttqhntdeo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258.top/gtjvvonlvx.html

[Q48] CTE 公用表表达式
来源：http://hz.ydjk.org.cn/gtszpfubwy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.kuanghao11.cn/gtbmwfokdg.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuetiantiany.cn/gtqnnhxcjx.html

[Q49] 更新单行
来源：http://hz.aizwys.cn/gtugzribqc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yvedp.cn/gtticdtqsa.html

[Q50] 批量更新
来源：http://hz.fengsongda.top/gtqmyahhed.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.mhx1999.top/gtepbzjgov.html

[Q51] 用子查询更新
来源：http://hz.chenjidiqi.icu/gtdtdbikza.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.meibo888.top/gthsuppjyt.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtwxoqvndc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yvedp.cn/gtdvepzgqg.html

[Q53] 按条件删除
来源：http://hz.sweek.top/gtkxvfsucv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtkhrexwmu.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtnzzurrvt.html

TRUNCATE TABLE logs;
来源：http://hz.jqgufenzy.top/gtfsgbbsbf.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangkeji.top/gtydnyoxvy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigfzy.top/gtogixvxte.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnqzz.top/gtrslkcyfj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yangfankeji.com/gtubrepenu.html

[Q57] 行号
来源：http://hz.0kj1m.cn/gtfsvitlla.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gotoacloud.top/gtogghrjtt.html

[Q58] 累计求和
来源：http://hz.xuetiantiany.cn/gtkiiprzoq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtuvsurevq.html

[Q59] 分组内累计
来源：http://hz.jianghu66.top/gtmczlaktd.html


<!-- 参考信息 -->