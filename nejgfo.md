代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gtewnzrfrj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnqzz.top/gtcyzotsmh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtlltcyfiz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtuhbkyivo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gthkersjdq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.meibo888.top/gtxylsejhu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.smart0.xyz/gtscbdtghq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gtxtjsvuzh.html

================================================================================
来源：http://hz.jinqigufen.top/gttzovcxjl.html

O. 并发与异步
来源：http://hz.vqdsnc.cn/gttkivzmdr.html

================================================================================
来源：http://hz.yueranfly.top/gtkalklwsm.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtpkyrddso.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtsefabkqe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigufen.top/gtniihwgln.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gogol.net.cn/gtixlckdex.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtzkecnxcq.html

Java: new Thread(() -> f()).start()
来源：http://hz.ybcxt.top/gtwbamjoro.html

Go:   go f()
来源：http://hz.svipenyu.cn/gthlroglsh.html

Ruby: Thread.new { f }
来源：http://hz.zhoulong.xyz/gtwtpadeza.html

C#:   Task.Run(() => F());
来源：http://hz.havefunace.top/gtvnslugsb.html

[O02] 使用线程池
来源：http://hz.guowangkeji.top/gtpzxifzsq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.aibaodan.cn/gthypmphdh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gzhubu.top/gtwikqgdsb.html

JS:   // worker_threads 线程池
来源：http://hz.gogol.net.cn/gtwyqqrppr.html

TS:   // worker_threads 线程池
来源：http://hz.316326.xyz/gtdjfaeyxi.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtgkabwnyp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinghuilouyu.cn/gtnrkpcxwv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.havefunace.top/gtvlbzeuoq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tianlin.xyz/gtoytsbkub.html

[O03] 加锁保护共享数据
来源：http://hz.jlsjyb.cn/gtcjkxtsoj.html

Py:   with lock: shared += 1
来源：http://hz.c1oappe.top/gtbbyqzsnw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtiyyacqug.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jiagoushi.top/gtkqhqfzmf.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtnnysmfgv.html

Java: synchronized (this) { shared++; }
来源：http://hz.jyoumei.cn/gtjhfdcmgp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtcqadfnpc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.redwolf501.top/gtpcqccvyp.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtietxohpf.html

[O04] 定义异步函数并等待
来源：http://hz.svipenyu.cn/gtaskeoier.html

Py:   async def f():⏎    await g()
来源：http://hz.birdmap.top/gtqcckeqbk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtjvepjcnk.html

JS:   async function f() { await g(); }
来源：http://hz.c1oappe.top/gtpzzpeyne.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtcyudgosu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gaohongyu789.top/gtplyopwpk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.smart0.xyz/gtycigxwhh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtgitjucvh.html

C#:   async Task F() { await G(); }
来源：http://hz.gogol.net.cn/gtytqcmaav.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gtyxnanilj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shanyushiyangtech.top/gtrfnmrofq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.sxryk.cn/gtooustkwe.html

JS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtxzqvwejr.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtdzyzxcju.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtsuqgnsrs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtajslckqu.html

Ruby: threads.map(&:join)
来源：http://hz.snrcjt.cn/gtkixpfxkp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jinyuanbaomall.cn/gteurtnjti.html

[O06] 使用进程池
来源：http://hz.hywenlv.cn/gtnajoqtmk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.kuanghao11.cn/gtqnphmkqq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtulteaimz.html

JS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtpeoypecj.html

TS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtcemwmmuu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gtsyreqsuj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtmjhleeyr.html

Ruby: // fork 块
来源：http://hz.yangfankeji.com/gtuxdfsbai.html

C#:   Parallel.For
来源：http://hz.yj20258.top/gtjxfksnsq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtaxhnmlwr.html

P. 常用工具函数
来源：http://hz.aizwys.cn/gtluwlaybf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmrvtsouq.html

[P01] 生成 UUID
来源：http://hz.xingfuxueyuan.xyz/gtdjobsufm.html

Py:   str(uuid.uuid4())
来源：http://hz.hnqzz.top/gtomypwugb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cucudq.cn/gteempyojh.html

JS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtddmfapss.html

TS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtnmhnoexr.html

Java: UUID.randomUUID().toString()
来源：http://hz.cheryme.top/gtwnakddru.html

Go:   // 用 github.com/google/uuid
来源：http://hz.9152youxi.cn/gtukhrjtjc.html

