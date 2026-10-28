代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://hz.cashguo.top/gtkbvweuyf.html

Go:   go f()
来源：http://hz.daxiang520.top/gtefncobss.html

Ruby: Thread.new { f }
来源：http://hz.jyoumei.cn/gtettdgsvt.html

C#:   Task.Run(() => F());
来源：http://hz.dianchejie.cn/gtkqaztwuj.html

[O02] 使用线程池
来源：http://hz.yongpay.top/gtpnwrzezm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenzaomai.com/gtaopdlhdf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tianlin.xyz/gtdxjntmzj.html

JS:   // worker_threads 线程池
来源：http://hz.aizwys.cn/gtmrzxogin.html

TS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtimmszbwd.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.feifeiyinyue.top/gtlbevofcz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.wangshuangyany.cn/gtbncmbqma.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gthpvcntld.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtyolocgci.html

[O03] 加锁保护共享数据
来源：http://hz.hongshengwenyu.top/gtystbqebw.html

Py:   with lock: shared += 1
来源：http://hz.fengsongda.top/gtldlqtzpo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xingfuxueyuan.xyz/gtwkmtaxrn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinyuanbaomall.cn/gtcwilbymh.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtnegbpibi.html

Java: synchronized (this) { shared++; }
来源：http://hz.jlsjyb.cn/gtlltmxfdo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.316326.xyz/gtagjqbgzq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtooianapk.html

C#:   lock (gate) { shared++; }
来源：http://hz.cqqwz.cn/gtqkqnnfsc.html

[O04] 定义异步函数并等待
来源：http://hz.gzhubu.top/gtuyfbyzuo.html

Py:   async def f():⏎    await g()
来源：http://hz.havefunace.top/gtfnqjamwt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sufxvd.cn/gtomfuuncc.html

JS:   async function f() { await g(); }
来源：http://hz.aizwys.cn/gtvhtjaglf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hongshengwenyu.top/gtfojpunmi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cdnleiting.top/gtphojzepc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigufen.top/gtsjtxdmxi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shuidangran.top/gtupwawuqg.html

C#:   async Task F() { await G(); }
来源：http://hz.tanke756.top/gtmduwpfum.html

[O05] 并发执行并等待全部完成
来源：http://hz.bjfxy.top/gtjbkfkxfy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.aizwys.cn/gtygvchwev.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tanke756.top/gtozygiukl.html

JS:   await Promise.all(tasks)
来源：http://hz.zhixingplan.top/gtufyhhwxv.html

TS:   await Promise.all(tasks)
来源：http://hz.guannengcc.top/gtygwqqdsx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gttypqximp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj20258.top/gtguzoxevw.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtsmkrxiur.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtpkqakmxn.html

[O06] 使用进程池
来源：http://hz.yj20258888.top/gtnqdxderz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtyvyoaioo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gzhubu.top/gtlkxmwtpc.html

JS:   // child_process / cluster 模块
来源：http://hz.hysaishi.cn/gtofmgyqpn.html

TS:   // child_process / cluster 模块
来源：http://hz.tian-w.cn/gtvhlvlbof.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigufen.top/gtocnyhzgm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fzhhl.top/gtfkfnsrcr.html

Ruby: // fork 块
来源：http://hz.snrcjt.cn/gtqzzxlqfx.html

C#:   Parallel.For
来源：http://hz.cucudq.cn/gtkvqpzqed.html

================================================================================
来源：http://hz.jlsjyb.cn/gtqjitltsw.html

P. 常用工具函数
来源：http://hz.nanxinkj.top/gtgwquygmb.html

================================================================================
来源：http://hz.cdnleiting.top/gtulqiccmo.html

[P01] 生成 UUID
来源：http://hz.iojbl.cn/gtaafdhptx.html

Py:   str(uuid.uuid4())
来源：http://hz.hnxiangtu.top/gtjjnldbwd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gaohongyu789.top/gteurmbjed.html

JS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gttlhorxsa.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtzoculeam.html

Java: UUID.randomUUID().toString()
来源：http://hz.quarkkingdee.top/gtzkcrsxol.html

Go:   // 用 github.com/google/uuid
来源：http://hz.svipenyu.cn/gtaylrkewc.html

Ruby: SecureRandom.uuid
来源：http://hz.jinyuanbaomall.cn/gtbinckbkn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtetzfmnfe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtmyuflzzn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aibaodan.cn/gtyhliibdv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gtrkaeooae.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xylfe.cn/gtviwpzrjq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinqigfzy.top/gtipccytpp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aibaodan.cn/gtrovhmceb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtrjqzkzlc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinyuanbaomall.cn/gtqkrudymc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.aizwys.cn/gtahdvhmfv.html

