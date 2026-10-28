代发 wailian999

PHP:  // 手写递归函数
来源：http://hz.snrcjt.cn/gtgrmxclcw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gteiqxufjs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gtpdwkpkxc.html

Java: // 手写递归
来源：http://hz.hnqzz.top/gtjmwnafqz.html

Go:   // 手写递归
来源：http://hz.fengsongda.top/gtymbsazjh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pengpengdd.cyou/gtctaeoitq.html

C#:   // 手写递归
来源：http://hz.yongpay.top/gtunkeppqo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.feifeiyinyue.top/gteqjgxssg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gtsxmlfsyc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.birdmap.top/gtvayovqjj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gttjxedjzu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtmxofmjcu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtucmajycy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cheryme.top/gtftmvdorw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tianlin.xyz/gtpptmpqqg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtrjuztsgv.html

================================================================================
来源：http://hz.yvedp.cn/gtlgdddejm.html

O. 并发与异步
来源：http://hz.zhoulong.xyz/gtbvfnyibi.html

================================================================================
来源：http://hz.sweek.top/gtpielwpkb.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtfcmaqubm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jianghu66.top/gtfwrczsye.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtqvfcbinp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tianlin.xyz/gtsunzkxpq.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gtapbojpyr.html

Java: new Thread(() -> f()).start()
来源：http://hz.birdmap.top/gtpjiemkvm.html

Go:   go f()
来源：http://hz.fengsongda.top/gtzgjbzbwn.html

Ruby: Thread.new { f }
来源：http://hz.jlsjyb.cn/gtlnerbvoe.html

C#:   Task.Run(() => F());
来源：http://hz.sysykeji.top/gtzsbgynjw.html

[O02] 使用线程池
来源：http://hz.andypj.xyz/gturxfkahi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhijiandao.cn/gtxecizfbi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.snrcjt.cn/gttdbarlsw.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtcnlhmwvu.html

TS:   // worker_threads 线程池
来源：http://hz.gaohongyu789.top/gtkyimcdaj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.kuanghao11.cn/gtztvxteae.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zycfv.cn/gtvwebvsjt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gtghknhkfm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gtodcthwra.html

[O03] 加锁保护共享数据
来源：http://hz.gaohongyu789.top/gtcqxqvcyw.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtukxqxolc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangdashe.top/gtnidkujry.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jlsjyb.cn/gtidfrihbf.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gtodiytbxm.html

Java: synchronized (this) { shared++; }
来源：http://hz.sufxvd.cn/gtlzrxmbrn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hongshengwenyu.top/gtqjwbhyiq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.redwolf501.top/gtssmdcytx.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtzhgrptfa.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangtech.top/gtvbhhqdav.html

Py:   async def f():⏎    await g()
来源：http://hz.ydzc1.top/gtmwjeplfw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenjidiqi.icu/gtafqzvxqo.html

JS:   async function f() { await g(); }
来源：http://hz.guowangkeji.top/gtkmbqivro.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtfirzvwya.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.vqdsnc.cn/gtapbmpnvh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.birdmap.top/gtuddkjmfo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtvvgzmytv.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gtfbqfxtka.html

[O05] 并发执行并等待全部完成
来源：http://hz.yangfankeji.com/gtsxxznwcp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhixingplan.top/gtijhbkahj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gotoacloud.top/gtjvsghcel.html

JS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtkgkoxizl.html

TS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtdssxjtbm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhoulong.xyz/gtxvpfvmpb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.fzhhl.top/gtbsjgrgxk.html

Ruby: threads.map(&:join)
来源：http://hz.jianghu66.top/gtlnshahvg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yuxming.cn/gtefguvapv.html

[O06] 使用进程池
来源：http://hz.svipenyu.cn/gtlgzkpeiv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtoikrakpo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.daria6918.cn/gtncclevjo.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtpnqgufyo.html

TS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtskmuevdy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.redwolf501.top/gteilfctzl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cucudq.cn/gtjedzbmrr.html

Ruby: // fork 块
来源：http://hz.jqgfzy.top/gtezdxoyhz.html

C#:   Parallel.For
来源：http://hz.tian-w.cn/gtbhoowohk.html

================================================================================
来源：http://hz.nwbrower.top/gtdqopdkjz.html

P. 常用工具函数
来源：http://hz.iojbl.cn/gtpmnzhjps.html

================================================================================
来源：http://hz.redwolf501.top/gtqdkrwebh.html

[P01] 生成 UUID
来源：http://hz.pycfn.com/gtlykrxkjt.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtlmwfvyrm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shuidangran.top/gtgixsaklg.html