Ruby: SecureRandom.uuid
来源：http://hz.gogol.net.cn/gtzwlwngfz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.redwolf501.top/gtefaoouvj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinghuilouyu.cn/gtisbtxlbn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.svipenyu.cn/gtrperdamb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hysaishi.cn/gtywmipyhs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tian-w.cn/gtoxqeszvk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.redwolf501.top/gtfwodaqpi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.316326.xyz/gtzmrrleuj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtzsjhddpx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.feifeiyinyue.top/gtezmqntcx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zdqjudy.top/gthtugfxnp.html

[P03] 生成短随机字符串
来源：http://hz.c1oappe.top/gtvzblpbhj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sufxvd.cn/gtkuxtxwrx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jianghu66.top/gtigejjsvf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnqzz.top/gtcrtimakg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtigcuaizc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jianghu66.top/gtrouldntf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.c1oappe.top/gtrxcdzhbz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.quarkkingdee.top/gtjinvdsop.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.andypj.xyz/gtwiivdjzj.html

[P04] 求长度
来源：http://hz.meibo888.top/gtattfixvz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xylfe.cn/gtcdutuhsl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtxhjpdrqk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenlongwang.top/gtkmjvgave.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuanzx.com/gtlyvjwxyn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.bjfxy.top/gtkhaypuen.html

Go:   len(arr);  len(m)
来源：http://hz.shuidangran.top/gtvymdishk.html

Ruby: x.length;  x.size
来源：http://hz.gzhubu.top/gtfxpezjam.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ppjwa.cn/gtzdculvmi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yanxiufei.cn/gttwudsteg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ivvv.top/gturzbgvjm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.haohaochexian.top/gtheblhabr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtarbbfsxv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.nanxuanxn.top/gtjphgyzho.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.pengpengdd.cyou/gtbmvtibft.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.tanke756.top/gtjkfyxfia.html

Ruby: a == b
来源：http://hz.haohaochexian.top/gthzbmucvr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gotoacloud.top/gtbvyisijo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gtvqcuotfz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sweek.top/gtozcyaajr.html

PHP:  if (empty($x)) {}
来源：http://hz.fengsongda.top/gtmvukvlgs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.0kj1m.cn/gtxlkvutxv.html

TS:   if (x == null) {}
来源：http://hz.quarkkingdee.top/gtjrnnyqln.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtyoezypsn.html

Go:   if x == nil {}
来源：http://hz.hfpthk.cn/gtkgmqwyds.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.0kj1m.cn/gtinnpfbua.html

C#:   if (x is null) {}
来源：http://hz.0kj1m.cn/gtujfijzrg.html

[P07] 防抖与节流
来源：http://hz.cheryme.top/gtnobfzgcx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hongshengwenyu.top/gtsssgsnxf.html

PHP:  // 手写时间戳比较
来源：http://hz.jinqigfzy.top/gtbiulypcw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhongyouzk.top/gtbrdguuqm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtiaanncuk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.andypj.xyz/gtchtkjhbz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.tian-w.cn/gtpkxrevlh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jqgfzy.top/gtbkpfbkwq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.guannengcc.top/gtidwtzbss.html

[P08] 处理浮点精度问题
来源：http://hz.gotoacloud.top/gtpumwtkho.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shanyushiyangtech.top/gtrjqxmxim.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ppjwa.cn/gtwpohqjal.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenlongwang.top/gtsvoxllyp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigufen.top/gtvxlkqfxq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ppjwa.cn/gteollggzn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cashguo.top/gtluwtlumj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cashguo.top/gtcvibearl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.kuanghao11.cn/gtvvahcvvn.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtbuivqlxd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hammf.cn/gtylclgxhl.html

================================================================================
来源：http://hz.9152youxi.cn/gtrbfruheo.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtuulroxxb.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtkghacibh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtdmyuvcol.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hnxiangtu.top/gtjtawlvmh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gtvedurnti.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hysaishi.cn/gtpisdnkxr.html

);
来源：http://hz.jyoumei.cn/gtvihiohwt.html

[Q02] 创建带外键的表
来源：http://hz.chenzaomai.com/gtaimmpebm.html

CREATE TABLE orders (
来源：http://hz.svipenyu.cn/gtruhndufu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtorjdfbbz.html

user_id INT NOT NULL,
来源：http://hz.redwolf501.top/gtkhuqxthu.html

amount DECIMAL(10, 2),
来源：http://hz.shuidangran.top/gtuvezmgoy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.havefunace.top/gtaehopzlu.html

);
来源：http://hz.havefunace.top/gtpyapprnw.html

[Q03] 增加列
来源：http://hz.xziqi.cn/gtudxrsjrw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.feifeiyinyue.top/gtpexfwrgl.html

