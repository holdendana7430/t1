代发 wailian999

[O02] 使用线程池
来源：http://hz.tian-w.cn/gttgkjuxwz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dashuyun.cn/gtjopqrdtw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuanzhike.top/gteclsraqo.html

JS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtghydxwsd.html

TS:   // worker_threads 线程池
来源：http://hz.yueranfly.top/gtmdjxbvyp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guowangkeji.top/gtbgvalndq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinqigfzy.top/gtkajsvipi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ybcxt.top/gtinxamvtl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ybcxt.top/gtzoqcwpxn.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gteqcxnwpf.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangkeji.top/gtxtcmmqzy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangkeji.top/gttmpzbnqe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hywenlv.cn/gtbzerhkro.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gttfycptqu.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgufenzy.top/gttoxiutwz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gtqnrosvfd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtcyaglkpk.html

C#:   lock (gate) { shared++; }
来源：http://hz.birdmap.top/gtgqcnocpc.html

[O04] 定义异步函数并等待
来源：http://hz.havefunace.top/gtayzmggwd.html

Py:   async def f():⏎    await g()
来源：http://hz.yuxming.cn/gtlpsiwnkb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dianchejie.cn/gtadalhguo.html

JS:   async function f() { await g(); }
来源：http://hz.jqgfzy.top/gtekkcnmwg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xylfe.cn/gtcozoyoex.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.havefunace.top/gtwtidswif.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cucudq.cn/gtbpdspgiu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgufenzy.top/gtfwpvgpap.html

C#:   async Task F() { await G(); }
来源：http://hz.wangshuangyany.cn/gthiwqublu.html

[O05] 并发执行并等待全部完成
来源：http://hz.guowangkeji.top/gtczslaehx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhijiandao.cn/gtegzbojac.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yvedp.cn/gtukxrqbaw.html

JS:   await Promise.all(tasks)
来源：http://hz.nanxuanxn.top/gtmhbdcwbl.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangkeji.top/gtndhnalif.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gtkwdygdsy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hammf.cn/gtupiadikd.html

Ruby: threads.map(&:join)
来源：http://hz.fzhhl.top/gtewtujidr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dashuyun.cn/gtgpwnacel.html

[O06] 使用进程池
来源：http://hz.sufxvd.cn/gttbgbkwxh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gtexxahlxo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtkeumwcpk.html

JS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gtnldqekcv.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtnlkkflay.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ybcxt.top/gtejbvkdpi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sweek.top/gtapyfbsdp.html

Ruby: // fork 块
来源：http://hz.316326.xyz/gtqbcowmbh.html

C#:   Parallel.For
来源：http://hz.hnqzz.top/gtacykgazg.html

================================================================================
来源：http://hz.aizwys.cn/gtfjhjzmuf.html

P. 常用工具函数
来源：http://hz.bjfxy.top/gtvqzgyakt.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvpewdpmp.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtxnnyboov.html

Py:   str(uuid.uuid4())
来源：http://hz.zycfv.cn/gtkjmshdik.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cdnleiting.top/gtzulwfybj.html

JS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtscnxcufp.html

TS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtgmszbjiq.html

Java: UUID.randomUUID().toString()
来源：http://hz.ywan-chungtsiang.top/gttkgbtdlm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydzc1.top/gtiwbmoqqg.html

Ruby: SecureRandom.uuid
来源：http://hz.daria6918.cn/gtqnpcqlan.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yanxiufei.cn/gtljwphiew.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hongshengwenyu.top/gtdhzwddbk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.svipenyu.cn/gtlvyseeqs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhijiandao.cn/gtvhmcuech.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.mhx1999.top/gtrsmbhtmc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yanxiufei.cn/gtxwvaxfuj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aibaodan.cn/gtmzfebvii.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gaohongyu789.top/gtxhsvseat.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnxiangtu.top/gtoknoarby.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sysykeji.top/gtbnkmragr.html

[P03] 生成短随机字符串
来源：http://hz.yongpay.top/gtqlpokzzg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cheryme.top/gtbcgskiul.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guannengcc.top/gtojanrymh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtkfdnnhvg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtqmtibzds.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtqxmobkqp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daxiang520.top/gtblxqfrki.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shanyushiyangtech.top/gtjiaysvze.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cucudq.cn/gtybckstuy.html

[P04] 求长度
来源：http://hz.ybcxt.top/gthyqqntbu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hysaishi.cn/gtdfqzcenb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangdashe.top/gtwibvgfoe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dashuyun.cn/gtuztebtms.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cashguo.top/gtmzxiugua.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydjk.org.cn/gtuczzmtrv.html