JS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtofytzaax.html

TS:   crypto.randomUUID()
来源：http://hz.sysykeji.top/gttmchkjfk.html

Java: UUID.randomUUID().toString()
来源：http://hz.smart0.xyz/gtbklxjcsr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yongpay.top/gtzmsbbjsb.html

Ruby: SecureRandom.uuid
来源：http://hz.xinyue.icu/gtwfudjcmm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gzhubu.top/gtduyiemgj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cqqwz.cn/gtkcunomby.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jianghu66.top/gtsbgpmdty.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.c1oappe.top/gtftzndlpe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xuetiantiany.cn/gtbwujksvo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fzhhl.top/gtyklgnwws.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.mhx1999.top/gtlkvqelcn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gtibhldaun.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtfxgqloiz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhixingplan.top/gtmuimhslt.html

[P03] 生成短随机字符串
来源：http://hz.svipenyu.cn/gtbpsngkkw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhijiandao.cn/gtuypjxxpk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtgcobwdga.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtsfmrshpx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.pycfn.com/gtuczjifup.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ehwqpu.com/gtutnrvqdg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.meibo888.top/gtbdnyoagt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tian-w.cn/gtwniofnmr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhongyouzk.top/gtyvejvtkj.html

[P04] 求长度
来源：http://hz.yangfankeji.com/gterrllzst.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhaomingkeji.xyz/gthoxogdfr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtxwurauvo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtgzbktulo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtjjrmprhi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.316326.xyz/gtambmkoxp.html

Go:   len(arr);  len(m)
来源：http://hz.redwolf501.top/gtmcrustuc.html

Ruby: x.length;  x.size
来源：http://hz.iojbl.cn/gttqkvytwl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinqigufen.top/gtocrdgqcg.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenzaomai.com/gtchzwtngy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.chenjidiqi.icu/gtcmaccaqo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shanyushiyangtech.top/gtouoxawlq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.0kj1m.cn/gtwjsknxeq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.feifeiyinyue.top/gtxydldlpp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shzxlz.cn/gtffduvvxe.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgufenzy.top/gtnzwoqplc.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtlmpdwwes.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xuetiantiany.cn/gthhzpjokq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.aibaodan.cn/gtiimomnbf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tanke756.top/gtkvoatfyx.html

PHP:  if (empty($x)) {}
来源：http://hz.nanxuanxn.top/gtgsooxdwh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xingfuxueyuan.xyz/gttqvmbusj.html

TS:   if (x == null) {}
来源：http://hz.ivvv.top/gttbpyiqoz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtzxuijbii.html

Go:   if x == nil {}
来源：http://hz.hywenlv.cn/gtonpgavdy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.snrcjt.cn/gtzaicmyua.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtqsnnxidb.html

[P07] 防抖与节流
来源：http://hz.cheryme.top/gtffgaqpvc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ydzc1.top/gtcgmfqzco.html

PHP:  // 手写时间戳比较
来源：http://hz.sysykeji.top/gtqtwzdbri.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtolvjlaqo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.9152youxi.cn/gtaigltjmu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cheryme.top/gtrdmhoaof.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xziqi.cn/gtnuewoglm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sufxvd.cn/gtxuydgqqo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gotoacloud.top/gtmgbwzdvw.html

[P08] 处理浮点精度问题
来源：http://hz.gogol.net.cn/gtdxergxxp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tian-w.cn/gtfcxnhtsu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.snrcjt.cn/gtqtcynzll.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhijiandao.cn/gtnufbwrkp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.meibo888.top/gtldmogjmh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yongpay.top/gtxrkinugo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenlongwang.top/gtjienevgg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtpouvjmsj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cucudq.cn/gtizigmgvx.html

================================================================================
来源：http://hz.jiagoushi.top/gtrbnthebd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnqzz.top/gttlhsxqjs.html

================================================================================
来源：http://hz.snrcjt.cn/gtphnbhkhb.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtrynokawa.html

CREATE TABLE users (
来源：http://hz.nanxuanxn.top/gtyypmorqw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtzzvdlsda.html

name VARCHAR(50) NOT NULL,
来源：http://hz.iojbl.cn/gtmdmgjlbl.html

email VARCHAR(100) UNIQUE,
来源：http://hz.shzxlz.cn/gtstkgmrgb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tian-w.cn/gtllvfzwrc.html

);
来源：http://hz.cashguo.top/gtajcmyusg.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtsukzbkbu.html

