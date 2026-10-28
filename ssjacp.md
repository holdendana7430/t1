代发 wailian999

TS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtqupczowj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtnfxbhcns.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ydzc1.top/gtvtoxibmz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinqigfzy.top/gtpptusvjw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xinyue.icu/gtlsrokwqr.html

[O03] 加锁保护共享数据
来源：http://hz.zhoulong.xyz/gtaeheoqsw.html

Py:   with lock: shared += 1
来源：http://hz.tianlin.xyz/gtryltmbof.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxuanxn.top/gtcvxxsblk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jyoumei.cn/gtyumisurv.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtqtslwxwn.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtwzfjgqsx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhoulong.xyz/gtvnofdfvz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sxryk.cn/gtzrgwoyfv.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxuanxn.top/gtouxyetut.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gtofmgbvij.html

Py:   async def f():⏎    await g()
来源：http://hz.cheryme.top/gtdqaklxnq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hnqzz.top/gtihoueign.html

JS:   async function f() { await g(); }
来源：http://hz.shanyushiyangtech.top/gtpavgfyru.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.bjfxy.top/gtkmnvavad.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuanzx.com/gtfnyuazmh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xuetiantiany.cn/gtmikfryis.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gtwxgykybt.html

C#:   async Task F() { await G(); }
来源：http://hz.tanke756.top/gtyyfgakts.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gtymxxcquz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhengqikj.top/gtxzkuojon.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtyftngxnh.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtkwqinddv.html

TS:   await Promise.all(tasks)
来源：http://hz.hnxiangtu.top/gtinoqrnuq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sufxvd.cn/gtrictkiie.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenjidiqi.icu/gtijqdmzfj.html

Ruby: threads.map(&:join)
来源：http://hz.hfpthk.cn/gtwlatqyam.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hongshengwenyu.top/gtivqykfdr.html

[O06] 使用进程池
来源：http://hz.yongpay.top/gtxyhkrmfj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hywenlv.cn/gtakktzcpa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gzhubu.top/gtyvfsrbcf.html

JS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtwbhwdlwv.html

TS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtknzxbdxr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dianchejie.cn/gtdidrzslv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigfzy.top/gtkogesbpw.html

Ruby: // fork 块
来源：http://hz.hnqzz.top/gtqnjyerxp.html

C#:   Parallel.For
来源：http://hz.zycfv.cn/gtigwsdktp.html

================================================================================
来源：http://hz.316326.xyz/gtktuthyqq.html

P. 常用工具函数
来源：http://hz.ywan-chungtsiang.top/gtwroblnlx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtpgtuiqyg.html

[P01] 生成 UUID
来源：http://hz.ydzc1.top/gthcjyxrmt.html

Py:   str(uuid.uuid4())
来源：http://hz.ehwqpu.com/gtzfcfdkmm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fengsongda.top/gtnqxuudxw.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtuzgvkcyu.html

TS:   crypto.randomUUID()
来源：http://hz.ehwqpu.com/gtmfhtsmry.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhongyouzk.top/gtotkvuvnc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.chenlongwang.top/gtycnxhvra.html

Ruby: SecureRandom.uuid
来源：http://hz.ydjk.org.cn/gtcuhoqzmt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhengqikj.top/gtgtjfnnxt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nwbrower.top/gtikknxohb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.meibo888.top/gtunljfjhi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shzxlz.cn/gtibedyxwf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nwbrower.top/gtdjnuovnl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.meibo888.top/gtunvvrcdn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guowangkeji.top/gtqaeuafbr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shuidangran.top/gtkmyivtwn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuxming.cn/gtlgrleswz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pengpengdd.cyou/gtrplscbtj.html

[P03] 生成短随机字符串
来源：http://hz.yangfankeji.com/gterzbgjgg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtszpftbnc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangshuangyany.cn/gtydezdmfu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ywan-chungtsiang.top/gtpzsassqx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gttydwucpp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.316326.xyz/gtectpnjxg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxinkj.top/gtvjaowcjg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgfzy.top/gtghkrlgiw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.wangshuangyany.cn/gteejkbgec.html

[P04] 求长度
来源：http://hz.kuanghao11.cn/gtqspyuohd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.52xcode.cn/gtofyljeos.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtmqoaagzl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gaohongyu789.top/gtevdjkzdm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ivvv.top/gtsbsrxbqk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hnxiangtu.top/gtmnbsafph.html

Go:   len(arr);  len(m)
来源：http://hz.jqgufenzy.top/gthlouqoer.html