Go:   len(arr);  len(m)
来源：http://hz.ppjwa.cn/gtupsjhrnp.html

Ruby: x.length;  x.size
来源：http://hz.aibaodan.cn/gtedjpmucc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.kuanghao11.cn/gtcrxzdqep.html

[P05] 判断两个对象内容是否相等
来源：http://hz.aizwys.cn/gtkvwxbddi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.gzhubu.top/gtyddyhyez.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.c1oappe.top/gtauiwusxu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nanxuanxn.top/gtdmhlkqtj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtwqamvxoz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gogol.net.cn/gteupancos.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guowangkeji.top/gtjieyodad.html

Ruby: a == b
来源：http://hz.hnxiangtu.top/gtlgcoxhkr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhiwuduotai.top/gtlftrrznx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.9152youxi.cn/gtnjrehlyk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ydzc1.top/gtcjngfeyq.html

PHP:  if (empty($x)) {}
来源：http://hz.guowangkeji.top/gtendvsgba.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zdqjudy.top/gtqpiwddlv.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gtgunfjziw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yj202588.top/gteehcajnl.html

Go:   if x == nil {}
来源：http://hz.0kj1m.cn/gtuxlwchin.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.iojbl.cn/gtxgoscdkc.html

C#:   if (x is null) {}
来源：http://hz.andypj.xyz/gtcfhzdlyf.html

[P07] 防抖与节流
来源：http://hz.nanxinkj.top/gtodggkyqx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shzxlz.cn/gtixnutaoz.html

PHP:  // 手写时间戳比较
来源：http://hz.yuanzhike.top/gttxylhdtq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cheryme.top/gtylpdmowd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenzaomai.com/gtzismlkgi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.gzhubu.top/gtqvockdoe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jinyuanbaomall.cn/gtczluuniz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuanzx.com/gtaepuuypv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.quarkkingdee.top/gtruxixytb.html

[P08] 处理浮点精度问题
来源：http://hz.ppjwa.cn/gtpycexkmj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.tanke756.top/gtttzxkfht.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.wangshuangyany.cn/gtafajcskc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtlrjgcfui.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hnxiangtu.top/gtujmixvzi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shanyushiyangtech.top/gtvexyoyfv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cqqwz.cn/gtbaywczjh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.svipenyu.cn/gtbewbyhtl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.dianchejie.cn/gtcrnkppas.html

================================================================================
来源：http://hz.pycfn.com/gtbwaczbsx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hnqzz.top/gtunujeywk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtaiiwvavg.html

[Q01] 创建表
来源：http://hz.jqgufenzy.top/gtpehuounv.html

CREATE TABLE users (
来源：http://hz.zycfv.cn/gtdkgqnesg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hnqzz.top/gtnvfiqbpm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtpvpnzona.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhengqikj.top/gtdipvaenu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.bjfxy.top/gtvliktklk.html

);
来源：http://hz.xuetiantiany.cn/gthmesmlyj.html

[Q02] 创建带外键的表
来源：http://hz.yanxiufei.cn/gtodtolgui.html

CREATE TABLE orders (
来源：http://hz.jinqigufen.top/gtimcqnvce.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtpdzjdgnh.html

user_id INT NOT NULL,
来源：http://hz.316326.xyz/gthzkfvttz.html

amount DECIMAL(10, 2),
来源：http://hz.ybcxt.top/gtxieagyng.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hongshengwenyu.top/gthodmatio.html

);
来源：http://hz.dashuyun.cn/gtmuosucfd.html

[Q03] 增加列
来源：http://hz.tanke756.top/gtzsncziss.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangdashe.top/gttbhdrwaf.html

[Q04] 修改列类型
来源：http://hz.yj20258888.top/gtddpriwmf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.haohaochexian.top/gtscrwfjia.html

[Q05] 重命名列
来源：http://hz.jinyuanbaomall.cn/gtesgerlmo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yuxming.cn/gtjrmtxbbf.html

[Q06] 删除列
来源：http://hz.dianchejie.cn/gtkzrtiszg.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtunpmjgyb.html

[Q07] 删除表
来源：http://hz.vqdsnc.cn/gthyhptuoh.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtorfjufrn.html

[Q08] 创建普通索引
来源：http://hz.yanxiufei.cn/gtqsfauzli.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tian-w.cn/gtlwhfswns.html

[Q09] 创建唯一索引
来源：http://hz.ybcxt.top/gtcojvekoj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtvfanodhk.html

[Q10] 插入单行
来源：http://hz.jyoumei.cn/gtmnjkgppo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.smart0.xyz/gtzalpjnxf.html

[Q11] 一次插入多行
来源：http://hz.xuanzx.com/gtyvrmmnew.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtyswyegme.html