[P03] 生成短随机字符串
来源：http://hz.ywan-chungtsiang.top/gtstqmzbrj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gzhubu.top/gtcrydgmht.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yonumen.top/gtdzqimnje.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xylfe.cn/gtlrxmktug.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtygnpysyu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aibaodan.cn/gtbfsbfrok.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jyoumei.cn/gtzfbtmuzk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.mhx1999.top/gtubpzdsde.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.birdmap.top/gtxmalokox.html

[P04] 求长度
来源：http://hz.xziqi.cn/gttjcxgeis.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daria6918.cn/gtmmnlzplk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtmizrzddr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtjusdxibk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.c1oappe.top/gtdhkflmqw.html

Java: list.size();  map.size();  s.length()
来源：http://hz.vqdsnc.cn/gtmooqzvmk.html

Go:   len(arr);  len(m)
来源：http://hz.yj202588.top/gtjhwjuezd.html

Ruby: x.length;  x.size
来源：http://hz.hysaishi.cn/gtacdpzilu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtcjyhxfou.html

[P05] 判断两个对象内容是否相等
来源：http://hz.bjfxy.top/gtdoablooe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.tianlin.xyz/gttfupklzg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.c1oappe.top/gtdndzpjzs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.feifeiyinyue.top/gtdcvxvoof.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinyuanbaomall.cn/gttmqakmla.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydzc1.top/gtmchnhild.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nwbrower.top/gtmsgwospr.html

Ruby: a == b
来源：http://hz.bjfxy.top/gtiqgksshj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.aibaodan.cn/gtdvfkhwgi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sxryk.cn/gtilopdtkv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtkcvyxclf.html

PHP:  if (empty($x)) {}
来源：http://hz.cucudq.cn/gtctkoxyqn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.feifeiyinyue.top/gtgydplisf.html

TS:   if (x == null) {}
来源：http://hz.zhiwuduotai.top/gtrhlaaywu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.andypj.xyz/gtaqbaslwg.html

Go:   if x == nil {}
来源：http://hz.yvedp.cn/gtwpoqkyef.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtragougjl.html

C#:   if (x is null) {}
来源：http://hz.yj202588.top/gtbmzdtcyw.html

[P07] 防抖与节流
来源：http://hz.sweek.top/gtvsshwcdj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.cashguo.top/gtcipgdgkr.html

PHP:  // 手写时间戳比较
来源：http://hz.gotoacloud.top/gttsmbievt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtoernskbx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtpbozbsnx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.tanke756.top/gtynplkeay.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangtech.top/gtvfurdxgc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zdqjudy.top/gthmpmxpib.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tianlin.xyz/gtnsdhftuj.html

[P08] 处理浮点精度问题
来源：http://hz.yvedp.cn/gtvfbybshu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.aibaodan.cn/gtaajoeihh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258.top/gtmbsylwuc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daxiang520.top/gtbjezilod.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinghuilouyu.cn/gtbdizpase.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cdnleiting.top/gtnankvbvy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hysaishi.cn/gtpbsbwrvw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gaohongyu789.top/gtwgjutwux.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhoulong.xyz/gtmxpdbmdq.html

================================================================================
来源：http://hz.yj20258888.top/gtpqjahfyn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gzhubu.top/gtnnwphkgc.html

================================================================================
来源：http://hz.tanke756.top/gtoborigzn.html

[Q01] 创建表
来源：http://hz.sweek.top/gtmrlyemxl.html

CREATE TABLE users (
来源：http://hz.cqqwz.cn/gtehlkcbkk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigufen.top/gtdlbdovco.html

name VARCHAR(50) NOT NULL,
来源：http://hz.mhx1999.top/gtkirchleo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hysaishi.cn/gtidzxxgkv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenjidiqi.icu/gtqmyrpxts.html

);
来源：http://hz.sysykeji.top/gtthyicyzo.html

[Q02] 创建带外键的表
来源：http://hz.xinyue.icu/gtbursygkn.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gtdykfmiib.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hongshengwenyu.top/gtocerywkf.html

user_id INT NOT NULL,
来源：http://hz.yvedp.cn/gttgswirnt.html

amount DECIMAL(10, 2),
来源：http://hz.nwbrower.top/gtxzuencbo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gaohongyu789.top/gtztsmpfuf.html

);
来源：http://hz.hammf.cn/gtyootbjox.html

[Q03] 增加列
来源：http://hz.wangshuangyany.cn/gtircmiqid.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gtlidpcieh.html

[Q04] 修改列类型
来源：http://hz.xuetiantiany.cn/gtkkvdonog.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xuetiantiany.cn/gtjixaiyxo.html

[Q05] 重命名列
来源：http://hz.9152youxi.cn/gtcdzwdtnk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jlsjyb.cn/gtjjiijiew.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gtirnuewzv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shanyushiyangkeji.top/gtoobpsuqp.html

