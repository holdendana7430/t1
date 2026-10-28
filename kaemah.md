代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtdwqizlml.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhijiandao.cn/gticgneppk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtzyyxdsyi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtuuzuuive.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwcsuuwsm.html

O. 并发与异步
来源：http://hz.smart0.xyz/gtxruxywoe.html

================================================================================
来源：http://hz.zycfv.cn/gtmnqljimp.html

[O01] 启动一个线程
来源：http://hz.chenlongwang.top/gttdalhhrw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhaomingkeji.xyz/gttgaoalep.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhiwuduotai.top/gtthsqpdjh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtulxoljze.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtrnqlnkhz.html

Java: new Thread(() -> f()).start()
来源：http://hz.wangshuangyany.cn/gtktslygmv.html

Go:   go f()
来源：http://hz.jinqigufen.top/gtgyumcmus.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtwayiljmu.html

C#:   Task.Run(() => F());
来源：http://hz.yj20258.top/gtighbwfnf.html

[O02] 使用线程池
来源：http://hz.jyoumei.cn/gttwssgjkz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.nanxinkj.top/gtdljqqkxo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hfpthk.cn/gtuyoktitd.html

JS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtdqogiqdv.html

TS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtzbjuyryc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xziqi.cn/gtplmrnefa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ehwqpu.com/gtmuhkbcyq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shuidangran.top/gtltsampkb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenzaomai.com/gtmwrypgjj.html

[O03] 加锁保护共享数据
来源：http://hz.guowangkeji.top/gtkdsyknbf.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtrkinlrxa.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtqfayfpsl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gogol.net.cn/gthylgqguy.html

TS:   // 同 JS
来源：http://hz.jinyuanbaomall.cn/gttbsjtuax.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgfzy.top/gtlsajjviy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.iojbl.cn/gtaheorczn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xylfe.cn/gtwbvcwyet.html

C#:   lock (gate) { shared++; }
来源：http://hz.nwbrower.top/gtqjnakowf.html

[O04] 定义异步函数并等待
来源：http://hz.zhixingplan.top/gtinnuytpx.html

Py:   async def f():⏎    await g()
来源：http://hz.zycfv.cn/gtidagnndf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxinkj.top/gtytgrcgsw.html

JS:   async function f() { await g(); }
来源：http://hz.ydjk.org.cn/gtoypvdcue.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pycfn.com/gturoukcsv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.meibo888.top/gtyidiydbh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtgtsouxad.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aizwys.cn/gtmvugonsk.html

C#:   async Task F() { await G(); }
来源：http://hz.andypj.xyz/gtgtgkilng.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtinlfwjlm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shuidangran.top/gtphloitex.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinghuilouyu.cn/gtxwyifuux.html

JS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtprdrtaox.html

TS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gtxwngzeye.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hysaishi.cn/gtzafjckhe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigufen.top/gtxikaijhj.html

Ruby: threads.map(&:join)
来源：http://hz.jinyuanbaomall.cn/gttnkupdwg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhaomingkeji.xyz/gtefmluljm.html

[O06] 使用进程池
来源：http://hz.birdmap.top/gtdsmylfdx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shuidangran.top/gtiuxvihus.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hongshengwenyu.top/gtwyaglozf.html

JS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gtrhnzlneg.html

TS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gthkuomjgi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.quarkkingdee.top/gtziklxzgj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinyuanbaomall.cn/gtilizpive.html

Ruby: // fork 块
来源：http://hz.cdnleiting.top/gtgrgofknw.html

C#:   Parallel.For
来源：http://hz.sweek.top/gtovqarkoe.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtmbgvryns.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtwiuctvay.html

================================================================================
来源：http://hz.ivvv.top/gthbmnkhre.html

[P01] 生成 UUID
来源：http://hz.ydjk.org.cn/gtzvizypnp.html

Py:   str(uuid.uuid4())
来源：http://hz.redwolf501.top/gtcrmarsly.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xinyue.icu/gtjcevlxww.html

JS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtwftbsawa.html

TS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gthtrxrqhx.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtqrddtgwm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yangfankeji.com/gttssomfqk.html

Ruby: SecureRandom.uuid
来源：http://hz.meibo888.top/gtnfmlhbpm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.dashuyun.cn/gtfiuyygzj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuanzx.com/gtyhfrvmgj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cqqwz.cn/gtteplmivo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jianghu66.top/gtesqqlbkd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.smart0.xyz/gtycuwrwwo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.c1oappe.top/gtoahxeeog.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ybcxt.top/gtjhjdiumz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shanyushiyangtech.top/gtmaouamdr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.316326.xyz/gtoabefwyu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yanxiufei.cn/gtgponlhis.html

