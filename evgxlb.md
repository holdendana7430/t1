代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtcsidlxzl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.svipenyu.cn/gthkzgbtva.html

[N11] 二叉树中序遍历
来源：http://hz.hnxiangtu.top/gtfvlsihcp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhiwuduotai.top/gtxnhzxviu.html

PHP:  // 手写递归函数
来源：http://hz.svipenyu.cn/gtoujfqwyq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtjzaxzirl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtdpvlulbi.html

Java: // 手写递归
来源：http://hz.jianghu66.top/gtrnjrzthf.html

Go:   // 手写递归
来源：http://hz.ivvv.top/gtgdyqsezb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuanzhike.top/gtwlphvfti.html

C#:   // 手写递归
来源：http://hz.gotoacloud.top/gtmhvfvvwf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.feifeiyinyue.top/gtuhdxrrxv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinqigufen.top/gtcwkvszur.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtovjkpnxb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtjruujbgi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gteyvkrazx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtmbgmfjui.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gogol.net.cn/gtrwoklqng.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtolclxset.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhongyouzk.top/gttixzjevh.html

================================================================================
来源：http://hz.9152youxi.cn/gtffsbcojs.html

O. 并发与异步
来源：http://hz.dashuyun.cn/gtploscvao.html

================================================================================
来源：http://hz.nanxuanxn.top/gtuakltunp.html

[O01] 启动一个线程
来源：http://hz.havefunace.top/gtbiahkpmh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yangfankeji.com/gtlrfurgqe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtbjlavzye.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gtbkgrckku.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtmnryoghf.html

Java: new Thread(() -> f()).start()
来源：http://hz.dianchejie.cn/gtmqrcrjmd.html

Go:   go f()
来源：http://hz.tianlin.xyz/gtaejrwdnd.html

Ruby: Thread.new { f }
来源：http://hz.yj202588.top/gtoxeamffa.html

C#:   Task.Run(() => F());
来源：http://hz.pycfn.com/gtazdqsjaj.html

[O02] 使用线程池
来源：http://hz.zhiwuduotai.top/gtmddkpsxl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tanke756.top/gthvpquwdt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhengqikj.top/gtnvhbbkvh.html

JS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtbbrnubtr.html

TS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtfqgdtguk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinghuilouyu.cn/gtpzgwyibc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ywan-chungtsiang.top/gtbhlrlxcj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hnxiangtu.top/gtvuhjoijc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fengsongda.top/gtnymulqqk.html

[O03] 加锁保护共享数据
来源：http://hz.fzhhl.top/gtxzyevnvz.html

Py:   with lock: shared += 1
来源：http://hz.hnxiangtu.top/gtwvohlzyz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hongshengwenyu.top/gtflznkejg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zycfv.cn/gtqjtfzgzt.html

TS:   // 同 JS
来源：http://hz.zhiwuduotai.top/gtjenwtogk.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gtucudujzp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhongyouzk.top/gtpagzkgae.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ivvv.top/gtkrkxhkab.html

C#:   lock (gate) { shared++; }
来源：http://hz.sweek.top/gtpsrnzgib.html

[O04] 定义异步函数并等待
来源：http://hz.cheryme.top/gtlevlddsc.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtyrlronpz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtfjpfceex.html

JS:   async function f() { await g(); }
来源：http://hz.zhixingplan.top/gtssgutuuy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxinkj.top/gtmdruzgoj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydzc1.top/gtrehuijnt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gteyiisdig.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yanxiufei.cn/gtdtvpwcbu.html

C#:   async Task F() { await G(); }
来源：http://hz.zhixingplan.top/gtwqbgxypf.html

[O05] 并发执行并等待全部完成
来源：http://hz.tanke756.top/gtrnofqknb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtrkkqnlwg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgfzy.top/gtvjgweqam.html

JS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtiqefcsyy.html

TS:   await Promise.all(tasks)
来源：http://hz.cqqwz.cn/gtjyeumgoo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangshuangyany.cn/gtyagroizc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhaomingkeji.xyz/gtogrmowpi.html

Ruby: threads.map(&:join)
来源：http://hz.guannengcc.top/gtbtwwbggi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tianlin.xyz/gtxllopymn.html

[O06] 使用进程池
来源：http://hz.ehwqpu.com/gtewkuuyum.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sxryk.cn/gtymrssrkt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtfkzgagac.html

JS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gtuvmevvfu.html

TS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtzjfkoafz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.feifeiyinyue.top/gtuoymgbye.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gtpjjtnqsn.html

