代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtaolfahhq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ppjwa.cn/gtjzorcgbs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ppjwa.cn/gttlytkbhv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.mhx1999.top/gtctjemcwi.html

================================================================================
来源：http://hz.hammf.cn/gttwkgfhuo.html

O. 并发与异步
来源：http://hz.sweek.top/gtmoakwuoz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzdbnkyrf.html

[O01] 启动一个线程
来源：http://hz.xuetiantiany.cn/gtmazfdncb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hysaishi.cn/gtltqkbwee.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenjidiqi.icu/gtthnsicgb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhaomingkeji.xyz/gtqmstrusy.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gtklmzxnup.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtnswgsrjg.html

Go:   go f()
来源：http://hz.snrcjt.cn/gthtgznpwp.html

Ruby: Thread.new { f }
来源：http://hz.tian-w.cn/gtougaqkym.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtbuftaijr.html

[O02] 使用线程池
来源：http://hz.guowangkeji.top/gtswwswowi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.snrcjt.cn/gtaflwwoga.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pengpengdd.cyou/gtwhjjwpdj.html

JS:   // worker_threads 线程池
来源：http://hz.hnxiangtu.top/gthblvlnvv.html

TS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtxxpztuza.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xziqi.cn/gtwcgbtzmd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yueranfly.top/gtgwsrvyud.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xylfe.cn/gtuagylymk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gtouipndtg.html

[O03] 加锁保护共享数据
来源：http://hz.tian-w.cn/gtanxtzvsr.html

Py:   with lock: shared += 1
来源：http://hz.dashuyun.cn/gtlfxielno.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.52xcode.cn/gtebmcwbou.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.meibo888.top/gtyppxbrwc.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtlwlkxbhy.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtwaugorju.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fengsongda.top/gtyxjleiht.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gthevntlie.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtomsbduld.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtgegfzuza.html

Py:   async def f():⏎    await g()
来源：http://hz.daria6918.cn/gtxqcibolj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zdqjudy.top/gtobgnnspe.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gtrzchlfmq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinqigfzy.top/gteqbsoodr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gtcoyoghae.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtakmxiayp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenlongwang.top/gtiphapgyd.html

C#:   async Task F() { await G(); }
来源：http://hz.meibo888.top/gtenlgivyi.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangkeji.top/gtnarzorcv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.tian-w.cn/gtidnthpov.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.52xcode.cn/gtwxdzifxo.html

JS:   await Promise.all(tasks)
来源：http://hz.dianchejie.cn/gtycblzlhs.html

TS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtycdpnuhp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yuxming.cn/gtyldqsjes.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.0kj1m.cn/gtylmoogkd.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtkfdakrnj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cdnleiting.top/gtwfhpxduy.html

[O06] 使用进程池
来源：http://hz.yonumen.top/gthjidihhd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxuanxn.top/gtdjsemjar.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.mhx1999.top/gtetbfmarc.html

JS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtfdmouuud.html

TS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtkbfwuvsz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sweek.top/gtmzsglreu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenlongwang.top/gtbqcutypv.html

Ruby: // fork 块
来源：http://hz.feifeiyinyue.top/gtaagonnay.html

C#:   Parallel.For
来源：http://hz.yj20258.top/gtjpmzeiop.html

================================================================================
来源：http://hz.cdnleiting.top/gtuxlchbca.html

P. 常用工具函数
来源：http://hz.daria6918.cn/gtwytrqvci.html

================================================================================
来源：http://hz.yueranfly.top/gtlstyliry.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gtubewerdl.html

Py:   str(uuid.uuid4())
来源：http://hz.wangshuangyany.cn/gtdslkcvst.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hnxiangtu.top/gtkhjwierg.html

JS:   crypto.randomUUID()
来源：http://hz.9152youxi.cn/gtwyodzzki.html

TS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtolpzcwob.html

Java: UUID.randomUUID().toString()
来源：http://hz.bjfxy.top/gtyfvbnkzh.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gtbonhdave.html

Ruby: SecureRandom.uuid
来源：http://hz.aibaodan.cn/gtuouabmmu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.haohaochexian.top/gtnzyphumh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gotoacloud.top/gttopgmyad.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.iojbl.cn/gtfkpljrtm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.iojbl.cn/gtitolohxm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.mhx1999.top/gtrpnnmtyh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhaomingkeji.xyz/gtcziaelhz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sysykeji.top/gtitasrgyn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhongyouzk.top/gtfqwlycio.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cheryme.top/gtbvmezcxr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yanxiufei.cn/gtzhrcnnuh.html