[Q04] 修改列类型
来源：http://hz.aibaodan.cn/gtplerqotw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ppjwa.cn/gtzpgyoznf.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtehyiufoh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jiagoushi.top/gtgyhbvsif.html

[Q06] 删除列
来源：http://hz.gzhubu.top/gtyyeaezth.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.fzhhl.top/gtodtjkeas.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gthagfqjoj.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yueranfly.top/gtxywgmrca.html

[Q08] 创建普通索引
来源：http://hz.zhiwuduotai.top/gtgglqtqxd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtjefuxflp.html

[Q09] 创建唯一索引
来源：http://hz.hnqzz.top/gtaeyyofob.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jianghu66.top/gtzhtlikwa.html

[Q10] 插入单行
来源：http://hz.nanxuanxn.top/gtwyfedvkq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yj20258.top/gtvmoupppo.html

[Q11] 一次插入多行
来源：http://hz.jlsjyb.cn/gtivkykhll.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sufxvd.cn/gtlhmkrpxw.html

[Q12] 插入后取自增 ID
来源：http://hz.hongshengwenyu.top/gtyrfaskte.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yvedp.cn/gtqwkycyrb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gogol.net.cn/gtpmszlhky.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gtvwxzdgpd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhongyouzk.top/gtiqamjbcc.html

[Q14] 存在则更新（upsert）
来源：http://hz.redwolf501.top/gtmgtbwrjw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxinkj.top/gteytxffnq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhijiandao.cn/gtfkmnqclz.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtbncpkyxi.html

SELECT * FROM users;
来源：http://hz.pengpengdd.cyou/gtxmnbawkc.html

[Q16] 查询指定列
来源：http://hz.fzhhl.top/gtnzgsfcir.html

SELECT id, name FROM users;
来源：http://hz.fzhhl.top/gtbkfycrbi.html

[Q17] 条件查询
来源：http://hz.jyoumei.cn/gtorsuiydd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.shangyingyoupin.top/gtkzrrvkkp.html

[Q18] 模糊匹配
来源：http://hz.zdqjudy.top/gtdprubmli.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhixingplan.top/gtkypenyuj.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtffuexwph.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ivvv.top/gtdtipkzss.html

[Q20] IN 列表
来源：http://hz.shangyingyoupin.top/gtpcajgiif.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gogol.net.cn/gtyliiqpqi.html

[Q21] 空值判断
来源：http://hz.zdqjudy.top/gtklydwyht.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xziqi.cn/gtawjdgjma.html

[Q22] 排序
来源：http://hz.haohaochexian.top/gtepiubyqo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hongshengwenyu.top/gtmynjfjmj.html

[Q23] 分页
来源：http://hz.yj20258.top/gtlqpieflf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinghuilouyu.cn/gtmyhsssye.html

[Q24] 去重
来源：http://hz.yangfankeji.com/gtzhrobawa.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnqzz.top/gtqztagtsd.html

[Q25] 只取前 N 条
来源：http://hz.jinghuilouyu.cn/gtdtwgrims.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gogol.net.cn/gtlxkukvfu.html

[Q26] 计数
来源：http://hz.ppjwa.cn/gtizxrcobl.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtcppijait.html

[Q27] 条件计数
来源：http://hz.xuanzx.com/gtrnwaghxz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangdashe.top/gtzezwoffu.html

[Q28] 求和与平均
来源：http://hz.zhixingplan.top/gtdxiiseam.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gthorptfbx.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtnizhyxgo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtbpomsuzr.html

[Q30] 分组统计
来源：http://hz.zhoulong.xyz/gtaiovkboa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtgfqhzzow.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gttjfbpecm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.vqdsnc.cn/gtchizknbz.html

[Q32] 分组拼接字符串
来源：http://hz.cqqwz.cn/gtjfcgarkj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtbtgsqqek.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ybcxt.top/gtpltnoxog.html

[Q33] 多列分组
来源：http://hz.ybcxt.top/gtsjloqkmr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gogol.net.cn/gtkqothnho.html

[Q34] 每组取第一条
来源：http://hz.ehwqpu.com/gtaeynfjnv.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gtyxmmvdtj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.pengpengdd.cyou/gtmsydvhlu.html

) t WHERE rn = 1;
来源：http://hz.hnqzz.top/gtwudkbcoe.html

[Q35] 内连接
来源：http://hz.yueranfly.top/gtsyiudrhd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtgndhufeb.html

[Q36] 左连接
来源：http://hz.jinqigufen.top/gtuenfrmds.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtaoawtowv.html

[Q37] 右连接
来源：http://hz.pengpengdd.cyou/gttfhpdlot.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.andypj.xyz/gthixetnaa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fengsongda.top/gtavacdats.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.sufxvd.cn/gtofndfgor.html