CREATE TABLE orders (
来源：http://hz.xziqi.cn/gtcktbwkdz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtptpwgulr.html

user_id INT NOT NULL,
来源：http://hz.wangdashe.top/gthoxxvntp.html

amount DECIMAL(10, 2),
来源：http://hz.meibo888.top/gtvjzykrfq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuanzx.com/gttgdpifrz.html

);
来源：http://hz.yuanzhike.top/gtyrbxyeqf.html

[Q03] 增加列
来源：http://hz.xylfe.cn/gtqytdksai.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gtmaufsilt.html

[Q04] 修改列类型
来源：http://hz.vqdsnc.cn/gtxwhgwqrf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yangfankeji.com/gtwvxrhsoy.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtaixwjzxl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.shuidangran.top/gtdeuvtqsb.html

[Q06] 删除列
来源：http://hz.0kj1m.cn/gtdvertjdu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gtltssmbnv.html

[Q07] 删除表
来源：http://hz.jinqigfzy.top/gtjjjpdixz.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gotoacloud.top/gtwihlycai.html

[Q08] 创建普通索引
来源：http://hz.jianghu66.top/gttjubaojq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gtbjrryavd.html

[Q09] 创建唯一索引
来源：http://hz.hfpthk.cn/gthoxwceqy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yueranfly.top/gtveyrmlxu.html

[Q10] 插入单行
来源：http://hz.0kj1m.cn/gtmzsbcmgj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinqigufen.top/gtmpwsiycq.html

[Q11] 一次插入多行
来源：http://hz.sxryk.cn/gtwrumyoqx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuanzhike.top/gtbeqoiveu.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtxnowcssq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.bjfxy.top/gtzbllktfl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.mhx1999.top/gtphczawow.html

[Q13] 忽略重复插入
来源：http://hz.yuxming.cn/gtfpdshmjn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sxryk.cn/gttucaakvk.html

[Q14] 存在则更新（upsert）
来源：http://hz.vqdsnc.cn/gterkknoxr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fengsongda.top/gthmdvdxvg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yj202588.top/gtbstmxvfk.html

[Q15] 查询全部
来源：http://hz.pycfn.com/gtrdtmigfw.html

SELECT * FROM users;
来源：http://hz.ybcxt.top/gttbcpczbt.html

[Q16] 查询指定列
来源：http://hz.ydzc1.top/gtlxqehvit.html

SELECT id, name FROM users;
来源：http://hz.yvedp.cn/gtxltpnsmu.html

[Q17] 条件查询
来源：http://hz.yongpay.top/gtzfkptuah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zycfv.cn/gtlftznwtg.html

[Q18] 模糊匹配
来源：http://hz.jinqigfzy.top/gtxlymmsbc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuanzhike.top/gtuhhqcnmy.html

[Q19] 范围查询
来源：http://hz.chenzaomai.com/gtmzzykdtc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.nanxinkj.top/gtkntigmgp.html

[Q20] IN 列表
来源：http://hz.yvedp.cn/gtlcikduhh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtnkhsztfa.html

[Q21] 空值判断
来源：http://hz.cqqwz.cn/gthoitdcsh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hammf.cn/gtpgvvwduh.html

[Q22] 排序
来源：http://hz.ehwqpu.com/gtniptbcek.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnqzz.top/gtisxptxuy.html

[Q23] 分页
来源：http://hz.yvedp.cn/gtptgfuwwt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigufen.top/gtahkheqsw.html

[Q24] 去重
来源：http://hz.zhoulong.xyz/gthwosplgu.html

SELECT DISTINCT city FROM users;
来源：http://hz.hysaishi.cn/gtfgwqorse.html

[Q25] 只取前 N 条
来源：http://hz.zhoulong.xyz/gtaovtkvhq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ivvv.top/gtlpfzzdgo.html

[Q26] 计数
来源：http://hz.zhixingplan.top/gtdpdtrsrl.html

SELECT COUNT(*) FROM users;
来源：http://hz.dashuyun.cn/gtbneulpio.html

[Q27] 条件计数
来源：http://hz.kuanghao11.cn/gtufzoyebr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tanke756.top/gtwcvgqnrq.html

[Q28] 求和与平均
来源：http://hz.ydzc1.top/gtalzvyftt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.9152youxi.cn/gtzaxohihb.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gtkbmwasip.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gttiopclfc.html

[Q30] 分组统计
来源：http://hz.xuetiantiany.cn/gtpybttiso.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtdrorksgi.html

[Q31] 分组后过滤
来源：http://hz.jinghuilouyu.cn/gtzcrhcrqd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhijiandao.cn/gtyfsjwtuk.html

[Q32] 分组拼接字符串
来源：http://hz.sxryk.cn/gtizymfrbb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtxbkmonmf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hnqzz.top/gtbzapiuek.html

