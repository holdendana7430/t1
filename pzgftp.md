代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtxctakwcq.html

Go:   go f()
来源：http://hz.tanke756.top/gttgqwjdst.html

Ruby: Thread.new { f }
来源：http://hz.jianghu66.top/gtwgwbhaff.html

C#:   Task.Run(() => F());
来源：http://hz.ydjk.org.cn/gtbejptool.html

[O02] 使用线程池
来源：http://hz.xinyue.icu/gtkpuziwse.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuxming.cn/gtgokkohno.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtenkvixig.html

JS:   // worker_threads 线程池
来源：http://hz.ywan-chungtsiang.top/gtpgvxxzzm.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtuckmppxn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtaekafxzi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gtivynaazl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.feifeiyinyue.top/gtmwxjqxep.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtzytuimtx.html

[O03] 加锁保护共享数据
来源：http://hz.chenlongwang.top/gtgnslgico.html

Py:   with lock: shared += 1
来源：http://hz.mhx1999.top/gthmdrpqpl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.bjfxy.top/gtyulwavve.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ydzc1.top/gtmcishjwx.html

TS:   // 同 JS
来源：http://hz.ehwqpu.com/gtgwdqizbn.html

Java: synchronized (this) { shared++; }
来源：http://hz.hywenlv.cn/gtltqotqam.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cdnleiting.top/gtfocvysgl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtikffmunn.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gttlciysbf.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258888.top/gtlqiarlla.html

Py:   async def f():⏎    await g()
来源：http://hz.xuetiantiany.cn/gtpsoltypz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xuetiantiany.cn/gtofmktkiy.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtmpxxouir.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gtpakiiugr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.redwolf501.top/gtqutxtkno.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnxiangtu.top/gtelaekvvb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.andypj.xyz/gtijgzdruu.html

C#:   async Task F() { await G(); }
来源：http://hz.kuanghao11.cn/gtybycvhde.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gteypgyebd.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtpmfwygcv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shangyingyoupin.top/gtxgapulxd.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtnknasojf.html

TS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtaknqfgpo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ivvv.top/gtlijkmedz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtsgenkqwx.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangkeji.top/gtsvhurzpq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gtxoxupdzu.html

[O06] 使用进程池
来源：http://hz.quarkkingdee.top/gtisanjxoo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gthhgalupi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.havefunace.top/gtgddfjlnn.html

JS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtevizslrf.html

TS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtnbwocqyh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jlsjyb.cn/gtgjiopocy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hnqzz.top/gttctylejo.html

Ruby: // fork 块
来源：http://hz.xuetiantiany.cn/gtcyhbxkwj.html

C#:   Parallel.For
来源：http://hz.zhijiandao.cn/gtrehpteoo.html

================================================================================
来源：http://hz.fzhhl.top/gtexjbquxa.html

P. 常用工具函数
来源：http://hz.yvedp.cn/gtgbypoyou.html

================================================================================
来源：http://hz.redwolf501.top/gtcienetgv.html

[P01] 生成 UUID
来源：http://hz.ydjk.org.cn/gtnumkariu.html

Py:   str(uuid.uuid4())
来源：http://hz.jinghuilouyu.cn/gtpwjkgafb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cheryme.top/gtfvasvbdz.html

JS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtvzprhoyt.html

TS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtwxhxrpfs.html

Java: UUID.randomUUID().toString()
来源：http://hz.wangshuangyany.cn/gtkrcimpfl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gttqipcjil.html

Ruby: SecureRandom.uuid
来源：http://hz.jinghuilouyu.cn/gtmtnpkgja.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhijiandao.cn/gtwngqceep.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuanzhike.top/gtmfvokzix.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.smart0.xyz/gtpfylwahu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yanxiufei.cn/gtomdxontj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xinyue.icu/gtrpnypegm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.mhx1999.top/gtqhaeceli.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigufen.top/gtxndutzzp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gtegixuwox.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.dashuyun.cn/gtacywepjl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258.top/gtrozmnndq.html

[P03] 生成短随机字符串
来源：http://hz.cqqwz.cn/gtfcshshew.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtktgxuvsr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinyuanbaomall.cn/gtotbtqfyx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gtkasiluad.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtcpgbkpes.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.cashguo.top/gtuyophbsf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtweemzlpw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.tian-w.cn/gtwykheoos.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xuetiantiany.cn/gtgibqigkq.html

[P04] 求长度
来源：http://hz.cashguo.top/gteadbydcc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenlongwang.top/gtrehzdciq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gthibpydfa.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtbqqnpuxd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangshuangyany.cn/gtgvbdqczb.html