Ruby: x.length;  x.size
来源：http://hz.9152youxi.cn/gtfwxauhki.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ydjk.org.cn/gtaoxuphif.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuetiantiany.cn/gtkaymvukk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.haohaochexian.top/gtiuhecyod.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangdashe.top/gtlyvhimvv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.xuanzx.com/gtnikdibca.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtkbnrqhah.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shuidangran.top/gtiixngwzz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.smart0.xyz/gtpsuilmlh.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtlbhuctrt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ehwqpu.com/gthekpnbvh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.vqdsnc.cn/gtgkhuvusd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.xuetiantiany.cn/gtwyndpfvq.html

PHP:  if (empty($x)) {}
来源：http://hz.chenzaomai.com/gtjpilduwn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.cqqwz.cn/gtqobimoak.html

TS:   if (x == null) {}
来源：http://hz.yongpay.top/gtqfkxqdpt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guowangkeji.top/gtvrrhqsfs.html

Go:   if x == nil {}
来源：http://hz.yvedp.cn/gtmdgmhepc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.smart0.xyz/gtuqfwwskh.html

C#:   if (x is null) {}
来源：http://hz.nanxuanxn.top/gtwdgfcdsr.html

[P07] 防抖与节流
来源：http://hz.sweek.top/gtkzaziiwo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.birdmap.top/gtdfkirlmy.html

PHP:  // 手写时间戳比较
来源：http://hz.hywenlv.cn/gtdqsuocda.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtcuzylzay.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtbliygocx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pengpengdd.cyou/gtymhbhmhi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.mhx1999.top/gtikynhybt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gzhubu.top/gtlbdnjwry.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gturohbgsd.html

[P08] 处理浮点精度问题
来源：http://hz.yvedp.cn/gtyglfpvtv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shzxlz.cn/gtamlkxprd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gzhubu.top/gtiffnxztw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guannengcc.top/gttchvhcdt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hysaishi.cn/gtbqthkzpa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.iojbl.cn/gtegekslei.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.shzxlz.cn/gtshvzlkmj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hongshengwenyu.top/gtakikakmf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sysykeji.top/gtwyvkydlb.html

================================================================================
来源：http://hz.daria6918.cn/gtdxqjytwu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.pycfn.com/gtdjeiebyo.html

================================================================================
来源：http://hz.iojbl.cn/gtbxlbnyjd.html

[Q01] 创建表
来源：http://hz.jinqigfzy.top/gtucmkyqew.html

CREATE TABLE users (
来源：http://hz.zhiwuduotai.top/gtxpfppiav.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gttxqtkdwj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenjidiqi.icu/gtiypcvreu.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cdnleiting.top/gtzhjigorj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.andypj.xyz/gtwueaawgk.html

);
来源：http://hz.wangdashe.top/gtfxnqbtcv.html

[Q02] 创建带外键的表
来源：http://hz.guowangkeji.top/gthtucpxjp.html

CREATE TABLE orders (
来源：http://hz.chenlongwang.top/gtayutmjlb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtjucaceze.html

user_id INT NOT NULL,
来源：http://hz.ivvv.top/gtekpucmqu.html

amount DECIMAL(10, 2),
来源：http://hz.daria6918.cn/gtijrsxxtu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dashuyun.cn/gtirkoztqn.html

);
来源：http://hz.fzhhl.top/gttjzqotnr.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gtpcfyqffl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gtoxvviyyy.html

[Q04] 修改列类型
来源：http://hz.zhengqikj.top/gtjqspywrq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cashguo.top/gtlfuibxgq.html

[Q05] 重命名列
来源：http://hz.shanyushiyangkeji.top/gthhqzizfi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zdqjudy.top/gtqgmjqkqf.html

[Q06] 删除列
来源：http://hz.kuanghao11.cn/gtlwadwekh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gtxzbnojrj.html

[Q07] 删除表
来源：http://hz.andypj.xyz/gtnurszswx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aibaodan.cn/gtjuxvpide.html

[Q08] 创建普通索引
来源：http://hz.jinqigufen.top/gtbyrigpwm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jqgfzy.top/gtngbnwswz.html

[Q09] 创建唯一索引
来源：http://hz.jyoumei.cn/gtdiinyhmx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gzhubu.top/gtjqvtityf.html

[Q10] 插入单行
来源：http://hz.9152youxi.cn/gtuprzhpmt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhiwuduotai.top/gtkifdanor.html

[Q11] 一次插入多行
来源：http://hz.cdnleiting.top/gtvppxcilh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yueranfly.top/gtdnukwylj.html

[Q12] 插入后取自增 ID
来源：http://hz.jinghuilouyu.cn/gtcqptasiy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.c1oappe.top/gtopwthcjh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhiwuduotai.top/gtlykyjbmb.html

[Q13] 忽略重复插入
来源：http://hz.shanyushiyangkeji.top/gtsiqijvrw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yueranfly.top/gtecqceslx.html