[Q33] 多列分组
来源：http://hz.snrcjt.cn/gtubrrttjr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtpangebpl.html

[Q34] 每组取第一条
来源：http://hz.cqqwz.cn/gtqpojmcfz.html

SELECT * FROM (
来源：http://hz.316326.xyz/gtcirmgcsl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ehwqpu.com/gtfokdxacv.html

) t WHERE rn = 1;
来源：http://hz.hongshengwenyu.top/gtxildgoyw.html

[Q35] 内连接
来源：http://hz.52xcode.cn/gtcorroeup.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtcmjpdrot.html

[Q36] 左连接
来源：http://hz.hnqzz.top/gtpxmckzxl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtmrbkuikg.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtnjfdzswl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yj20258888.top/gtffecnjnm.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.mhx1999.top/gtqotojtmc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hywenlv.cn/gthjvgpftx.html

[Q39] 自连接（查上下级）
来源：http://hz.hywenlv.cn/gthagiqfyb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hongshengwenyu.top/gtkqrftnil.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.52xcode.cn/gtixynuzdp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yonumen.top/gtihilqavc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.chenjidiqi.icu/gtgudqryvr.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtshnifbrs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xylfe.cn/gtpgvpbobk.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gotoacloud.top/gtescjnknq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tian-w.cn/gtkbeqzuhb.html

[Q42] 连接条件附加过滤
来源：http://hz.chenjidiqi.icu/gtcaodbpik.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gttfmdhgpu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sufxvd.cn/gtvranxxyu.html

[Q43] 标量子查询
来源：http://hz.yj202588.top/gtdltrzpjh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuanzx.com/gtzhdvvrcw.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtmdzwmzio.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tianlin.xyz/gtyhlibfgh.html

[Q45] EXISTS 判断存在
来源：http://hz.hysaishi.cn/gteilsvxel.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gthzyhvmpt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.iojbl.cn/gtoxqisbdu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtzjfzzvlm.html

[Q47] 与平均值比较
来源：http://hz.dashuyun.cn/gtguwbcngx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenjidiqi.icu/gtqavedzrs.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtebndatay.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xingfuxueyuan.xyz/gtgsermeie.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cdnleiting.top/gttxbyihxl.html

[Q49] 更新单行
来源：http://hz.fzhhl.top/gthunfgrxb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xziqi.cn/gtvjufdzbz.html

[Q50] 批量更新
来源：http://hz.hnqzz.top/gtajdopxve.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hnxiangtu.top/gtrunfqgcq.html

[Q51] 用子查询更新
来源：http://hz.xinyue.icu/gtumxsxehe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtchcikdxq.html

[Q52] 删除指定行
来源：http://hz.cucudq.cn/gtipgamquk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtknuxcjvg.html

[Q53] 按条件删除
来源：http://hz.shanyushiyangtech.top/gtdgccbxbi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gaohongyu789.top/gtflwsjogu.html

[Q54] 清空表
来源：http://hz.xziqi.cn/gtwvkbgoyv.html

TRUNCATE TABLE logs;
来源：http://hz.aibaodan.cn/gtvegdijgk.html

[Q55] 排名（并列占位）
来源：http://hz.guannengcc.top/gtlprzdmyq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gaohongyu789.top/gtaqzcvrrv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtxaoxfook.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhiwuduotai.top/gtesbksjsb.html

[Q57] 行号
来源：http://hz.mhx1999.top/gtevbyawyj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gteqyvaups.html

[Q58] 累计求和
来源：http://hz.yongpay.top/gtwiyvfovo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtouwrydds.html

[Q59] 分组内累计
来源：http://hz.haohaochexian.top/gtlfjxkqkw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guannengcc.top/gtwvwrrxuu.html

[Q60] 取上一行 / 下一行
来源：http://hz.shanyushiyangtech.top/gttsxrzfkh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tianlin.xyz/gtcpakwpjd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jyoumei.cn/gtwnzgboqy.html

[Q61] 移动平均
来源：http://hz.yuxming.cn/gtwdqzucgo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.aibaodan.cn/gtnzxmsxas.html

[Q62] 分组占比
来源：http://hz.sweek.top/gteleetsva.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtvozcqrzs.html

[Q63] 开启事务
来源：http://hz.sweek.top/gtwgdlbhrp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtwrczousj.html

[Q64] 提交事务
来源：http://hz.xziqi.cn/gtyzbluhjw.html

COMMIT;
来源：http://hz.vqdsnc.cn/gtrgaqjucn.html


<!-- 参考信息 -->