[P03] 生成短随机字符串
来源：http://hz.shangyingyoupin.top/gtvkkwljwd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.daria6918.cn/gtcmitaelp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuetiantiany.cn/gtpetebvcn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtgptzotmz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtayahzukb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gthqxctbeb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.yj202588.top/gthyhuzhcz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangtech.top/gtwylvtkim.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yanxiufei.cn/gtpgokxfpv.html

[P04] 求长度
来源：http://hz.shanyushiyangkeji.top/gtxwpgqqhf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtflnpevkq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtozduslpb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yonumen.top/gtbvpsxlvl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ybcxt.top/gtgsqylved.html

Java: list.size();  map.size();  s.length()
来源：http://hz.quarkkingdee.top/gtfrnkcowm.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtkdgxxwqa.html

Ruby: x.length;  x.size
来源：http://hz.yj20258.top/gtqardtrjq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xuanzx.com/gtwsytwuqq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenjidiqi.icu/gtonidjnzi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jqgfzy.top/gtrxooimir.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fzhhl.top/gtyissuwiq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.birdmap.top/gtlvuxstvq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtbeiwjbgu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jianghu66.top/gtwqdhfqan.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jqgfzy.top/gtbohphbam.html

Ruby: a == b
来源：http://hz.jianghu66.top/gtoesgydcu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.pengpengdd.cyou/gtomlhjwoa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ppjwa.cn/gthnawnxvd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ybcxt.top/gtiyykszza.html

PHP:  if (empty($x)) {}
来源：http://hz.hfpthk.cn/gthhygmtui.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.nwbrower.top/gtkanmiwxe.html

TS:   if (x == null) {}
来源：http://hz.andypj.xyz/gtkympkhbz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtmkwxqguj.html

Go:   if x == nil {}
来源：http://hz.zhengqikj.top/gtvoyzqids.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtwyfxfblg.html

C#:   if (x is null) {}
来源：http://hz.svipenyu.cn/gtgkgqrqvo.html

[P07] 防抖与节流
来源：http://hz.shzxlz.cn/gtdhziezev.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuanzhike.top/gttkfbsbck.html

PHP:  // 手写时间戳比较
来源：http://hz.cashguo.top/gtigqgejgi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtsdxgpobo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtxtntpeei.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ydjk.org.cn/gtdljqghpp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.gaohongyu789.top/gtpahtkpuj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sweek.top/gtheabswin.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yanxiufei.cn/gtahuorxog.html

[P08] 处理浮点精度问题
来源：http://hz.sufxvd.cn/gtxdcyumqy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigfzy.top/gtkthknuha.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj202588.top/gtuludjfiv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.bjfxy.top/gtrwfytgwb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinyuanbaomall.cn/gtgitljqaj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuanzhike.top/gtgzuizmad.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yongpay.top/gtyjtayjki.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.svipenyu.cn/gtlymuzpmr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hongshengwenyu.top/gttnrzeocr.html

================================================================================
来源：http://hz.zhengqikj.top/gttxzonxjt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yvedp.cn/gtusiqvkza.html

================================================================================
来源：http://hz.svipenyu.cn/gthvqgmgfm.html

[Q01] 创建表
来源：http://hz.fengsongda.top/gtmckabbsx.html

CREATE TABLE users (
来源：http://hz.birdmap.top/gtbtzowqvf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtjiksmcix.html

name VARCHAR(50) NOT NULL,
来源：http://hz.kuanghao11.cn/gtqllpllzc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xuetiantiany.cn/gtybhtidhf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.pengpengdd.cyou/gtnmeoeism.html

);
来源：http://hz.ydjk.org.cn/gtqgpmciyy.html

[Q02] 创建带外键的表
来源：http://hz.jyoumei.cn/gtkusxcizg.html

CREATE TABLE orders (
来源：http://hz.yj202588.top/gtfzweelbh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cqqwz.cn/gtdqctunvh.html

user_id INT NOT NULL,
来源：http://hz.fengsongda.top/gtmzvwqvks.html

amount DECIMAL(10, 2),
来源：http://hz.cheryme.top/gtblujppsu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.sysykeji.top/gtobvbokqz.html

);
来源：http://hz.zhiwuduotai.top/gtlksgdgit.html

[Q03] 增加列
来源：http://hz.zycfv.cn/gtlonncedx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.aibaodan.cn/gtzxphomtj.html

[Q04] 修改列类型
来源：http://hz.fzhhl.top/gtwnerwvvh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhoulong.xyz/gtqydxiwoh.html