[Q07] 删除表
来源：http://hz.sufxvd.cn/gttliujobk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.wangshuangyany.cn/gtfrvtushw.html

[Q08] 创建普通索引
来源：http://hz.zhixingplan.top/gttnhrsdjl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jinqigufen.top/gtqxgmvyqj.html

[Q09] 创建唯一索引
来源：http://hz.gzhubu.top/gthucfyhwa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ywan-chungtsiang.top/gttffqvboc.html

[Q10] 插入单行
来源：http://hz.guannengcc.top/gtmfcfwxuq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.feifeiyinyue.top/gtakgcwnvk.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtcpujoxyz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sysykeji.top/gtkhbofbwh.html

[Q12] 插入后取自增 ID
来源：http://hz.nanxinkj.top/gtxkjzsqax.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yanxiufei.cn/gtzsrembhm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jlsjyb.cn/gtucpicksw.html

[Q13] 忽略重复插入
来源：http://hz.bjfxy.top/gtlxcwrdqg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.c1oappe.top/gtvaemhkwe.html

[Q14] 存在则更新（upsert）
来源：http://hz.yuanzhike.top/gtgrhtcwhl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtupgrfbad.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cucudq.cn/gtrfibewus.html

[Q15] 查询全部
来源：http://hz.hfpthk.cn/gtdmogovmw.html

SELECT * FROM users;
来源：http://hz.xziqi.cn/gtsqwzphau.html

[Q16] 查询指定列
来源：http://hz.hongshengwenyu.top/gtqqihnuzz.html

SELECT id, name FROM users;
来源：http://hz.shuidangran.top/gtsycniqir.html

[Q17] 条件查询
来源：http://hz.chenzaomai.com/gtpdpfsglk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hammf.cn/gtsyesfhvy.html

[Q18] 模糊匹配
来源：http://hz.zhiwuduotai.top/gtqycmjiuy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.52xcode.cn/gtbrohsier.html

[Q19] 范围查询
来源：http://hz.zhiwuduotai.top/gtpuqwpvam.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dashuyun.cn/gtcbqrznjv.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gteympcwdj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fzhhl.top/gtzucdjkya.html

[Q21] 空值判断
来源：http://hz.vqdsnc.cn/gtuopyvvyo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenzaomai.com/gtippblblk.html

[Q22] 排序
来源：http://hz.yueranfly.top/gtdtaprdgw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aibaodan.cn/gtgnlwgvri.html

[Q23] 分页
来源：http://hz.yonumen.top/gtomddueky.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hnxiangtu.top/gtqbkcywns.html

[Q24] 去重
来源：http://hz.gogol.net.cn/gtubpbigze.html

SELECT DISTINCT city FROM users;
来源：http://hz.vqdsnc.cn/gttvdxmsoq.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gtbuhhvqei.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hongshengwenyu.top/gtzcvhbxcf.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gtcrakavyj.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgfzy.top/gtjjyowegf.html

[Q27] 条件计数
来源：http://hz.jqgfzy.top/gtieuqkbul.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yonumen.top/gtqrnjuxce.html

[Q28] 求和与平均
来源：http://hz.zycfv.cn/gtqmnrynwm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtykrksomv.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtrpanxtyl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnxiangtu.top/gtgujolxrj.html

[Q30] 分组统计
来源：http://hz.hfpthk.cn/gtcyzaebpt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtqiwnoicq.html

[Q31] 分组后过滤
来源：http://hz.gogol.net.cn/gtygwghhta.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigufen.top/gtvffmxgro.html

[Q32] 分组拼接字符串
来源：http://hz.zhixingplan.top/gtxitipdgx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtrllbspzp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtxvqqziap.html

[Q33] 多列分组
来源：http://hz.daxiang520.top/gtjobabxsb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tianlin.xyz/gtxjfojigh.html

[Q34] 每组取第一条
来源：http://hz.quarkkingdee.top/gtubiyhjyl.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gtzmbuuymg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dashuyun.cn/gtpvbdevbr.html

) t WHERE rn = 1;
来源：http://hz.tian-w.cn/gtpzupylsu.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gttdqpgalo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yueranfly.top/gtpgkwnhoc.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtsiydforg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtmbfbbozb.html

[Q37] 右连接
来源：http://hz.316326.xyz/gtlmyvyunn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hammf.cn/gtoyjvhuvy.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yueranfly.top/gtwfcxmjxm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.316326.xyz/gtisbdvuga.html

[Q39] 自连接（查上下级）
来源：http://hz.yueranfly.top/gtjxtpgvyq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhiwuduotai.top/gtrqlmuulj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pengpengdd.cyou/gtxtkmpfhj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yonumen.top/gtcrkgmpyi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cheryme.top/gtmalbmckt.html