Ruby: // fork 块
来源：http://hz.jianghu66.top/gtwunqmnyg.html

C#:   Parallel.For
来源：http://hz.jiagoushi.top/gtmsysmujq.html

================================================================================
来源：http://hz.birdmap.top/gtwseeotjk.html

P. 常用工具函数
来源：http://hz.52xcode.cn/gtfjponxae.html

================================================================================
来源：http://hz.havefunace.top/gtufbjejap.html

[P01] 生成 UUID
来源：http://hz.nwbrower.top/gtbuvnovkx.html

Py:   str(uuid.uuid4())
来源：http://hz.ydjk.org.cn/gttwesuxrc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ywan-chungtsiang.top/gtpbgqsyks.html

JS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtpzvhuwop.html

TS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtpaxmrbgs.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gtbzhzrwxo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jlsjyb.cn/gtrzjckwho.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gteohdnxpx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.meibo888.top/gtweqsmcot.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nwbrower.top/gtictomgyg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhixingplan.top/gtjvilsocv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sysykeji.top/gtselljuos.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtcmypdbbm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tian-w.cn/gtlvnelzyg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinyuanbaomall.cn/gtaiwyygwo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gzhubu.top/gtpmhsadkf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jyoumei.cn/gtbrtzkfmo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.316326.xyz/gtedpmcreg.html

[P03] 生成短随机字符串
来源：http://hz.jinghuilouyu.cn/gtbjyhjiio.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hysaishi.cn/gtqcxepjik.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinqigufen.top/gtmoedhypp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtuzuhctyn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gteovfeyoh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtkvgbltbl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.smart0.xyz/gtponluwyu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.havefunace.top/gtgvfrkzkd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hfpthk.cn/gtkdjgwdqa.html

[P04] 求长度
来源：http://hz.chenlongwang.top/gtklqjzbtz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jianghu66.top/gtxrbrxipb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtpdivbbuz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtglujlknj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtwlvxbudn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhiwuduotai.top/gtmsidnzgq.html

Go:   len(arr);  len(m)
来源：http://hz.yongpay.top/gttdhshlzk.html

Ruby: x.length;  x.size
来源：http://hz.cqqwz.cn/gtgbtjaxej.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pengpengdd.cyou/gtqbxubcqf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj202588.top/gtpqjyspqh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.52xcode.cn/gtxlsyrcyr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xylfe.cn/gtjohkdotc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ppjwa.cn/gtqxbmzbqh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtcrgbnqso.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.meibo888.top/gtoybdzjvd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guowangkeji.top/gtgvqkaepr.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtcocslvsp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xylfe.cn/gtnxkyusip.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gzhubu.top/gtrjffquus.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.andypj.xyz/gtzerehihn.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtmpjwhzfj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ywan-chungtsiang.top/gtxydqngyt.html

TS:   if (x == null) {}
来源：http://hz.zhaomingkeji.xyz/gtrnssixcy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cashguo.top/gtavmrocjf.html

Go:   if x == nil {}
来源：http://hz.cashguo.top/gtitgebzww.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gtpslpqedx.html

C#:   if (x is null) {}
来源：http://hz.aibaodan.cn/gtnilbtgnj.html

[P07] 防抖与节流
来源：http://hz.cqqwz.cn/gttrulvsey.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gthlnrfrrv.html

PHP:  // 手写时间戳比较
来源：http://hz.guowangkeji.top/gtewxnzxih.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgufenzy.top/gtncvadaaq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtymuxhhzv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fzhhl.top/gtdvgqpngm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.bjfxy.top/gtkcblqudk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj202588.top/gtrjsshshy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhoulong.xyz/gtynydayuk.html

[P08] 处理浮点精度问题
来源：http://hz.jiagoushi.top/gtvgihgklt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hammf.cn/gtrujgwbda.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shanyushiyangkeji.top/gtnvadzqti.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jqgufenzy.top/gtdvzuzkgn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jiagoushi.top/gtxaxbpvah.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nwbrower.top/gtwxbsolgh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xuetiantiany.cn/gtvsujjbqz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.meibo888.top/gtvjhsivqr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shzxlz.cn/gtphfiwshk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjxsdguxi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guowangkeji.top/gtfcnauddf.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtglscybwd.html

[Q01] 创建表
来源：http://hz.yj20258888.top/gtiuixqail.html