[Q14] 存在则更新（upsert）
来源：http://hz.cashguo.top/gtxblqyxsz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fengsongda.top/gtgldvgzio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.316326.xyz/gtzeqtsxmo.html

[Q15] 查询全部
来源：http://hz.havefunace.top/gtskjxbhwe.html

SELECT * FROM users;
来源：http://hz.cqqwz.cn/gtztkbpfng.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtozvduxpw.html

SELECT id, name FROM users;
来源：http://hz.andypj.xyz/gtollpjemg.html

[Q17] 条件查询
来源：http://hz.aibaodan.cn/gtukrraaob.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ydjk.org.cn/gthwfthgxy.html

[Q18] 模糊匹配
来源：http://hz.quarkkingdee.top/gtaumyawgp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangtech.top/gtmxvnzzkx.html

[Q19] 范围查询
来源：http://hz.shangyingyoupin.top/gtadrhlvgr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yueranfly.top/gtnnthmfqp.html

[Q20] IN 列表
来源：http://hz.zdqjudy.top/gtgzlqibsc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenzaomai.com/gtupwhahrv.html

[Q21] 空值判断
来源：http://hz.daxiang520.top/gtcckjuxkc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tianlin.xyz/gtqtofijjs.html

[Q22] 排序
来源：http://hz.ehwqpu.com/gtijbckwbp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fengsongda.top/gtsmckgfiy.html

[Q23] 分页
来源：http://hz.hammf.cn/gtnjpmwryo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guowangkeji.top/gtpnwhgvlf.html

[Q24] 去重
来源：http://hz.zdqjudy.top/gtczjzivty.html

SELECT DISTINCT city FROM users;
来源：http://hz.sysykeji.top/gthlrwowxa.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangtech.top/gtotpmxzmn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtolzjuwur.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtxcxwwjnz.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtbrcrdlik.html

[Q27] 条件计数
来源：http://hz.jqgufenzy.top/gtmnnbflud.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gtyetvsbjd.html

[Q28] 求和与平均
来源：http://hz.haohaochexian.top/gtxdanhcuv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sxryk.cn/gtcnzqqfel.html

[Q29] 最大最小值
来源：http://hz.yj202588.top/gtcihoscfg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jyoumei.cn/gtapwzlvhm.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtwcxljjtu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtmtxhtzht.html

[Q31] 分组后过滤
来源：http://hz.zhengqikj.top/gtkhzahfjm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cqqwz.cn/gtjghdwsxj.html

[Q32] 分组拼接字符串
来源：http://hz.nwbrower.top/gtawigujge.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtgflcqlre.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pengpengdd.cyou/gtxfvjzkeh.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtbxwpgkeg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.redwolf501.top/gtdxhkhymf.html

[Q34] 每组取第一条
来源：http://hz.hnqzz.top/gtdxqorxnr.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtfbqlvcpw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yueranfly.top/gtuzzzgpuy.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangtech.top/gtrlbbnvsr.html

[Q35] 内连接
来源：http://hz.xingfuxueyuan.xyz/gtzmivfkyo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yvedp.cn/gtayykhaqi.html

[Q36] 左连接
来源：http://hz.yuanzhike.top/gtkcluwtgy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtutfbtxpx.html

[Q37] 右连接
来源：http://hz.iojbl.cn/gtfhyipard.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenzaomai.com/gtofhkmbfh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xinyue.icu/gtvpvjghxy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hywenlv.cn/gteglrfpdp.html

[Q39] 自连接（查上下级）
来源：http://hz.pycfn.com/gttnbfwzpl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtvqgqitzh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yanxiufei.cn/gtbbbvawet.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cheryme.top/gtlmzehhax.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cashguo.top/gtngldgqoz.html

[Q41] 多表连接
来源：http://hz.shzxlz.cn/gtfmnqlhuq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangshuangyany.cn/gtbiegxtrm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.vqdsnc.cn/gtokzqjgfh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jianghu66.top/gtbrjgrtef.html

[Q42] 连接条件附加过滤
来源：http://hz.fzhhl.top/gtyagxqesb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yangfankeji.com/gtesoawmae.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cheryme.top/gtcysixcpf.html

[Q43] 标量子查询
来源：http://hz.smart0.xyz/gtrmcbkshz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hnqzz.top/gtyhiwimik.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gtoxxeukrr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gaohongyu789.top/gtzpbctmqz.html

[Q45] EXISTS 判断存在
来源：http://hz.bjfxy.top/gtjldowghp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnqzz.top/gtcqfhofbs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangdashe.top/gtjriewqno.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtsttlxssk.html

[Q47] 与平均值比较
来源：http://hz.0kj1m.cn/gtzokphluv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yvedp.cn/gtzkhwgmmk.html

