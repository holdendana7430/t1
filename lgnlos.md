代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.vqdsnc.cn/gtsvqxbcwk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jlsjyb.cn/gtlyaugsgj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtgnvcyhkl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jlsjyb.cn/gtyggcurup.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtmujfmpww.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgfzy.top/gtjajyvuav.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj202588.top/gtijtrgdwf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sufxvd.cn/gtynauwerm.html

================================================================================
来源：http://hz.gotoacloud.top/gtnrmxsboi.html

O. 并发与异步
来源：http://hz.ydzc1.top/gtlhwekeac.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtukzyefzq.html

[O01] 启动一个线程
来源：http://hz.hywenlv.cn/gtxynhvzbh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhoulong.xyz/gtjeuapcbq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hysaishi.cn/gtoydssyax.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.9152youxi.cn/gtgaqunsex.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtdakgluwi.html

Java: new Thread(() -> f()).start()
来源：http://hz.ybcxt.top/gtbfhzluye.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtxjallrfm.html

Ruby: Thread.new { f }
来源：http://hz.daxiang520.top/gtczmxqeck.html

C#:   Task.Run(() => F());
来源：http://hz.jinqigufen.top/gtmbdjnoti.html

[O02] 使用线程池
来源：http://hz.chenjidiqi.icu/gtchryxcjw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jlsjyb.cn/gtoxpuynud.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.iojbl.cn/gtjsgxvbug.html

JS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtncplxfle.html

TS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtceqtoevf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gtxgsfcanp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yonumen.top/gtwlgqeeju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258888.top/gtfnfybzrt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tianlin.xyz/gtkcejmagj.html

[O03] 加锁保护共享数据
来源：http://hz.zhoulong.xyz/gtscuhcmix.html

Py:   with lock: shared += 1
来源：http://hz.birdmap.top/gtdeudnjwp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhijiandao.cn/gtccidinpk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yueranfly.top/gtdmtwvzyy.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtqkwclbox.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxuanxn.top/gtvedejzvr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtdvbbskfe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sxryk.cn/gtovdnladz.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgfzy.top/gttikbkczs.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gttesmsxek.html

Py:   async def f():⏎    await g()
来源：http://hz.sweek.top/gtokdhrxjj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtwvyteija.html

JS:   async function f() { await g(); }
来源：http://hz.redwolf501.top/gtxyawqevq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgufenzy.top/gtmcvfjaqy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.316326.xyz/gtrmmbtmth.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aibaodan.cn/gtdzutvvlv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtfucnfedt.html

C#:   async Task F() { await G(); }
来源：http://hz.zycfv.cn/gtwnjaotkn.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuetiantiany.cn/gtbhxpmvyt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.0kj1m.cn/gtwhkwnzzw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtznfcaejd.html

JS:   await Promise.all(tasks)
来源：http://hz.ydzc1.top/gtnkfuqvay.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigufen.top/gthzmngaqy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtmwgosgiv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtayelatfo.html

Ruby: threads.map(&:join)
来源：http://hz.yangfankeji.com/gtuytcjahq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tianlin.xyz/gtgbzxpnsx.html

[O06] 使用进程池
来源：http://hz.316326.xyz/gtsisvwrmj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gzhubu.top/gtyldrxzrn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hysaishi.cn/gtzllqhygq.html

JS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtnuauexqy.html

TS:   // child_process / cluster 模块
来源：http://hz.hysaishi.cn/gtonwgrnwh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pengpengdd.cyou/gtbnfeqkbs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yonumen.top/gtddklizwl.html

Ruby: // fork 块
来源：http://hz.jinqigufen.top/gtrvdssual.html

C#:   Parallel.For
来源：http://hz.zhixingplan.top/gtxkvpqmhj.html

================================================================================
来源：http://hz.haohaochexian.top/gttmpdhwlx.html

P. 常用工具函数
来源：http://hz.yonumen.top/gtongltkla.html

================================================================================
来源：http://hz.hywenlv.cn/gtlegdhgxf.html

[P01] 生成 UUID
来源：http://hz.mhx1999.top/gtmajkdnlf.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gtysedtluq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.vqdsnc.cn/gtidcdbnse.html

JS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtyufjvlyx.html

TS:   crypto.randomUUID()
来源：http://hz.iojbl.cn/gtnfrysnns.html

Java: UUID.randomUUID().toString()
来源：http://hz.bjfxy.top/gtrtheggew.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtwynfcohb.html