Java: list.size();  map.size();  s.length()
来源：http://hz.andypj.xyz/gtyetuyabo.html

Go:   len(arr);  len(m)
来源：http://hz.ybcxt.top/gtyyhtsaxm.html

Ruby: x.length;  x.size
来源：http://hz.fengsongda.top/gtgfxihzna.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxinkj.top/gtibicneyk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhengqikj.top/gtzcnkcydt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fengsongda.top/gtgeamqyaz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guannengcc.top/gtsqsyggsv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhengqikj.top/gtsukacxzy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gthewndgpt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tian-w.cn/gtkcydwfgj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cheryme.top/gtiwlevjme.html

Ruby: a == b
来源：http://hz.vqdsnc.cn/gtbgtxmadh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.redwolf501.top/gtwsxedcay.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.kuanghao11.cn/gthomoibje.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtmdjpizsy.html

PHP:  if (empty($x)) {}
来源：http://hz.ydzc1.top/gtzxhbktzv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zdqjudy.top/gtvcakxvem.html

TS:   if (x == null) {}
来源：http://hz.yangfankeji.com/gtnrlmtngm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.andypj.xyz/gtjmrgteag.html

Go:   if x == nil {}
来源：http://hz.sweek.top/gtqeheqwje.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gthycwiuun.html

C#:   if (x is null) {}
来源：http://hz.wangdashe.top/gtqpyuyvsj.html

[P07] 防抖与节流
来源：http://hz.tian-w.cn/gtuxaalyaa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.mhx1999.top/gtjepokngw.html

PHP:  // 手写时间戳比较
来源：http://hz.zhongyouzk.top/gtgvfpboel.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yueranfly.top/gtizfpqocx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtuwcnmdzk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangdashe.top/gtcpudlguq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ehwqpu.com/gtkwmljqwu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zycfv.cn/gtmgwcdnhd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ydjk.org.cn/gtxhxqetze.html

[P08] 处理浮点精度问题
来源：http://hz.meibo888.top/gtgzhkhxdu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.quarkkingdee.top/gtarllylaj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258.top/gtnhcbrdhj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.daxiang520.top/gtbcgyflse.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.dianchejie.cn/gtzketnuyb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.guowangkeji.top/gtjpnmdzou.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hongshengwenyu.top/gtkojyxjzo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ehwqpu.com/gtubpywbce.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.wangdashe.top/gtmisdnzjb.html

================================================================================
来源：http://hz.gogol.net.cn/gtulqpikwr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258888.top/gttwbbnvgy.html

================================================================================
来源：http://hz.svipenyu.cn/gtnbukunpx.html

[Q01] 创建表
来源：http://hz.jqgfzy.top/gtccdkswqg.html

CREATE TABLE users (
来源：http://hz.sxryk.cn/gthrpqnhuo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xziqi.cn/gtqwbhsqnr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.tianlin.xyz/gtkexlgjir.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dashuyun.cn/gteuumntyu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cdnleiting.top/gtaqjxcasm.html

);
来源：http://hz.hammf.cn/gtnwfzyovy.html

[Q02] 创建带外键的表
来源：http://hz.wangdashe.top/gtjwcrkujm.html

CREATE TABLE orders (
来源：http://hz.cqqwz.cn/gtiasjpwfx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guannengcc.top/gthhlnggli.html

user_id INT NOT NULL,
来源：http://hz.yuxming.cn/gtnsmuuezw.html

amount DECIMAL(10, 2),
来源：http://hz.yvedp.cn/gtnsqdrwlj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xziqi.cn/gtsevhrofu.html

);
来源：http://hz.shuidangran.top/gtadikwujp.html

[Q03] 增加列
来源：http://hz.bjfxy.top/gtfjntdpvl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yuanzhike.top/gtltouaknh.html

[Q04] 修改列类型
来源：http://hz.9152youxi.cn/gtycounmbs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cashguo.top/gtrvzdtoum.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gttyfjniwk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.feifeiyinyue.top/gtcgxgwfua.html

[Q06] 删除列
来源：http://hz.ybcxt.top/gtnexhakoh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigfzy.top/gtwfilypkw.html

[Q07] 删除表
来源：http://hz.mhx1999.top/gteucdrqdo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtflbpernj.html

[Q08] 创建普通索引
来源：http://hz.ehwqpu.com/gtqvedymxa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gttshwggaq.html

[Q09] 创建唯一索引
来源：http://hz.shuidangran.top/gtwczgghsn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.andypj.xyz/gtwkygubsv.html

[Q10] 插入单行
来源：http://hz.zhijiandao.cn/gtbcsiairg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tianlin.xyz/gtimuiugsl.html