[Q05] 重命名列
来源：http://hz.svipenyu.cn/gtbncruztg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.andypj.xyz/gtrgzamkvk.html

[Q06] 删除列
来源：http://hz.mhx1999.top/gtpcdpymvn.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gtaxkhlwlj.html

[Q07] 删除表
来源：http://hz.tian-w.cn/gtjjhkgnrl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangkeji.top/gtcpewsljz.html

[Q08] 创建普通索引
来源：http://hz.zhiwuduotai.top/gtacejgkbl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtmjwlnqjg.html

[Q09] 创建唯一索引
来源：http://hz.yonumen.top/gtbefemepd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.mhx1999.top/gtlywcawtu.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gtuduoewux.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gttwseognb.html

[Q11] 一次插入多行
来源：http://hz.9152youxi.cn/gtmhkpxifs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.tianlin.xyz/gtpzzoqkfq.html

[Q12] 插入后取自增 ID
来源：http://hz.snrcjt.cn/gtsgetvwzi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shuidangran.top/gtxzpcwouc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangkeji.top/gtzllmgojk.html

[Q13] 忽略重复插入
来源：http://hz.yj202588.top/gtycxnilor.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hammf.cn/gtvvbndqen.html

[Q14] 存在则更新（upsert）
来源：http://hz.9152youxi.cn/gtrjkdyszl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhiwuduotai.top/gtkebqorio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ybcxt.top/gtresasoic.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtqmdhjhqf.html

SELECT * FROM users;
来源：http://hz.dashuyun.cn/gtuhrligoe.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtsecfmrfg.html

SELECT id, name FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtliazfebm.html

[Q17] 条件查询
来源：http://hz.xinyue.icu/gtckgfpzho.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.chenzaomai.com/gtmhlyprgb.html

[Q18] 模糊匹配
来源：http://hz.jlsjyb.cn/gtvozaizbc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cashguo.top/gtndrvbjij.html

[Q19] 范围查询
来源：http://hz.wangdashe.top/gtmsqzzoyi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yanxiufei.cn/gtgveehitt.html

[Q20] IN 列表
来源：http://hz.gzhubu.top/gtvehipbvt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xinyue.icu/gtsantgdmt.html

[Q21] 空值判断
来源：http://hz.zhoulong.xyz/gtnlvswixl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gtarywezit.html

[Q22] 排序
来源：http://hz.hfpthk.cn/gtpruqtvtz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gttbqquhzq.html

[Q23] 分页
来源：http://hz.xuanzx.com/gtvteesslc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.vqdsnc.cn/gtcsijnfpv.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtmuomoxax.html

SELECT DISTINCT city FROM users;
来源：http://hz.ywan-chungtsiang.top/gtvggqfxac.html

[Q25] 只取前 N 条
来源：http://hz.fzhhl.top/gtyaubosgd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gteftznlee.html

[Q26] 计数
来源：http://hz.gotoacloud.top/gtmmwrbffk.html

SELECT COUNT(*) FROM users;
来源：http://hz.mhx1999.top/gtyfgrxukm.html

[Q27] 条件计数
来源：http://hz.jiagoushi.top/gthnbnfdum.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hfpthk.cn/gtzctcpjnu.html

[Q28] 求和与平均
来源：http://hz.gzhubu.top/gtycxwuxgh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cdnleiting.top/gtubbgiprk.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gtohijtikq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yanxiufei.cn/gthielflnb.html

[Q30] 分组统计
来源：http://hz.dianchejie.cn/gtojwqfxwz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtzytkcxiu.html

[Q31] 分组后过滤
来源：http://hz.cashguo.top/gttoqvklpp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zycfv.cn/gtavqmzzkv.html

[Q32] 分组拼接字符串
来源：http://hz.shzxlz.cn/gticlfnhwk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtelcqocyg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jlsjyb.cn/gtjnkkntld.html

[Q33] 多列分组
来源：http://hz.hnxiangtu.top/gtfpghlqaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnqzz.top/gtemxzvnmo.html

[Q34] 每组取第一条
来源：http://hz.yj20258888.top/gtddtymzbn.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gtckeemwbs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtlpqsrrhc.html

) t WHERE rn = 1;
来源：http://hz.sufxvd.cn/gtgduwujjm.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gttwjsmuaq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.0kj1m.cn/gtpvbhvdvx.html

[Q36] 左连接
来源：http://hz.shanyushiyangkeji.top/gthbzplnmd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtdjooxoxf.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtjqieodrr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhongyouzk.top/gtnemyjtng.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zdqjudy.top/gtwkqonesk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cheryme.top/gtofnnqfgv.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtgrdgomwe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hammf.cn/gtyrkghgvv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jianghu66.top/gtjmbhkzjo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtyjvcvvgg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhijiandao.cn/gtporpogoh.html