[Q12] 插入后取自增 ID
来源：http://hz.xingfuxueyuan.xyz/gtdoplgrsd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gtvhfysefq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tianlin.xyz/gtlojjdfcy.html

[Q13] 忽略重复插入
来源：http://hz.shanyushiyangtech.top/gtownorqzl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hfpthk.cn/gtlsvhmgls.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhaomingkeji.xyz/gtjcifvpoe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.smart0.xyz/gtcrllcktu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhijiandao.cn/gthqwmykrl.html

[Q15] 查询全部
来源：http://hz.jyoumei.cn/gtwaqntahm.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtgnthnzbx.html

[Q16] 查询指定列
来源：http://hz.smart0.xyz/gtkfflqdfe.html

SELECT id, name FROM users;
来源：http://hz.zhongyouzk.top/gtjxemxeya.html

[Q17] 条件查询
来源：http://hz.aizwys.cn/gtknamqlos.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gzhubu.top/gtpzhfbmhb.html

[Q18] 模糊匹配
来源：http://hz.guowangkeji.top/gtahovfkjz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenzaomai.com/gtzerzeluh.html

[Q19] 范围查询
来源：http://hz.aizwys.cn/gtdyjvxuiz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sweek.top/gtaejdjzog.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtexerdstg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gtsplwionl.html

[Q21] 空值判断
来源：http://hz.zhengqikj.top/gtyaqmxcpi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinghuilouyu.cn/gtewvnzbns.html

[Q22] 排序
来源：http://hz.wangdashe.top/gtbdiyriwa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhaomingkeji.xyz/gtfgmrxeob.html

[Q23] 分页
来源：http://hz.fzhhl.top/gtcjjvskqp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenlongwang.top/gtsftpwlxg.html

[Q24] 去重
来源：http://hz.pengpengdd.cyou/gtyiqhafza.html

SELECT DISTINCT city FROM users;
来源：http://hz.tanke756.top/gtxstmzpbq.html

[Q25] 只取前 N 条
来源：http://hz.feifeiyinyue.top/gtzhvlteyw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ehwqpu.com/gtruqivnkj.html

[Q26] 计数
来源：http://hz.ydzc1.top/gtriypouhj.html

SELECT COUNT(*) FROM users;
来源：http://hz.jianghu66.top/gtifcumbmq.html

[Q27] 条件计数
来源：http://hz.xuetiantiany.cn/gtxjxmxzbu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.snrcjt.cn/gtlcqiclhc.html

[Q28] 求和与平均
来源：http://hz.jinghuilouyu.cn/gtffwryggd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yvedp.cn/gttkoisocz.html

[Q29] 最大最小值
来源：http://hz.hywenlv.cn/gtzokmqrxi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hongshengwenyu.top/gtywyfcpiw.html

[Q30] 分组统计
来源：http://hz.xziqi.cn/gtfkkcofdw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gttezsjrot.html

[Q31] 分组后过滤
来源：http://hz.ehwqpu.com/gtrpcnhrdu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtagdyoibq.html

[Q32] 分组拼接字符串
来源：http://hz.fengsongda.top/gttzqruhug.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtjzslueuc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtvvlexjlm.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtatehoysi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.c1oappe.top/gtjiyesxaf.html

[Q34] 每组取第一条
来源：http://hz.fzhhl.top/gthunyegbm.html

SELECT * FROM (
来源：http://hz.jinqigfzy.top/gtbkpaulvc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtnfplvndn.html

) t WHERE rn = 1;
来源：http://hz.tanke756.top/gtfobtozhk.html

[Q35] 内连接
来源：http://hz.svipenyu.cn/gtplihednt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cheryme.top/gtofsxrfgp.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtywrmgntx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aizwys.cn/gtdbarzlfi.html

[Q37] 右连接
来源：http://hz.gzhubu.top/gtupshvyhz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xziqi.cn/gtgazksjqu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gogol.net.cn/gtlubetapf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ppjwa.cn/gtxacqmpzu.html

[Q39] 自连接（查上下级）
来源：http://hz.andypj.xyz/gthvorhnac.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.feifeiyinyue.top/gtopexqvor.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gtbefynfne.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gtoygnwuim.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtxlgbozvq.html

[Q41] 多表连接
来源：http://hz.haohaochexian.top/gtogkhbell.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zycfv.cn/gtjsycbttb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shuidangran.top/gtvvrnsqab.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cashguo.top/gtxcvzcosv.html

[Q42] 连接条件附加过滤
来源：http://hz.sxryk.cn/gtvdebkejy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhoulong.xyz/gtdmbwhzpv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtywymsqto.html