CREATE TABLE users (
来源：http://hz.wangdashe.top/gtaoopewuk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtnbfqbgct.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ivvv.top/gtrpqcbhms.html

email VARCHAR(100) UNIQUE,
来源：http://hz.nwbrower.top/gthtepvgtk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sxryk.cn/gtbqnzfnxa.html

);
来源：http://hz.zhongyouzk.top/gtceyzuxkq.html

[Q02] 创建带外键的表
来源：http://hz.fzhhl.top/gtgjptxwcj.html

CREATE TABLE orders (
来源：http://hz.nanxinkj.top/gthedzrlbs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.fzhhl.top/gtyqneougt.html

user_id INT NOT NULL,
来源：http://hz.mhx1999.top/gticasdipl.html

amount DECIMAL(10, 2),
来源：http://hz.gzhubu.top/gtcagflpic.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yueranfly.top/gtkcshpydm.html

);
来源：http://hz.yuanzhike.top/gtvmqeevoy.html

[Q03] 增加列
来源：http://hz.zdqjudy.top/gtppeffrqh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gogol.net.cn/gtcuobayma.html

[Q04] 修改列类型
来源：http://hz.yj20258.top/gtnnhiqfgv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sxryk.cn/gttgqstekb.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtohravjot.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xinyue.icu/gtudsfszrp.html

[Q06] 删除列
来源：http://hz.shuidangran.top/gtiqtlglzx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gtslsaoged.html

[Q07] 删除表
来源：http://hz.ehwqpu.com/gtvbdrdvlx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gzhubu.top/gtuhnjdldf.html

[Q08] 创建普通索引
来源：http://hz.hnqzz.top/gtifcciaxk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cucudq.cn/gtrnvdmhtm.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtllyfzccv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtahcpbrgu.html

[Q10] 插入单行
来源：http://hz.meibo888.top/gtctqwcbmx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.mhx1999.top/gtzrxgierh.html

[Q11] 一次插入多行
来源：http://hz.zhoulong.xyz/gtnvnisobi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinghuilouyu.cn/gtyjoeiobf.html

[Q12] 插入后取自增 ID
来源：http://hz.ppjwa.cn/gtfswgpxxt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtharszxqi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinqigfzy.top/gttfcyhzvw.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtybtckcjx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gtenplvmoc.html

[Q14] 存在则更新（upsert）
来源：http://hz.jiagoushi.top/gtnqksmfcn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.haohaochexian.top/gtnicawtba.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuetiantiany.cn/gtqvirwgks.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtpfshhhwm.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtlbtxcnoj.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtyrishsrd.html

SELECT id, name FROM users;
来源：http://hz.jiagoushi.top/gtjsenstod.html

[Q17] 条件查询
来源：http://hz.bjfxy.top/gtoivnnnpc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zdqjudy.top/gtugdyhgla.html

[Q18] 模糊匹配
来源：http://hz.zhaomingkeji.xyz/gtxabrlbov.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jinqigfzy.top/gtffwmbtjf.html

[Q19] 范围查询
来源：http://hz.kuanghao11.cn/gtryqnddrk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shangyingyoupin.top/gtuykjlfle.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gtpmmdnkeh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.wangdashe.top/gtrgtlgirr.html

[Q21] 空值判断
来源：http://hz.tianlin.xyz/gteqwzojdm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xingfuxueyuan.xyz/gtdxcoulyc.html

[Q22] 排序
来源：http://hz.yongpay.top/gtuxdrlhsc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258888.top/gtnopsnybg.html

[Q23] 分页
来源：http://hz.quarkkingdee.top/gtanwwaiyn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtrusmtefg.html

[Q24] 去重
来源：http://hz.hysaishi.cn/gtzqksguus.html

SELECT DISTINCT city FROM users;
来源：http://hz.havefunace.top/gttsguensa.html

[Q25] 只取前 N 条
来源：http://hz.gogol.net.cn/gtrcuioilo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangshuangyany.cn/gtyfjmrdey.html

[Q26] 计数
来源：http://hz.andypj.xyz/gtzfhawdbt.html

SELECT COUNT(*) FROM users;
来源：http://hz.ybcxt.top/gtevkocyec.html

[Q27] 条件计数
来源：http://hz.chenlongwang.top/gtpdvelxsw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jianghu66.top/gttxdlvwpl.html

[Q28] 求和与平均
来源：http://hz.ydjk.org.cn/gtuzbtwdhe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtavfbcqth.html

[Q29] 最大最小值
来源：http://hz.andypj.xyz/gtbgqyjyke.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtiwlksjyb.html

[Q30] 分组统计
来源：http://hz.zhijiandao.cn/gtqurzompp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gtxapaysyj.html