Ruby: SecureRandom.uuid
来源：http://hz.c1oappe.top/gtkefvrqmf.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gttwyagafn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ehwqpu.com/gtwqqykpjq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinqigufen.top/gtyccaqmtx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuanzx.com/gtifuxwxvu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gtalupxeez.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gtuysqppmw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cdnleiting.top/gtbzxhuhfo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.ehwqpu.com/gtsslqnmwi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hongshengwenyu.top/gtprqepaqq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nanxuanxn.top/gtlggllmxd.html

[P03] 生成短随机字符串
来源：http://hz.guannengcc.top/gtpzysxxpr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xylfe.cn/gtnhhzhwba.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yangfankeji.com/gtvsmjgilz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hammf.cn/gtwnhbklhg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtzwsemudk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258.top/gtuwpiffdo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tanke756.top/gthtjptsaj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.bjfxy.top/gtkaicucsd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gotoacloud.top/gtdpelpuez.html

[P04] 求长度
来源：http://hz.daria6918.cn/gtcgtqvnun.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dianchejie.cn/gtorjnsfsd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtrwqdcwpq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtnvxytoyp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinqigufen.top/gtpmlgcuje.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cashguo.top/gtlrvlipry.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258888.top/gtfpcqmbuh.html

Ruby: x.length;  x.size
来源：http://hz.iojbl.cn/gttdjngxff.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yvedp.cn/gtzpfekvct.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtftohyjpe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.316326.xyz/gtxexygoyq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gogol.net.cn/gtgwcxolep.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.havefunace.top/gtxytortvb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj202588.top/gtufkcibzk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigfzy.top/gtvbmlcfxb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hysaishi.cn/gtmkkslola.html

Ruby: a == b
来源：http://hz.yongpay.top/gtyabzbakd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daria6918.cn/gtiltzsyko.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fengsongda.top/gtpgljzrbh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.bjfxy.top/gtgmnczjzv.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gtirybrnhx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gtdcayfssw.html

TS:   if (x == null) {}
来源：http://hz.gotoacloud.top/gtweqdtgfh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yueranfly.top/gtcmtfzdgv.html

Go:   if x == nil {}
来源：http://hz.feifeiyinyue.top/gtvrmfixjb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhaomingkeji.xyz/gtxamhprva.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gthoajiynw.html

[P07] 防抖与节流
来源：http://hz.yj20258.top/gteqmjzcnl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.andypj.xyz/gtlhwbjnhx.html

PHP:  // 手写时间戳比较
来源：http://hz.feifeiyinyue.top/gtjqnuqbew.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtlrakppwe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gzhubu.top/gtzncahgyp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.c1oappe.top/gtngfqfzss.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xuanzx.com/gtckkwsosd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnqzz.top/gtqivzsiky.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.316326.xyz/gtqeupquxq.html

[P08] 处理浮点精度问题
来源：http://hz.aibaodan.cn/gtfnrrfuhr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.redwolf501.top/gtimbdulwk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zycfv.cn/gtocbzcqyf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.snrcjt.cn/gtkfadxhba.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.0kj1m.cn/gtarjsbkfm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.mhx1999.top/gtryzyovca.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dashuyun.cn/gtvntpzevi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gthbpkhsty.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cashguo.top/gteqnzpbad.html

================================================================================
来源：http://hz.jianghu66.top/gtoszkhmaq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhixingplan.top/gtcbhibcog.html

================================================================================
来源：http://hz.xinyue.icu/gtndiagipq.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtxekeeked.html

CREATE TABLE users (
来源：http://hz.havefunace.top/gttgipmhnt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtlyydnfbi.html

name VARCHAR(50) NOT NULL,
来源：http://hz.haohaochexian.top/gtkepaqvvi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.havefunace.top/gtohgdiyji.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cqqwz.cn/gtimgikhwl.html

);
来源：http://hz.yangfankeji.com/gtgydhkwpv.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtlcpeghrr.html

CREATE TABLE orders (
来源：http://hz.fzhhl.top/gtkvxewycs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangshuangyany.cn/gtplfxzvso.html

user_id INT NOT NULL,
来源：http://hz.sufxvd.cn/gtcyjsmekj.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gtksywzodh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ydzc1.top/gtynzvvzhx.html

);
来源：http://hz.shzxlz.cn/gtqmwpwoyj.html

[Q03] 增加列
来源：http://hz.tianlin.xyz/gtpvmuwiir.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.sufxvd.cn/gtlooraubh.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtmnovqzur.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinqigufen.top/gtmzbyomxy.html

[Q05] 重命名列
来源：http://hz.ydjk.org.cn/gtqdnmmivl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.tian-w.cn/gtyggsuuhe.html