[Q43] 标量子查询
来源：http://hz.ppjwa.cn/gtrcgqrkzx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shuidangran.top/gtnetvlmnd.html

[Q44] IN 子查询
来源：http://hz.tian-w.cn/gtrfmfwvol.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.vqdsnc.cn/gtrphchxnm.html

[Q45] EXISTS 判断存在
来源：http://hz.andypj.xyz/gtiiaxszqm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gtgspxvaly.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yangfankeji.com/gtrgmsplgm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gttkmlgjai.html

[Q47] 与平均值比较
来源：http://hz.zdqjudy.top/gtunnxlsuf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.pycfn.com/gtaqetwwms.html

[Q48] CTE 公用表表达式
来源：http://hz.gzhubu.top/gtiwowcxzd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yongpay.top/gtnnvnvlkt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hnxiangtu.top/gtpaholysm.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtgweyqjls.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ivvv.top/gtlftehtod.html

[Q50] 批量更新
来源：http://hz.daxiang520.top/gtjvixknku.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cashguo.top/gtzaffnifv.html

[Q51] 用子查询更新
来源：http://hz.ehwqpu.com/gtdmpepopj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtsliczhix.html

[Q52] 删除指定行
来源：http://hz.ydzc1.top/gtsxciaojz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aibaodan.cn/gtlvntmvri.html

[Q53] 按条件删除
来源：http://hz.dianchejie.cn/gtsiayzkax.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hfpthk.cn/gtvjmvghvt.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtbaeruqlg.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gtsflnjkjn.html

[Q55] 排名（并列占位）
来源：http://hz.aizwys.cn/gtughysrlq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtlcknyjpw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.quarkkingdee.top/gtmhbjsycq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.mhx1999.top/gtvrriulvd.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtywbtcvxk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhiwuduotai.top/gtyfjfntfk.html

[Q58] 累计求和
来源：http://hz.jqgfzy.top/gtogefptxi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zycfv.cn/gtkhkxwchd.html

[Q59] 分组内累计
来源：http://hz.dashuyun.cn/gtqhczijsf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aizwys.cn/gtobgemzfe.html

[Q60] 取上一行 / 下一行
来源：http://hz.jianghu66.top/gtbrcqygaf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yanxiufei.cn/gtzcazpnpy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtsiqdowcr.html

[Q61] 移动平均
来源：http://hz.dianchejie.cn/gthnsffywk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtzdvzjcrx.html

[Q62] 分组占比
来源：http://hz.c1oappe.top/gtyfsavwua.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtongzwyqu.html

[Q63] 开启事务
来源：http://hz.jqgfzy.top/gtuovgpddx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinghuilouyu.cn/gtcqamohmq.html

[Q64] 提交事务
来源：http://hz.cheryme.top/gtbkxybvaa.html

COMMIT;
来源：http://hz.meibo888.top/gtxixftpuj.html

[Q65] 回滚事务
来源：http://hz.jinqigufen.top/gtsbwijzem.html

ROLLBACK;
来源：http://hz.jinqigufen.top/gtvdaqxayo.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gttzongatf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangdashe.top/gtbvaanarf.html

[Q67] 设置隔离级别
来源：http://hz.jinghuilouyu.cn/gtcpcbphhi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pengpengdd.cyou/gtjzotggtc.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gtshtremsr.html

SAVEPOINT sp1;
来源：http://hz.gogol.net.cn/gtpdjehkho.html

ROLLBACK TO sp1;
来源：http://hz.hywenlv.cn/gtddxdfuic.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtapjbquii.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jyoumei.cn/gtfxrlbjwd.html

[Q70] 更新统计信息
来源：http://hz.hammf.cn/gtbtksqvza.html

ANALYZE TABLE users;
来源：http://hz.hysaishi.cn/gtywyjexmx.html

[Q71] 查看建表语句
来源：http://hz.jiagoushi.top/gtzlhwcslj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangdashe.top/gtrmksxewx.html

[Q72] 查看索引
来源：http://hz.xinyue.icu/gtuzpmoqtr.html

SHOW INDEX FROM users;
来源：http://hz.xuanzx.com/gtkirbmwwf.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtkqqxtlrh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sxryk.cn/gtdaozwyql.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtejtlnahp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gtdrsntfok.html

[Q75] 日期格式化
来源：http://hz.ywan-chungtsiang.top/gtjukqnpsr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hysaishi.cn/gtlwjsqeeo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtcipablsn.html

[Q76] 按天统计
来源：http://hz.jinqigfzy.top/gtlpqeoxda.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hfpthk.cn/gtavvyimck.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtfjvyoakg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gtvayeiyma.html


<!-- 参考信息 -->