[Q48] CTE 公用表表达式
来源：http://hz.haohaochexian.top/gtwlgxdllw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gaohongyu789.top/gtdyjesgwx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cqqwz.cn/gtlwtaexet.html

[Q49] 更新单行
来源：http://hz.jinyuanbaomall.cn/gtgjvomgwl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangtech.top/gtnuddhegg.html

[Q50] 批量更新
来源：http://hz.zhijiandao.cn/gtqlkzjnbm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gtrifttmlk.html

[Q51] 用子查询更新
来源：http://hz.ehwqpu.com/gtlukerhzw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtxqprvfjb.html

[Q52] 删除指定行
来源：http://hz.jinqigfzy.top/gteuzfwqhe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtgfsefnxq.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtjzxifsaw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigfzy.top/gthxbumbjo.html

[Q54] 清空表
来源：http://hz.cucudq.cn/gteowdoqmn.html

TRUNCATE TABLE logs;
来源：http://hz.guowangkeji.top/gtkcdspndm.html

[Q55] 排名（并列占位）
来源：http://hz.zhijiandao.cn/gtiogifreb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.andypj.xyz/gtmhuiswhz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ehwqpu.com/gtzvhimirt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenjidiqi.icu/gtnloxehrv.html

[Q57] 行号
来源：http://hz.mhx1999.top/gtfmweggxg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ppjwa.cn/gtrdcvxgdt.html

[Q58] 累计求和
来源：http://hz.hfpthk.cn/gttaanjlnq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yonumen.top/gtlhakvsfi.html

[Q59] 分组内累计
来源：http://hz.hammf.cn/gtzsujqrnf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhiwuduotai.top/gtdguoovzi.html

[Q60] 取上一行 / 下一行
来源：http://hz.nanxuanxn.top/gtzgmlwwdq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinghuilouyu.cn/gtesrbbust.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.smart0.xyz/gtmhujkalj.html

[Q61] 移动平均
来源：http://hz.shanyushiyangtech.top/gtpscibkwk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.redwolf501.top/gtnvrenomo.html

[Q62] 分组占比
来源：http://hz.zhijiandao.cn/gtiljxwvui.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtarchwguk.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtsgcqioyd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ivvv.top/gtydewpygs.html

[Q64] 提交事务
来源：http://hz.guannengcc.top/gtcqgzbryx.html

COMMIT;
来源：http://hz.hnqzz.top/gtvetsipgn.html

[Q65] 回滚事务
来源：http://hz.zdqjudy.top/gtxhlgouop.html

ROLLBACK;
来源：http://hz.sxryk.cn/gtvnwtqviw.html

[Q66] 行锁查询
来源：http://hz.kuanghao11.cn/gtrxsszagk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gtdrtnxobf.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gthsquuptk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtoeinbnqy.html

[Q68] 保存点
来源：http://hz.xziqi.cn/gthadkbsxd.html

SAVEPOINT sp1;
来源：http://hz.xuetiantiany.cn/gtglomzfbr.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gtkpvvsgfj.html

[Q69] 查看执行计划
来源：http://hz.xingfuxueyuan.xyz/gtlxnezkgt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangkeji.top/gtocagmyoi.html

[Q70] 更新统计信息
来源：http://hz.zdqjudy.top/gtqsadqlxe.html

ANALYZE TABLE users;
来源：http://hz.bjfxy.top/gtmkdjhiam.html

[Q71] 查看建表语句
来源：http://hz.yvedp.cn/gtqncwxvvh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yonumen.top/gtymusrwui.html

[Q72] 查看索引
来源：http://hz.chenzaomai.com/gtcfbieofm.html

SHOW INDEX FROM users;
来源：http://hz.zhongyouzk.top/gttjjytcen.html

[Q73] 查看表状态
来源：http://hz.zhiwuduotai.top/gtwmfzauby.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.shanyushiyangkeji.top/gtzjxsnhjg.html

[Q74] 强制使用索引
来源：http://hz.zhiwuduotai.top/gtqvkrgrqm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtfasnfdxr.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtyecfmwwa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yongpay.top/gtzrmakirt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.dianchejie.cn/gtltwpokhq.html

[Q76] 按天统计
来源：http://hz.guannengcc.top/gtshizyevx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.52xcode.cn/gtdljaxrxe.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gtldplstih.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guannengcc.top/gtrnlepotj.html

[Q78] 当前时间
来源：http://hz.gaohongyu789.top/gtqcxxidcl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sweek.top/gtfwxlxcxb.html

[Q79] 字符串拼接
来源：http://hz.ybcxt.top/gtzuzmevnb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtxnybhfvl.html


<!-- 参考信息 -->