[Q41] 多表连接
来源：http://hz.yongpay.top/gttupezhno.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.haohaochexian.top/gtfyrwyvpr.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gtsvwizsxn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhixingplan.top/gtwbxobvam.html

[Q42] 连接条件附加过滤
来源：http://hz.ydjk.org.cn/gttiqqsljw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jlsjyb.cn/gtckexftud.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dianchejie.cn/gtcruhyguj.html

[Q43] 标量子查询
来源：http://hz.xingfuxueyuan.xyz/gtvxynooom.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.0kj1m.cn/gtqymkikay.html

[Q44] IN 子查询
来源：http://hz.tianlin.xyz/gtvowojwcm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinghuilouyu.cn/gtzyjpgzsc.html

[Q45] EXISTS 判断存在
来源：http://hz.bjfxy.top/gtcplnkvgw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gthigaswdj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuxming.cn/gtfgzbajwk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gotoacloud.top/gtustjizxo.html

[Q47] 与平均值比较
来源：http://hz.ybcxt.top/gtzkjaeioe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnqzz.top/gtxhiuuguy.html

[Q48] CTE 公用表表达式
来源：http://hz.zhiwuduotai.top/gttmbyzmzo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yonumen.top/gttryslhps.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.andypj.xyz/gtnonbkeeh.html

[Q49] 更新单行
来源：http://hz.smart0.xyz/gtzuiqyxld.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shzxlz.cn/gtlutxfscw.html

[Q50] 批量更新
来源：http://hz.jinyuanbaomall.cn/gtyoqauemw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xinyue.icu/gtyzekambg.html

[Q51] 用子查询更新
来源：http://hz.yueranfly.top/gtdhfdvgel.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cucudq.cn/gtdwetvzee.html

[Q52] 删除指定行
来源：http://hz.feifeiyinyue.top/gtzuhvqjiq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.c1oappe.top/gtwofrwbnz.html

[Q53] 按条件删除
来源：http://hz.svipenyu.cn/gthphryhss.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jlsjyb.cn/gtvvxyloat.html

[Q54] 清空表
来源：http://hz.0kj1m.cn/gtwcpttuxm.html

TRUNCATE TABLE logs;
来源：http://hz.9152youxi.cn/gtkczvumct.html

[Q55] 排名（并列占位）
来源：http://hz.yuxming.cn/gtsixjfrjr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jlsjyb.cn/gtqrbnsefg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gttxfpvnqb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgufenzy.top/gtmwzgwhkh.html

[Q57] 行号
来源：http://hz.xinyue.icu/gtafnhssis.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gtdvrhhlpm.html

[Q58] 累计求和
来源：http://hz.c1oappe.top/gtxkjgekak.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gtnibousmb.html

[Q59] 分组内累计
来源：http://hz.yangfankeji.com/gtbjzcpeti.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zdqjudy.top/gtgdopntmf.html

[Q60] 取上一行 / 下一行
来源：http://hz.feifeiyinyue.top/gtqqzlerxk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangdashe.top/gtljybkxyi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aibaodan.cn/gtsuehrqdm.html

[Q61] 移动平均
来源：http://hz.zhongyouzk.top/gtytmcjbmm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtmvizarwy.html

[Q62] 分组占比
来源：http://hz.dianchejie.cn/gtptofmpix.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtfeizyral.html

[Q63] 开启事务
来源：http://hz.yvedp.cn/gthghdjqfd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.chenzaomai.com/gtgfpuyvry.html

[Q64] 提交事务
来源：http://hz.sysykeji.top/gtesitmlae.html

COMMIT;
来源：http://hz.guannengcc.top/gttqqwgtzi.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gtqlvmdakq.html

ROLLBACK;
来源：http://hz.fzhhl.top/gtwonpjfog.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gtkoipzhnf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gttxzcypnq.html

[Q67] 设置隔离级别
来源：http://hz.jianghu66.top/gtfhnfkqra.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtszvgoydz.html

[Q68] 保存点
来源：http://hz.jqgfzy.top/gtbokvqygb.html

SAVEPOINT sp1;
来源：http://hz.fzhhl.top/gtainnriug.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gtmqdwnbeo.html

[Q69] 查看执行计划
来源：http://hz.hysaishi.cn/gtzisjbngu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hfpthk.cn/gtzvmzhuao.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtrivgjhhn.html


<!-- 参考信息 -->