[P03] 生成短随机字符串
来源：http://hz.gzhubu.top/gtuxajkygn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtzzvhuryl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj20258888.top/gtxqmmacdx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guannengcc.top/gtmlvckaof.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cashguo.top/gtxwohhebc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yangfankeji.com/gtzvugyyfz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.mhx1999.top/gtsyiuxgva.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sweek.top/gtqmioylyu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinqigufen.top/gtsrtwthgh.html

[P04] 求长度
来源：http://hz.jinqigufen.top/gtewkfqetd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nwbrower.top/gtgajjkyhx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtmbgagzib.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gogol.net.cn/gtgkrrkkqn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gthgkpflef.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nwbrower.top/gtytqrgmft.html

Go:   len(arr);  len(m)
来源：http://hz.jqgfzy.top/gtonamtysg.html

Ruby: x.length;  x.size
来源：http://hz.jianghu66.top/gtzxevlomp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.pengpengdd.cyou/gtfffjelji.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenzaomai.com/gtiheanjkp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ehwqpu.com/gttdktganr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hysaishi.cn/gtsfzenplo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangdashe.top/gtohjtsmpv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yvedp.cn/gtcjyzfhzj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.dashuyun.cn/gteefejvhy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinyuanbaomall.cn/gtcmfoictg.html

Ruby: a == b
来源：http://hz.tian-w.cn/gtkuilrlrh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gtrcxxykbm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gotoacloud.top/gtghlpjozh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuanzx.com/gtgvzckdqc.html

PHP:  if (empty($x)) {}
来源：http://hz.zhongyouzk.top/gtatafhblp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cqqwz.cn/gtonqyppwb.html

TS:   if (x == null) {}
来源：http://hz.pycfn.com/gtkarzuqxu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.redwolf501.top/gtqdmyxgfc.html

Go:   if x == nil {}
来源：http://hz.nanxuanxn.top/gtxvqrwpnd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtjidkgowc.html

C#:   if (x is null) {}
来源：http://hz.wangdashe.top/gtdaslonvd.html

[P07] 防抖与节流
来源：http://hz.sysykeji.top/gtimpnicmv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangtech.top/gtijjtzvbb.html

PHP:  // 手写时间戳比较
来源：http://hz.pengpengdd.cyou/gtsjvjdmzb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxinkj.top/gtofrcezyn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtrjngazrs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sysykeji.top/gtmkvdbmoq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenjidiqi.icu/gtitgsbftp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gtcmpatpxx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydjk.org.cn/gtqbrjyylo.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gtugqicmmy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtnjiqwtqe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.mhx1999.top/gtmysdupgo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnxiangtu.top/gtqypnkddd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.sweek.top/gtoqibcuah.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yueranfly.top/gtipbyhtlz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtonapjhri.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtvfsiduvw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.tianlin.xyz/gtugznamlj.html

================================================================================
来源：http://hz.haohaochexian.top/gtboehfosd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sxryk.cn/gtpiyursof.html

================================================================================
来源：http://hz.tanke756.top/gtqrouwtve.html

[Q01] 创建表
来源：http://hz.guannengcc.top/gtaskqtutz.html

CREATE TABLE users (
来源：http://hz.daria6918.cn/gtnhimrabh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.316326.xyz/gtbgriyiri.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jqgufenzy.top/gtnehpcxbc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yonumen.top/gtqgzkuskl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yongpay.top/gtptusqrfc.html

);
来源：http://hz.hywenlv.cn/gtoqzbmynk.html

[Q02] 创建带外键的表
来源：http://hz.hfpthk.cn/gtzulxgvjv.html

CREATE TABLE orders (
来源：http://hz.zhongyouzk.top/gtrddiveab.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ywan-chungtsiang.top/gtknezpjry.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtfzklyoja.html

amount DECIMAL(10, 2),
来源：http://hz.zycfv.cn/gtgticbwqp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.andypj.xyz/gthgrdtepa.html

);
来源：http://hz.yueranfly.top/gtyfjorbfk.html

[Q03] 增加列
来源：http://hz.ydjk.org.cn/gtgzmfctad.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.guowangkeji.top/gtwjnnrhgd.html

[Q04] 修改列类型
来源：http://hz.ppjwa.cn/gtjestchpn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.mhx1999.top/gtefqmnnjc.html

[Q05] 重命名列
来源：http://hz.yanxiufei.cn/gtapczpsrp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.smart0.xyz/gtpmmeesqv.html

[Q06] 删除列
来源：http://hz.hywenlv.cn/gthquwsbbf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.redwolf501.top/gtevvjvzuw.html