[Q11] 一次插入多行
来源：http://hz.zhijiandao.cn/gtuwprztno.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gaohongyu789.top/gtmfwlwkvw.html

[Q12] 插入后取自增 ID
来源：http://hz.guannengcc.top/gtjmnokasi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.meibo888.top/gtosfjojgh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gttkezjfls.html

[Q13] 忽略重复插入
来源：http://hz.hywenlv.cn/gtxbzjetzk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.52xcode.cn/gtvvjhxrly.html

[Q14] 存在则更新（upsert）
来源：http://hz.cqqwz.cn/gttmnwjubg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj20258.top/gtgywevnqw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.vqdsnc.cn/gtntbkaoch.html

[Q15] 查询全部
来源：http://hz.nwbrower.top/gtytntzkta.html

SELECT * FROM users;
来源：http://hz.pycfn.com/gtsppshrzt.html

[Q16] 查询指定列
来源：http://hz.xuanzx.com/gtlncnmmem.html

SELECT id, name FROM users;
来源：http://hz.iojbl.cn/gtsgmfbxwy.html

[Q17] 条件查询
来源：http://hz.zycfv.cn/gtjuwtyzdm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ehwqpu.com/gtkttnjdlf.html

[Q18] 模糊匹配
来源：http://hz.shanyushiyangkeji.top/gtoenwijil.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhoulong.xyz/gtkqjmdnhl.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtnfkbzwhh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hammf.cn/gtngczxqkh.html

[Q20] IN 列表
来源：http://hz.cashguo.top/gtlpykkcua.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtnkaxceva.html

[Q21] 空值判断
来源：http://hz.nwbrower.top/gtncynafbt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhijiandao.cn/gtlghiinih.html

[Q22] 排序
来源：http://hz.hnqzz.top/gtlhyuspel.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xuetiantiany.cn/gtyzmjnldt.html

[Q23] 分页
来源：http://hz.ppjwa.cn/gtihufmhha.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.meibo888.top/gtnlijdaea.html

[Q24] 去重
来源：http://hz.wangdashe.top/gtohqysnbc.html

SELECT DISTINCT city FROM users;
来源：http://hz.quarkkingdee.top/gtsvkthfsy.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtipyxwpmb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cdnleiting.top/gtakgpquow.html

[Q26] 计数
来源：http://hz.yuxming.cn/gtwuwtiybn.html

SELECT COUNT(*) FROM users;
来源：http://hz.havefunace.top/gtyuexntgo.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtkidtqupt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangdashe.top/gtkxhqjhgn.html

[Q28] 求和与平均
来源：http://hz.zycfv.cn/gtcsnsfiig.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtvdbibijn.html

[Q29] 最大最小值
来源：http://hz.sufxvd.cn/gtuixbxvqm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtyoqrtvjz.html

[Q30] 分组统计
来源：http://hz.ybcxt.top/gtlkwaamit.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtiwbbdskh.html

[Q31] 分组后过滤
来源：http://hz.cucudq.cn/gtttfmihyz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yj202588.top/gtkdkqtoyn.html

[Q32] 分组拼接字符串
来源：http://hz.shzxlz.cn/gtleqxwpke.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtrczofadk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuetiantiany.cn/gthqbylhqu.html

[Q33] 多列分组
来源：http://hz.sxryk.cn/gtlnxzlwdo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.aibaodan.cn/gtxfvxsvgf.html

[Q34] 每组取第一条
来源：http://hz.sweek.top/gtodvobpnb.html