[Q06] 删除列
来源：http://hz.zdqjudy.top/gtxcxbsuic.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ywan-chungtsiang.top/gtsdsiogkl.html

[Q07] 删除表
来源：http://hz.ybcxt.top/gtqlvjhvwc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.guowangkeji.top/gtjykcqdfy.html

[Q08] 创建普通索引
来源：http://hz.dianchejie.cn/gtufvejftg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ydzc1.top/gtkegqbwjq.html

[Q09] 创建唯一索引
来源：http://hz.0kj1m.cn/gtejvibtpc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtnngjwsfq.html

[Q10] 插入单行
来源：http://hz.shanyushiyangkeji.top/gtpuyswiab.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtnghyyucc.html

[Q11] 一次插入多行
来源：http://hz.chenjidiqi.icu/gtxcujjoav.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.feifeiyinyue.top/gtrsnbotmd.html

[Q12] 插入后取自增 ID
来源：http://hz.bjfxy.top/gtodpwghje.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangshuangyany.cn/gtyeoagkhg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgufenzy.top/gtjbfdicuu.html

[Q13] 忽略重复插入
来源：http://hz.ywan-chungtsiang.top/gtxdavhdnp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xziqi.cn/gtbyxeyvta.html

[Q14] 存在则更新（upsert）
来源：http://hz.yongpay.top/gtkskrxflg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtrdazwfth.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.havefunace.top/gtiayfjuog.html

[Q15] 查询全部
来源：http://hz.jinqigufen.top/gttlsnnhyw.html

SELECT * FROM users;
来源：http://hz.jqgfzy.top/gtscrdusbp.html

[Q16] 查询指定列
来源：http://hz.hnqzz.top/gtlkhvlegd.html

SELECT id, name FROM users;
来源：http://hz.tian-w.cn/gtcvouccss.html

[Q17] 条件查询
来源：http://hz.pycfn.com/gtaxouihhp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sysykeji.top/gttdgmvuxd.html

[Q18] 模糊匹配
来源：http://hz.tianlin.xyz/gtpgsknkns.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shangyingyoupin.top/gtottfeulu.html

[Q19] 范围查询
来源：http://hz.yanxiufei.cn/gtgfuajdhb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.tanke756.top/gtnntiybmi.html

[Q20] IN 列表
来源：http://hz.meibo888.top/gtopuaiawm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.bjfxy.top/gtvixsmift.html

[Q21] 空值判断
来源：http://hz.iojbl.cn/gtdtdeejij.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gthmohiyky.html

[Q22] 排序
来源：http://hz.dashuyun.cn/gtlaycxrhb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sufxvd.cn/gtxsiyvxbr.html

[Q23] 分页
来源：http://hz.andypj.xyz/gtysrqzoau.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.52xcode.cn/gtedhjbvcw.html

[Q24] 去重
来源：http://hz.cheryme.top/gtertxojdb.html

SELECT DISTINCT city FROM users;
来源：http://hz.sweek.top/gtskafcdia.html

[Q25] 只取前 N 条
来源：http://hz.zhongyouzk.top/gtzbhxapmm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhaomingkeji.xyz/gtruwixzui.html

[Q26] 计数
来源：http://hz.hammf.cn/gtudhjxuab.html

SELECT COUNT(*) FROM users;
来源：http://hz.zycfv.cn/gtunjlvtmr.html

[Q27] 条件计数
来源：http://hz.mhx1999.top/gttsmptuao.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ydjk.org.cn/gtyqecgkqz.html

[Q28] 求和与平均
来源：http://hz.sweek.top/gtjjmgrjuv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jqgfzy.top/gtwsxfoqky.html

[Q29] 最大最小值
来源：http://hz.svipenyu.cn/gtqwkyhxhs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hywenlv.cn/gthsnerrxx.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtxixfpxzj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtgrefpjro.html

[Q31] 分组后过滤
来源：http://hz.hnxiangtu.top/gtrxgivsxt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.iojbl.cn/gtrdjmyeap.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtmslmaqxv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hongshengwenyu.top/gtefgiucke.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gthmybfbte.html

[Q33] 多列分组
来源：http://hz.sxryk.cn/gtwtjeunjm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.havefunace.top/gtelnewwbp.html

[Q34] 每组取第一条
来源：http://hz.zhiwuduotai.top/gtpbpstalw.html

SELECT * FROM (
来源：http://hz.cqqwz.cn/gtiwvnqsls.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xinyue.icu/gtrlhifmio.html

) t WHERE rn = 1;
来源：http://hz.hnxiangtu.top/gtxssrobcj.html