[Q07] 删除表
来源：http://hz.xuetiantiany.cn/gtlkcftkco.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuxming.cn/gtxhlxtscm.html

[Q08] 创建普通索引
来源：http://hz.zhijiandao.cn/gtntjybhke.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtisayearl.html

[Q09] 创建唯一索引
来源：http://hz.chenlongwang.top/gtbohxwlyj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cheryme.top/gtmynstspo.html

[Q10] 插入单行
来源：http://hz.zhijiandao.cn/gtczwizlfw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtcfjnxnwv.html

[Q11] 一次插入多行
来源：http://hz.hammf.cn/gtaodbrfiq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jianghu66.top/gtdlufwhkf.html

[Q12] 插入后取自增 ID
来源：http://hz.yuxming.cn/gtpxnktaht.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.ydzc1.top/gtpyvtyhoe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.svipenyu.cn/gtebplmtmu.html

[Q13] 忽略重复插入
来源：http://hz.pycfn.com/gttbhkmzxi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ywan-chungtsiang.top/gtuozqbigk.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gtxdaxfeyc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.0kj1m.cn/gtbhibzbfn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.sysykeji.top/gtvrxiojcl.html

[Q15] 查询全部
来源：http://hz.ppjwa.cn/gtxkhciojm.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtpvikrkma.html

[Q16] 查询指定列
来源：http://hz.xuanzx.com/gtwpfuennb.html

SELECT id, name FROM users;
来源：http://hz.tian-w.cn/gtuzepgyat.html

[Q17] 条件查询
来源：http://hz.hywenlv.cn/gtufvpexmg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yueranfly.top/gtfcmipcnb.html

[Q18] 模糊匹配
来源：http://hz.gotoacloud.top/gtpfwjzccg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtzcwckjjn.html

[Q19] 范围查询
来源：http://hz.jinghuilouyu.cn/gtdethcwmv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jlsjyb.cn/gtqqakvzsa.html

[Q20] IN 列表
来源：http://hz.meibo888.top/gtrfefobpd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jinqigufen.top/gtcbafjrat.html

[Q21] 空值判断
来源：http://hz.jlsjyb.cn/gttxtynqbq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtnxgiqtip.html

[Q22] 排序
来源：http://hz.zhixingplan.top/gtsmvbwaan.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinyuanbaomall.cn/gtuvrkpmls.html

[Q23] 分页
来源：http://hz.shanyushiyangkeji.top/gtbdanvcjh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cashguo.top/gthgcsztwn.html

[Q24] 去重
来源：http://hz.dianchejie.cn/gtsxkhmwtp.html

SELECT DISTINCT city FROM users;
来源：http://hz.shangyingyoupin.top/gtrixrwzgq.html

[Q25] 只取前 N 条
来源：http://hz.xuanzx.com/gtqrquifpw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuxming.cn/gtcbbwgbpd.html

[Q26] 计数
来源：http://hz.316326.xyz/gtpoadggaq.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtdzggqirg.html

[Q27] 条件计数
来源：http://hz.jinghuilouyu.cn/gtitszmzon.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangkeji.top/gtbpkswcta.html

[Q28] 求和与平均
来源：http://hz.nwbrower.top/gtuutvjtvy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ppjwa.cn/gtbafrakrg.html

[Q29] 最大最小值
来源：http://hz.zhengqikj.top/gtkomgpuie.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cdnleiting.top/gtcnfhozol.html

[Q30] 分组统计
来源：http://hz.jinyuanbaomall.cn/gthfzdqccc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtqthedrnp.html

[Q31] 分组后过滤
来源：http://hz.hnqzz.top/gtdltjrcjc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.feifeiyinyue.top/gtsfsuwzki.html

[Q32] 分组拼接字符串
来源：http://hz.zhongyouzk.top/gtmhufrceq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtjoninmdw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigufen.top/gtfacccbhj.html

[Q33] 多列分组
来源：http://hz.jlsjyb.cn/gtcauychze.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.aibaodan.cn/gtuyekwgro.html

[Q34] 每组取第一条
来源：http://hz.zhongyouzk.top/gtluszdejs.html

SELECT * FROM (
来源：http://hz.snrcjt.cn/gtxnudzitu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gzhubu.top/gtriqywlee.html

) t WHERE rn = 1;
来源：http://hz.nwbrower.top/gtqdtowuss.html

[Q35] 内连接
来源：http://hz.shzxlz.cn/gtpyenwhym.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtqvsnvgxk.html

[Q36] 左连接
来源：http://hz.gaohongyu789.top/gtbdwckhts.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgufenzy.top/gtcglhscli.html