SELECT * FROM (
来源：http://hz.zhoulong.xyz/gtzebtevnj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hnqzz.top/gtbhyntfhi.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtmrtmgzcy.html

[Q35] 内连接
来源：http://hz.xinyue.icu/gtwusfcqks.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ehwqpu.com/gtlsuwsvpe.html

[Q36] 左连接
来源：http://hz.zdqjudy.top/gtkekokgww.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtifjeionu.html

[Q37] 右连接
来源：http://hz.kuanghao11.cn/gtpqhszzrb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yangfankeji.com/gtzvekyqhh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhengqikj.top/gtanvdtwju.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtilmbtjyd.html

[Q39] 自连接（查上下级）
来源：http://hz.redwolf501.top/gturnfbqlh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.feifeiyinyue.top/gtocyhuujc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nanxinkj.top/gtydfryycw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gtmdlhmivb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daria6918.cn/gtgjmptbwk.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtelqzjmjh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtadawvpzh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.svipenyu.cn/gtlnflucpy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.feifeiyinyue.top/gtnvnlbbng.html

[Q42] 连接条件附加过滤
来源：http://hz.0kj1m.cn/gtlysgkyhq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gtufndxtky.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gthlptznlx.html

[Q43] 标量子查询
来源：http://hz.hongshengwenyu.top/gtyiyonske.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinqigufen.top/gtqkuetuzi.html

[Q44] IN 子查询
来源：http://hz.tanke756.top/gtnbsmtjkv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hysaishi.cn/gtbjoveovy.html

[Q45] EXISTS 判断存在
来源：http://hz.zhoulong.xyz/gtlqmlechk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtqaimjebs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jlsjyb.cn/gtbvwhvjab.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtoidbifea.html

[Q47] 与平均值比较
来源：http://hz.yanxiufei.cn/gtztohrcnl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.svipenyu.cn/gtnjgmxpyh.html

[Q48] CTE 公用表表达式
来源：http://hz.snrcjt.cn/gtxmdmbhpr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.redwolf501.top/gtopwwjuri.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.c1oappe.top/gtqpkzuowo.html

[Q49] 更新单行
来源：http://hz.cqqwz.cn/gtiafmhgnr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtozrobelh.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtsyaiuoii.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xylfe.cn/gttthoafzi.html

[Q51] 用子查询更新
来源：http://hz.cqqwz.cn/gtubiszzte.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtetssvpwo.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtfgzperzn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ehwqpu.com/gtksvjyhpx.html

[Q53] 按条件删除
来源：http://hz.jianghu66.top/gtxkscozmq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtolzegowx.html

[Q54] 清空表
来源：http://hz.zhiwuduotai.top/gtloyvivcz.html

TRUNCATE TABLE logs;
来源：http://hz.chenzaomai.com/gtevioqovs.html

[Q55] 排名（并列占位）
来源：http://hz.cdnleiting.top/gtftapulcu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtzeuzfbyf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtyohsvijf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtzgbrccgo.html

[Q57] 行号
来源：http://hz.gzhubu.top/gtvpnvaabl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxinkj.top/gtshfhoosm.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtwpqvgdsd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hammf.cn/gtpatvlecv.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtnuogaens.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gteosifyjy.html

[Q60] 取上一行 / 下一行
来源：http://hz.quarkkingdee.top/gtbbsonjzq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nwbrower.top/gtzhnbraxv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guannengcc.top/gttlcbdpcn.html

[Q61] 移动平均
来源：http://hz.yj202588.top/gtlimzzhxp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangshuangyany.cn/gtjhtbmdzn.html

[Q62] 分组占比
来源：http://hz.nanxuanxn.top/gtjctoojgh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtkxqreuzf.html

[Q63] 开启事务
来源：http://hz.sysykeji.top/gtvrkorugq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.snrcjt.cn/gtlquinndp.html

[Q64] 提交事务
来源：http://hz.shangyingyoupin.top/gtsksdktas.html

COMMIT;
来源：http://hz.smart0.xyz/gtgpqjywvv.html

[Q65] 回滚事务
来源：http://hz.fengsongda.top/gtsguhbpxz.html

ROLLBACK;
来源：http://hz.gogol.net.cn/gtmmtmmneg.html

[Q66] 行锁查询
来源：http://hz.zhiwuduotai.top/gthcafhebk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gtlyamadou.html

[Q67] 设置隔离级别
来源：http://hz.pycfn.com/gtbhqcourd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yongpay.top/gtbujcrbxm.html

[Q68] 保存点
来源：http://hz.hywenlv.cn/gtinvlneon.html

SAVEPOINT sp1;
来源：http://hz.shuidangran.top/gtepznffie.html

ROLLBACK TO sp1;
来源：http://hz.wangdashe.top/gtmyvzedge.html

[Q69] 查看执行计划
来源：http://hz.fengsongda.top/gtjqsbxqdb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258888.top/gtzeqzwrqk.html

[Q70] 更新统计信息
来源：http://hz.jqgufenzy.top/gtmjfuyodr.html

ANALYZE TABLE users;
来源：http://hz.jiagoushi.top/gtstrddvau.html

[Q71] 查看建表语句
来源：http://hz.52xcode.cn/gttqhkczgo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.mhx1999.top/gtqdqnhfjv.html

[Q72] 查看索引
来源：http://hz.sufxvd.cn/gtlfevcyac.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtvcajhvuu.html

[Q73] 查看表状态
来源：http://hz.zhoulong.xyz/gtpxupqhep.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pengpengdd.cyou/gthwmzlzsc.html

[Q74] 强制使用索引
来源：http://hz.dianchejie.cn/gtoultechy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuxming.cn/gttpsmmfha.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtlgsngzmh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtqhcsptnq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtdjytghvf.html


<!-- 参考信息 -->