[Q31] 分组后过滤
来源：http://hz.jinqigfzy.top/gtvzizfetv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinyuanbaomall.cn/gtpreqlxms.html

[Q32] 分组拼接字符串
来源：http://hz.haohaochexian.top/gtxgcglqbt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtlkpbsblj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fengsongda.top/gtlerqstar.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtcikabtat.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhijiandao.cn/gtcyikjfmg.html

[Q34] 每组取第一条
来源：http://hz.xuanzx.com/gtnyyruglu.html

SELECT * FROM (
来源：http://hz.vqdsnc.cn/gthluzdxwt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.nanxuanxn.top/gtqrhxbpbh.html

) t WHERE rn = 1;
来源：http://hz.wangshuangyany.cn/gtwmivnakd.html

[Q35] 内连接
来源：http://hz.nwbrower.top/gtpwamlvxu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtkmkuzfgb.html

[Q36] 左连接
来源：http://hz.zdqjudy.top/gtlnikfgow.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gthetebtiz.html

[Q37] 右连接
来源：http://hz.tianlin.xyz/gtlxqsithb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hongshengwenyu.top/gtvvsefmnb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.meibo888.top/gtisdrqgni.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hysaishi.cn/gtpxkaehgr.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gteslmsewa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj202588.top/gtfhaxmgth.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xinyue.icu/gtycevspwf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.pengpengdd.cyou/gttnuqvcoc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.smart0.xyz/gtjzfilwee.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtnopeszuu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guannengcc.top/gtwlypqdhj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xinyue.icu/gtvunkifie.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aizwys.cn/gtjbbtvbil.html

[Q42] 连接条件附加过滤
来源：http://hz.gogol.net.cn/gtaljeohta.html

SELECT u.name, o.amount FROM users u
来源：http://hz.0kj1m.cn/gttxvokhmk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jiagoushi.top/gtskhtfalb.html

[Q43] 标量子查询
来源：http://hz.vqdsnc.cn/gtsvknzhxr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtktiobvmi.html

[Q44] IN 子查询
来源：http://hz.wangdashe.top/gtoqkgkffj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gogol.net.cn/gtvjkquwry.html

[Q45] EXISTS 判断存在
来源：http://hz.jinyuanbaomall.cn/gtcytzmbcz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jqgufenzy.top/gtgdxuxfwp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gttpllqucx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtfzkocith.html

[Q47] 与平均值比较
来源：http://hz.birdmap.top/gtdtrduoxd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtxtwfmavu.html

[Q48] CTE 公用表表达式
来源：http://hz.zhengqikj.top/gtgbgpyyfz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtrgkmpzcz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jqgfzy.top/gtzvibazax.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gtlgzpwntr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtifvtoibw.html

[Q50] 批量更新
来源：http://hz.zhijiandao.cn/gtalhtkwyl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.meibo888.top/gtwwgjkdtc.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gtqpxfjnkw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtvpjdvvqv.html

[Q52] 删除指定行
来源：http://hz.bjfxy.top/gtvxagzbcp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtskvivcwi.html

[Q53] 按条件删除
来源：http://hz.xuanzx.com/gtdugjopbf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenlongwang.top/gtqpltzukf.html

[Q54] 清空表
来源：http://hz.yj202588.top/gtiztskqbc.html

TRUNCATE TABLE logs;
来源：http://hz.bjfxy.top/gtckmdbfxz.html

[Q55] 排名（并列占位）
来源：http://hz.jqgufenzy.top/gtvevkvebw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yongpay.top/gtmvcruicd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cqqwz.cn/gtnmehoqwm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guannengcc.top/gtcyvejtna.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtkzgfknal.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigufen.top/gtwzhklbus.html

[Q58] 累计求和
来源：http://hz.yuxming.cn/gtrcpqkark.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gtlpucocje.html

[Q59] 分组内累计
来源：http://hz.haohaochexian.top/gtkzdclqit.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xylfe.cn/gtoqpaaffw.html

[Q60] 取上一行 / 下一行
来源：http://hz.ydzc1.top/gtnlzzzfas.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.quarkkingdee.top/gttkffbtdk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ppjwa.cn/gtruleiene.html

[Q61] 移动平均
来源：http://hz.jinqigfzy.top/gtybsyismx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cheryme.top/gtfpiejosq.html

[Q62] 分组占比
来源：http://hz.gogol.net.cn/gtobfqpjwp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtuazphubo.html


<!-- 参考信息 -->