[Q37] 右连接
来源：http://hz.jianghu66.top/gtorbvymii.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ivvv.top/gtvypfxqkw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gtpoddcwuu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.smart0.xyz/gtycomrpdz.html

[Q39] 自连接（查上下级）
来源：http://hz.tian-w.cn/gtuluxubgu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.snrcjt.cn/gtqgraxslv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtuwkxarrj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinyuanbaomall.cn/gtdvkkajpf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zdqjudy.top/gtwnvbctep.html

[Q41] 多表连接
来源：http://hz.cqqwz.cn/gtmagtuiht.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hongshengwenyu.top/gtschxjknf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtqhqyivud.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.tanke756.top/gtyomumbes.html

[Q42] 连接条件附加过滤
来源：http://hz.zhiwuduotai.top/gtsxrbvmef.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangkeji.top/gtccbfjbar.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.smart0.xyz/gtqfafnfdl.html

[Q43] 标量子查询
来源：http://hz.ywan-chungtsiang.top/gtkxjaownk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuetiantiany.cn/gtorxqldsg.html

[Q44] IN 子查询
来源：http://hz.pycfn.com/gtpaoyqddz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtkecipxkb.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtwpucvcxf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtzemlzrcn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daria6918.cn/gttygzereg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtuzgyjbrq.html

[Q47] 与平均值比较
来源：http://hz.xuetiantiany.cn/gtebrtewkq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hysaishi.cn/gtpscocvxi.html

[Q48] CTE 公用表表达式
来源：http://hz.feifeiyinyue.top/gtjqvwwsgz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ehwqpu.com/gtjrbjxbyc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.havefunace.top/gtgdvtlyoy.html

[Q49] 更新单行
来源：http://hz.haohaochexian.top/gtwnhihkbm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtszgiuqyb.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gthuehsypf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangdashe.top/gtznxycurh.html

[Q51] 用子查询更新
来源：http://hz.hysaishi.cn/gtswdcumfq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinqigfzy.top/gtlicxyssy.html

[Q52] 删除指定行
来源：http://hz.xziqi.cn/gtkpgclqbu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258.top/gtfiqhcely.html

[Q53] 按条件删除
来源：http://hz.0kj1m.cn/gtehwnlcik.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guannengcc.top/gtvpnkcjbo.html

[Q54] 清空表
来源：http://hz.jlsjyb.cn/gtgkzmcorx.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gtmwbwxvsj.html

[Q55] 排名（并列占位）
来源：http://hz.iojbl.cn/gtidinfalg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zycfv.cn/gtahgkbwno.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pycfn.com/gtwigpuigh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yvedp.cn/gtveeplyqo.html

[Q57] 行号
来源：http://hz.dashuyun.cn/gtikqbgarj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aibaodan.cn/gtrvtlaeny.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtcsqgqhal.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gtnvafjgmp.html

[Q59] 分组内累计
来源：http://hz.ydjk.org.cn/gtkfgbbnpe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ppjwa.cn/gtuuxzemtm.html

[Q60] 取上一行 / 下一行
来源：http://hz.shzxlz.cn/gtkszdgmxe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yuanzhike.top/gtylmmpapo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jiagoushi.top/gtrkygbzje.html

[Q61] 移动平均
来源：http://hz.iojbl.cn/gttixplqqx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenjidiqi.icu/gtmgmbaqac.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gtoburcmgn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtgdcmmtse.html

[Q63] 开启事务
来源：http://hz.xziqi.cn/gtmeuogyoh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtddisrkuh.html

[Q64] 提交事务
来源：http://hz.yueranfly.top/gtdwzwgnro.html

COMMIT;
来源：http://hz.jinghuilouyu.cn/gtpjnsuyqw.html

[Q65] 回滚事务
来源：http://hz.andypj.xyz/gtmkhcslnm.html

ROLLBACK;
来源：http://hz.c1oappe.top/gtgfjdvpvv.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtdnyuswjn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhaomingkeji.xyz/gtplgtuvli.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtfxlfsejs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hnxiangtu.top/gtxuieeung.html

[Q68] 保存点
来源：http://hz.jiagoushi.top/gthbmfwyfy.html

SAVEPOINT sp1;
来源：http://hz.nwbrower.top/gtbiwenocy.html

ROLLBACK TO sp1;
来源：http://hz.ivvv.top/gtyxunmpak.html

[Q69] 查看执行计划
来源：http://hz.cashguo.top/gtkuikosez.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xuetiantiany.cn/gthnhkzqjr.html

[Q70] 更新统计信息
来源：http://hz.jqgufenzy.top/gtjpmtnenw.html


<!-- 参考信息 -->