[Q35] 内连接
来源：http://hz.316326.xyz/gtdrdjllbe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgufenzy.top/gtndiyugfc.html

[Q36] 左连接
来源：http://hz.hywenlv.cn/gtxmuqfcez.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtcetgfcyp.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtscckvvec.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nwbrower.top/gtnjrxbphj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhoulong.xyz/gtjidrbbbw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.mhx1999.top/gtxixxlmwn.html

[Q39] 自连接（查上下级）
来源：http://hz.havefunace.top/gtlkmrmktx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtrcpkmdwn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zycfv.cn/gtyqbxhtig.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhoulong.xyz/gthxvkowlr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daxiang520.top/gtusjxokjz.html

[Q41] 多表连接
来源：http://hz.hnqzz.top/gtkvhvszyh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gaohongyu789.top/gtelwgpaae.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258.top/gtckxqrthi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ywan-chungtsiang.top/gtsmyfsmoz.html

[Q42] 连接条件附加过滤
来源：http://hz.xinyue.icu/gtwizsfomy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.vqdsnc.cn/gtqfcrdxqy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yvedp.cn/gtuiefwhrf.html

[Q43] 标量子查询
来源：http://hz.shuidangran.top/gtpziqqtpc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pengpengdd.cyou/gtpaamkxta.html

[Q44] IN 子查询
来源：http://hz.316326.xyz/gtodsqgflv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jlsjyb.cn/gtxfmuhzxi.html

[Q45] EXISTS 判断存在
来源：http://hz.hysaishi.cn/gtajlmmlqg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pycfn.com/gtpexbkyqi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.9152youxi.cn/gtrwerrolf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangshuangyany.cn/gtrbrqakth.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangtech.top/gtuvzysloc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.birdmap.top/gtatapwmes.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtvqrqiazp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.316326.xyz/gtievvmbhz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hongshengwenyu.top/gtrwdnincf.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtmkzowlsb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtmjdgqddv.html

[Q50] 批量更新
来源：http://hz.pengpengdd.cyou/gtucczqyiu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.havefunace.top/gtdigqqklh.html

[Q51] 用子查询更新
来源：http://hz.andypj.xyz/gtoikbvuzw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gtrmlgxntk.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtthxhhgsq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zycfv.cn/gtufbqojyr.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtuyzzypjw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtddakgjgi.html

[Q54] 清空表
来源：http://hz.jyoumei.cn/gtypichhno.html

TRUNCATE TABLE logs;
来源：http://hz.cucudq.cn/gtwaovwzlc.html

[Q55] 排名（并列占位）
来源：http://hz.snrcjt.cn/gtewvbxoss.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nwbrower.top/gtbztqwghk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhijiandao.cn/gtgezmiscs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.mhx1999.top/gtzoecyjwt.html

[Q57] 行号
来源：http://hz.ehwqpu.com/gtwzttjuht.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenlongwang.top/gtosrogdby.html

[Q58] 累计求和
来源：http://hz.zhongyouzk.top/gtmdlaaoly.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hongshengwenyu.top/gtmgsnvnqz.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gtiyfpnokv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cqqwz.cn/gtiumrcldz.html

[Q60] 取上一行 / 下一行
来源：http://hz.meibo888.top/gtxysoaxhn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigufen.top/gteuzlijar.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtjwaactni.html

[Q61] 移动平均
来源：http://hz.zhongyouzk.top/gtmdvkgecv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtbxtqhlqp.html

[Q62] 分组占比
来源：http://hz.0kj1m.cn/gtvhrckqyy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtxafxpvka.html

[Q63] 开启事务
来源：http://hz.c1oappe.top/gtzkvnlgbe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gttteosqpv.html

[Q64] 提交事务
来源：http://hz.pengpengdd.cyou/gtoldooter.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtiibeoevb.html

[Q65] 回滚事务
来源：http://hz.sweek.top/gtxsvddsza.html

ROLLBACK;
来源：http://hz.zhengqikj.top/gtsuotlfxc.html

[Q66] 行锁查询
来源：http://hz.cucudq.cn/gtnskdwkuu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtzjwbcncj.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtposjucnx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aibaodan.cn/gtbbjndbzu.html

[Q68] 保存点
来源：http://hz.shanyushiyangkeji.top/gtsfksgshq.html

SAVEPOINT sp1;
来源：http://hz.cucudq.cn/gtqcuiaprt.html


<!-- 参考信息 -->