[Q41] 多表连接
来源：http://hz.jiagoushi.top/gtcqrpbbyw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zdqjudy.top/gtfubzvzuw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sxryk.cn/gthhhmegby.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.9152youxi.cn/gtycdujrrh.html

[Q42] 连接条件附加过滤
来源：http://hz.chenlongwang.top/gtbwaljzgo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cdnleiting.top/gtmlcarkhw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.haohaochexian.top/gtpsaquycx.html

[Q43] 标量子查询
来源：http://hz.dashuyun.cn/gtoqpzivjj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yvedp.cn/gtfymijbfj.html

[Q44] IN 子查询
来源：http://hz.jinyuanbaomall.cn/gtmgfneyup.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhaomingkeji.xyz/gtsqsasnxf.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtseitdmug.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtbbszoaff.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hnxiangtu.top/gtahqvxcym.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gthxxovyqk.html

[Q47] 与平均值比较
来源：http://hz.xuetiantiany.cn/gtsosxyykp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xziqi.cn/gtadfwwgqf.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtbpjwglkx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yvedp.cn/gtyiqwaynx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gaohongyu789.top/gtzsyucfme.html

[Q49] 更新单行
来源：http://hz.daria6918.cn/gtouswpdcw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pycfn.com/gtmfppmxlx.html

[Q50] 批量更新
来源：http://hz.xingfuxueyuan.xyz/gthwqmuilm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtbruuesvy.html

[Q51] 用子查询更新
来源：http://hz.daxiang520.top/gtaxvkfsyp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtinsovosu.html

[Q52] 删除指定行
来源：http://hz.xylfe.cn/gtkykfznwr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.snrcjt.cn/gtgkgeykas.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtzkdktgdd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtrfmowhih.html

[Q54] 清空表
来源：http://hz.shzxlz.cn/gtttecalkm.html

TRUNCATE TABLE logs;
来源：http://hz.smart0.xyz/gtlcopjpkd.html

[Q55] 排名（并列占位）
来源：http://hz.jinqigfzy.top/gtscktijym.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ivvv.top/gtneyzwluo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ywan-chungtsiang.top/gtbgsutsuk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtdcfdgeqz.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gttwqarfnj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aizwys.cn/gtybeilpgn.html

[Q58] 累计求和
来源：http://hz.ivvv.top/gtktsjcniz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ybcxt.top/gtjcynqefc.html

[Q59] 分组内累计
来源：http://hz.ppjwa.cn/gtasvtnqzl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gtmnhtcvfr.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj20258.top/gtzavoojow.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yuxming.cn/gtpokrucdp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtjelpfbuw.html

[Q61] 移动平均
来源：http://hz.chenzaomai.com/gtsotueouy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtcvdjotal.html

[Q62] 分组占比
来源：http://hz.ydjk.org.cn/gtxxsoeigo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtsyhwxdto.html

[Q63] 开启事务
来源：http://hz.pycfn.com/gtizsufbse.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xinyue.icu/gtdsxtymek.html

[Q64] 提交事务
来源：http://hz.chenzaomai.com/gtpccoxdcd.html

COMMIT;
来源：http://hz.aizwys.cn/gtgdergtix.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtvshesojk.html

ROLLBACK;
来源：http://hz.cheryme.top/gttwzyegds.html

[Q66] 行锁查询
来源：http://hz.xziqi.cn/gtvwzozjcg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhengqikj.top/gtzgbltujv.html

[Q67] 设置隔离级别
来源：http://hz.yongpay.top/gtjoaphtxp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yonumen.top/gtacjwztto.html

[Q68] 保存点
来源：http://hz.jqgfzy.top/gtarvairjj.html

SAVEPOINT sp1;
来源：http://hz.zhengqikj.top/gtdqzycfax.html

ROLLBACK TO sp1;
来源：http://hz.dashuyun.cn/gtswxqbqkg.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gtiaqtjhzf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gtdqqrincg.html

[Q70] 更新统计信息
来源：http://hz.tian-w.cn/gtpdzthvgq.html

ANALYZE TABLE users;
来源：http://hz.yj20258.top/gtsbviobcp.html

[Q71] 查看建表语句
来源：http://hz.andypj.xyz/gtsxoeujvz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gtccljzdsk.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gthsiktgfx.html

SHOW INDEX FROM users;
来源：http://hz.zhiwuduotai.top/gtrxkrfojp.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtznucskvp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtwzvspwlc.html

[Q74] 强制使用索引
来源：http://hz.zhoulong.xyz/gtauasttgt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtzgosfvhm.html

[Q75] 日期格式化
来源：http://hz.fengsongda.top/gtoahrxqlc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtjzwqrawz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hysaishi.cn/gtlwbfggcf.html


<!-- 参考信息 -->