[Q39] 自连接（查上下级）
来源：http://hz.nanxuanxn.top/gtbsdlmnqz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.52xcode.cn/gthyzckzcy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gtzgqmrcra.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhixingplan.top/gtoxfdgxyf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yuanzhike.top/gtdjybscnw.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtzltahcwk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.meibo888.top/gtufttqwjw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.dianchejie.cn/gtexmhagkd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gtuqctpyqu.html

[Q42] 连接条件附加过滤
来源：http://hz.guowangkeji.top/gtmtddgqde.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jyoumei.cn/gtrynwakpd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.vqdsnc.cn/gtcrbnafax.html

[Q43] 标量子查询
来源：http://hz.52xcode.cn/gtjqpujffz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jianghu66.top/gtrjpdwvyr.html

[Q44] IN 子查询
来源：http://hz.sxryk.cn/gtugannyen.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yueranfly.top/gtpogrkfeo.html

[Q45] EXISTS 判断存在
来源：http://hz.chenjidiqi.icu/gtpjyybjeh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtecvizbhw.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cucudq.cn/gtmzeiskae.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtbqfnnjgq.html

[Q47] 与平均值比较
来源：http://hz.jyoumei.cn/gtcmgooutl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258.top/gtbjulwplm.html

[Q48] CTE 公用表表达式
来源：http://hz.birdmap.top/gtswtzuhiz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xinyue.icu/gtazffysbt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.birdmap.top/gtwncejagq.html

[Q49] 更新单行
来源：http://hz.cqqwz.cn/gtmhuizaql.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.redwolf501.top/gtyqceztut.html

[Q50] 批量更新
来源：http://hz.yongpay.top/gtjoezbxvp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.dashuyun.cn/gtqorwwzbn.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtbvzlwbhn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zycfv.cn/gthzlleakh.html

[Q52] 删除指定行
来源：http://hz.gotoacloud.top/gtniabslvh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.snrcjt.cn/gtnmstzgly.html

[Q53] 按条件删除
来源：http://hz.hysaishi.cn/gtlahqyrah.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydjk.org.cn/gtwwjqtill.html

[Q54] 清空表
来源：http://hz.gotoacloud.top/gtsgxcfhzf.html

TRUNCATE TABLE logs;
来源：http://hz.zhaomingkeji.xyz/gtdloqlqeh.html

[Q55] 排名（并列占位）
来源：http://hz.yongpay.top/gtxmmrdhvi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuanzhike.top/gtkrtjabzr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnxiangtu.top/gthdyefauk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hfpthk.cn/gtdbfoatkd.html

[Q57] 行号
来源：http://hz.gotoacloud.top/gtdoazmzvn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guowangkeji.top/gtbzydlkmv.html

[Q58] 累计求和
来源：http://hz.sweek.top/gtklmvawcg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.quarkkingdee.top/gtbcijlvyy.html

[Q59] 分组内累计
来源：http://hz.yuanzhike.top/gtdmzjmdse.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgfzy.top/gtqerxialo.html

[Q60] 取上一行 / 下一行
来源：http://hz.havefunace.top/gtucdtcftc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtpcidkxvz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yangfankeji.com/gtljmryyre.html

[Q61] 移动平均
来源：http://hz.dashuyun.cn/gtnpwvbtvb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nwbrower.top/gtqekmdpzm.html

[Q62] 分组占比
来源：http://hz.shuidangran.top/gtzxjusnzj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gthuygikrx.html

[Q63] 开启事务
来源：http://hz.zhixingplan.top/gtjldbnqpw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gticguzxws.html

[Q64] 提交事务
来源：http://hz.xingfuxueyuan.xyz/gtumifkcng.html

COMMIT;
来源：http://hz.redwolf501.top/gtfrrbwbor.html

[Q65] 回滚事务
来源：http://hz.c1oappe.top/gtdmslunye.html

ROLLBACK;
来源：http://hz.yj202588.top/gtypwgmora.html

[Q66] 行锁查询
来源：http://hz.9152youxi.cn/gtmraqwyhl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.snrcjt.cn/gtfbqkyuwc.html

[Q67] 设置隔离级别
来源：http://hz.ybcxt.top/gttlgkzvuc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangdashe.top/gtiukiwdsu.html

[Q68] 保存点
来源：http://hz.jinghuilouyu.cn/gtqftousvt.html

SAVEPOINT sp1;
来源：http://hz.smart0.xyz/gtiejlnxwr.html


<!-- 参考信息 -->