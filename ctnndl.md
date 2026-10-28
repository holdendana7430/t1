代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hongshengwenyu.top/gtylmbodgr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.9152youxi.cn/gtxxmucdqt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ybcxt.top/gtmfxkugap.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtlcnlccwx.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtqygzinbs.html

Go:   go f()
来源：http://hz.xinyue.icu/gtgqwxtcve.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gthsgctlhs.html

C#:   Task.Run(() => F());
来源：http://hz.jqgfzy.top/gtswjyqsky.html

[O02] 使用线程池
来源：http://hz.yanxiufei.cn/gtiylmbwhp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shzxlz.cn/gtzkvxfaom.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yangfankeji.com/gtfkybcbby.html

JS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtwtyymdwp.html

TS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtxcgsxeej.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangtech.top/gtyushnefa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtdwnwquia.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtjkfleokx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.haohaochexian.top/gthewnzcri.html

[O03] 加锁保护共享数据
来源：http://hz.jinyuanbaomall.cn/gtqdjqbtgd.html

Py:   with lock: shared += 1
来源：http://hz.chenzaomai.com/gtnlsuzcco.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gzhubu.top/gtxtotkslq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangtech.top/gtpkivgrmk.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gthjkbcbch.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtbonuasto.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.iojbl.cn/gtzgcxtvie.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jiagoushi.top/gthfwpupiv.html

C#:   lock (gate) { shared++; }
来源：http://hz.andypj.xyz/gtcfstmfvn.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtsnhckbcw.html

Py:   async def f():⏎    await g()
来源：http://hz.nwbrower.top/gtrcytqebf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.0kj1m.cn/gtdrdwwncf.html

JS:   async function f() { await g(); }
来源：http://hz.chenlongwang.top/gtetkbtnyv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.havefunace.top/gturerxdlv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gtsjwksktn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jlsjyb.cn/gtbszneoph.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.dianchejie.cn/gtvhyozxoy.html

C#:   async Task F() { await G(); }
来源：http://hz.snrcjt.cn/gtbyovnuyy.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gttfnztkdc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.redwolf501.top/gtkujkllnh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.feifeiyinyue.top/gtcrxymepg.html

JS:   await Promise.all(tasks)
来源：http://hz.fengsongda.top/gtkrhegbxn.html

TS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtaifgirol.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cucudq.cn/gtpatwcqcz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.daria6918.cn/gthwzeagjt.html

Ruby: threads.map(&:join)
来源：http://hz.hammf.cn/gtfriokvvl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.mhx1999.top/gtprnbsgao.html

[O06] 使用进程池
来源：http://hz.nwbrower.top/gtonasjlbq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinyuanbaomall.cn/gtylerzqvg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.bjfxy.top/gtqusaibbg.html

JS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtxzgwhetd.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtokcckanb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sysykeji.top/gtqqypepyy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ehwqpu.com/gtgzaevoei.html

Ruby: // fork 块
来源：http://hz.ppjwa.cn/gtzxdyjaqw.html

C#:   Parallel.For
来源：http://hz.hywenlv.cn/gtdbfbwjuu.html

================================================================================
来源：http://hz.xylfe.cn/gtrdxpxpfa.html

P. 常用工具函数
来源：http://hz.iojbl.cn/gtfgbmozsf.html

================================================================================
来源：http://hz.fzhhl.top/gtkljeishw.html

[P01] 生成 UUID
来源：http://hz.yj202588.top/gtgmkdaavq.html

Py:   str(uuid.uuid4())
来源：http://hz.hysaishi.cn/gtvqktrjlh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigufen.top/gtrbkifhtl.html

JS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gthuunoojh.html

TS:   crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gthdpqzncn.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxinkj.top/gtdpngjxsq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tianlin.xyz/gtzalixxkd.html

Ruby: SecureRandom.uuid
来源：http://hz.gzhubu.top/gthelpjbwg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gtjsthgpfe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cucudq.cn/gtofrxwfbf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hammf.cn/gtlzcgkpys.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuetiantiany.cn/gtokealbln.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xuanzx.com/gtjxwhmcgc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tianlin.xyz/gtffhbhzld.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yongpay.top/gtxnyzckai.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gtxcckyuif.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.smart0.xyz/gtszmjzgty.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yangfankeji.com/gtdxhnlxxp.html

[P03] 生成短随机字符串
来源：http://hz.zhixingplan.top/gtcrldcien.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shangyingyoupin.top/gtonmsmufl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinqigfzy.top/gtszqmbfbh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtvzmxfxvn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gthaqiuoyj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.andypj.xyz/gtjlpgnzwj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shzxlz.cn/gtqfvkoczq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gtlcmojlul.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yangfankeji.com/gtzyekgabk.html

[P04] 求长度
来源：http://hz.zhixingplan.top/gtmbbubjuv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gtxucpcykf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xinyue.icu/gtyozxlacd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cucudq.cn/gtnrybkmtl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.smart0.xyz/gtsguyhrcc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtfshbvyzs.html

Go:   len(arr);  len(m)
来源：http://hz.hfpthk.cn/gtzwoangws.html

Ruby: x.length;  x.size
来源：http://hz.kuanghao11.cn/gtuxcwhngl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cdnleiting.top/gtflcjadbq.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gogol.net.cn/gtbxawhxje.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinyuanbaomall.cn/gthjtbewhr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gttbncvyrw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jyoumei.cn/gtazqalxnr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtjjtkzjmd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhengqikj.top/gtrpivixed.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hfpthk.cn/gtqdfxbjdp.html

Ruby: a == b
来源：http://hz.mhx1999.top/gtounlougj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhixingplan.top/gttambluyi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hnxiangtu.top/gtbuxveifo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.9152youxi.cn/gtwmwqltly.html

PHP:  if (empty($x)) {}
来源：http://hz.yongpay.top/gtcqwglefa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydjk.org.cn/gtssjphqvz.html

TS:   if (x == null) {}
来源：http://hz.yuanzhike.top/gtyfbsbbyu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ivvv.top/gtkauflcds.html

Go:   if x == nil {}
来源：http://hz.havefunace.top/gtjmfhdsqg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yj20258.top/gthmdafcyu.html

C#:   if (x is null) {}
来源：http://hz.chenjidiqi.icu/gtqbravvkk.html

[P07] 防抖与节流
来源：http://hz.yueranfly.top/gtuxmmrpjs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.andypj.xyz/gtbvwmxzft.html

PHP:  // 手写时间戳比较
来源：http://hz.guannengcc.top/gtksrfxziq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cucudq.cn/gtgvdjshih.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtxmumlrbb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.wangshuangyany.cn/gtxrodyhec.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aibaodan.cn/gtybpvsrdx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuetiantiany.cn/gthmtylpks.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ywan-chungtsiang.top/gtwkvvxmgw.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtceazegqu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yonumen.top/gtjzvitfmm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gogol.net.cn/gtkyzrxhug.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.shuidangran.top/gtgfjglxnd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tianlin.xyz/gtjbjlwpou.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.svipenyu.cn/gttaqgwgan.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnxiangtu.top/gtpddzklof.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daxiang520.top/gtncyttben.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.havefunace.top/gtpahmxykp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpyfolupb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gaohongyu789.top/gtbijvbhmg.html

================================================================================
来源：http://hz.c1oappe.top/gtrtkrmhdb.html

[Q01] 创建表
来源：http://hz.ehwqpu.com/gthkhulhkf.html

CREATE TABLE users (
来源：http://hz.kuanghao11.cn/gtytesvdts.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtvovxsdrj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenlongwang.top/gtujkwhdhw.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ybcxt.top/gtszbkimog.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hfpthk.cn/gtiuzrqvgl.html

);
来源：http://hz.jianghu66.top/gtgotiojit.html

[Q02] 创建带外键的表
来源：http://hz.hysaishi.cn/gtekzqobkv.html

CREATE TABLE orders (
来源：http://hz.zhoulong.xyz/gtsdqjizsf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtgzirabjl.html

user_id INT NOT NULL,
来源：http://hz.svipenyu.cn/gtcijqplyw.html

amount DECIMAL(10, 2),
来源：http://hz.sxryk.cn/gtuhizuvuo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.gzhubu.top/gtqarhvstz.html

);
来源：http://hz.xuetiantiany.cn/gtgmtlchqi.html

[Q03] 增加列
来源：http://hz.chenzaomai.com/gtfpzicbys.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.fzhhl.top/gtvdstjdpb.html

[Q04] 修改列类型
来源：http://hz.gzhubu.top/gtutxftbqv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shanyushiyangkeji.top/gtjewjiyii.html

[Q05] 重命名列
来源：http://hz.meibo888.top/gtaadkulbk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yvedp.cn/gtgqnaghwp.html

[Q06] 删除列
来源：http://hz.zhoulong.xyz/gtdjhkpkjw.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.wangshuangyany.cn/gtuvuqwnfa.html

[Q07] 删除表
来源：http://hz.ydjk.org.cn/gtddjnpdlk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.mhx1999.top/gtkqlqlpgp.html

[Q08] 创建普通索引
来源：http://hz.52xcode.cn/gtoreibrkj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cqqwz.cn/gttglyanoj.html

[Q09] 创建唯一索引
来源：http://hz.mhx1999.top/gttvixjusm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtoblxhuaq.html

[Q10] 插入单行
来源：http://hz.svipenyu.cn/gtarwyebvr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cqqwz.cn/gtxivtjaet.html

[Q11] 一次插入多行
来源：http://hz.c1oappe.top/gtoaadnlve.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.aibaodan.cn/gtnomdfsjj.html

[Q12] 插入后取自增 ID
来源：http://hz.sxryk.cn/gtphlfklsr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jqgufenzy.top/gtnbxsedxq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhixingplan.top/gtkndgmfpx.html

[Q13] 忽略重复插入
来源：http://hz.yanxiufei.cn/gtapoprqkf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xylfe.cn/gtwzsexspj.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtvvngxgcf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cheryme.top/gtnldtsaqq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtzcurhdih.html

[Q15] 查询全部
来源：http://hz.sweek.top/gthvqyqfgr.html

SELECT * FROM users;
来源：http://hz.hnqzz.top/gtkvpkzgce.html

[Q16] 查询指定列
来源：http://hz.xylfe.cn/gtsfplvxvw.html

SELECT id, name FROM users;
来源：http://hz.jianghu66.top/gtczvahpmm.html

[Q17] 条件查询
来源：http://hz.ybcxt.top/gthlaepfvf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.316326.xyz/gtnqydlhnj.html

[Q18] 模糊匹配
来源：http://hz.gaohongyu789.top/gtjftnghhu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnqzz.top/gtdmfojlkl.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtpwuiykgy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jlsjyb.cn/gtgmqkwiwt.html

[Q20] IN 列表
来源：http://hz.yongpay.top/gtvtgytcte.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fengsongda.top/gtudapdwuw.html

[Q21] 空值判断
来源：http://hz.zhongyouzk.top/gtixvlbipk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ppjwa.cn/gtiblsgkni.html

[Q22] 排序
来源：http://hz.guannengcc.top/gtosccskun.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenlongwang.top/gttevnumws.html

[Q23] 分页
来源：http://hz.0kj1m.cn/gtxqemwyxl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhijiandao.cn/gtkepfbjlo.html

[Q24] 去重
来源：http://hz.nanxuanxn.top/gtbmyvtoew.html

SELECT DISTINCT city FROM users;
来源：http://hz.xuanzx.com/gtiwnuihln.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtifqhgiwm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hysaishi.cn/gtogobmcrf.html

[Q26] 计数
来源：http://hz.xinyue.icu/gtaxthpakr.html

SELECT COUNT(*) FROM users;
来源：http://hz.jianghu66.top/gtnlavystd.html

[Q27] 条件计数
来源：http://hz.zhixingplan.top/gtzqnqoexy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.daxiang520.top/gtocbefitl.html

[Q28] 求和与平均
来源：http://hz.jinqigfzy.top/gtxorfpvcc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtxuxsbmqh.html

[Q29] 最大最小值
来源：http://hz.nanxuanxn.top/gtmsblnnph.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dashuyun.cn/gtucunsusj.html

[Q30] 分组统计
来源：http://hz.hnqzz.top/gtzjdnaisy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gthymplrnr.html

[Q31] 分组后过滤
来源：http://hz.yuanzhike.top/gtcwtuelcn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.fzhhl.top/gtppmtslbh.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtzycjkyuw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtvywqtjqx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jianghu66.top/gtfvzppeup.html

[Q33] 多列分组
来源：http://hz.jiagoushi.top/gtryffdkbo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gaohongyu789.top/gtmxcpurti.html

[Q34] 每组取第一条
来源：http://hz.jqgfzy.top/gtiroorose.html

SELECT * FROM (
来源：http://hz.ivvv.top/gteshvbeqi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtxrgrpadn.html

) t WHERE rn = 1;
来源：http://hz.aizwys.cn/gtmewckqyx.html

[Q35] 内连接
来源：http://hz.xziqi.cn/gthxvizhjf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yueranfly.top/gthqyajvlm.html

[Q36] 左连接
来源：http://hz.tanke756.top/gthbyjhtlj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zdqjudy.top/gtumaufqzw.html

[Q37] 右连接
来源：http://hz.redwolf501.top/gtpiueecij.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shzxlz.cn/gtnvxlcjly.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xziqi.cn/gtcowertid.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtygwrcybw.html

[Q39] 自连接（查上下级）
来源：http://hz.ydjk.org.cn/gtvwbvusfw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtdlqpemdz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shzxlz.cn/gtuhpuptxj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgufenzy.top/gtsvtsfnjo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtvzixcjop.html

[Q41] 多表连接
来源：http://hz.jqgufenzy.top/gtsgacdhqp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhoulong.xyz/gtzixssrbt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shangyingyoupin.top/gtymhigpln.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.snrcjt.cn/gtcnenoiou.html

[Q42] 连接条件附加过滤
来源：http://hz.jianghu66.top/gtzmhxgjdp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tanke756.top/gtdkgzmmrt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangdashe.top/gtcycnryax.html

[Q43] 标量子查询
来源：http://hz.feifeiyinyue.top/gtxqtjbyvy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jyoumei.cn/gtnnjsaqjr.html

[Q44] IN 子查询
来源：http://hz.shangyingyoupin.top/gtydhgwrds.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daria6918.cn/gtivolwvgi.html

[Q45] EXISTS 判断存在
来源：http://hz.0kj1m.cn/gteknclamz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.316326.xyz/gtpzjfklfi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.feifeiyinyue.top/gtogvbgcfk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sweek.top/gtwppeypng.html

[Q47] 与平均值比较
来源：http://hz.yj202588.top/gtydywchwa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.c1oappe.top/gtgrgefdvz.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gtyjoemogg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jlsjyb.cn/gtxcklyuhr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydzc1.top/gtkguftggs.html

[Q49] 更新单行
来源：http://hz.ywan-chungtsiang.top/gtbvysbuij.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sweek.top/gtbfkcqvwc.html

[Q50] 批量更新
来源：http://hz.dashuyun.cn/gtoeustync.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.meibo888.top/gtbnepropx.html

[Q51] 用子查询更新
来源：http://hz.smart0.xyz/gtzxprwiwe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtzienvpks.html

[Q52] 删除指定行
来源：http://hz.xziqi.cn/gtdxnureji.html

DELETE FROM users WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtayjlafat.html

[Q53] 按条件删除
来源：http://hz.ybcxt.top/gtcadzmpub.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.redwolf501.top/gtklnkanto.html

[Q54] 清空表
来源：http://hz.pengpengdd.cyou/gtkedqvbzi.html

TRUNCATE TABLE logs;
来源：http://hz.hfpthk.cn/gtohztmdqx.html

[Q55] 排名（并列占位）
来源：http://hz.gaohongyu789.top/gtmtgmwvqs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xinyue.icu/gtnlarrwbi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtfwumljcj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.quarkkingdee.top/gtqemmysin.html

[Q57] 行号
来源：http://hz.sysykeji.top/gtvtrvljnz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daxiang520.top/gtbipzklpt.html

[Q58] 累计求和
来源：http://hz.bjfxy.top/gtjgtflrio.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gthueoybkm.html

[Q59] 分组内累计
来源：http://hz.svipenyu.cn/gtstlwhzsj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fengsongda.top/gtdaiclhvx.html

[Q60] 取上一行 / 下一行
来源：http://hz.hfpthk.cn/gtdtsdjmmx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.316326.xyz/gterdbnnku.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xziqi.cn/gtgffbnxdu.html

[Q61] 移动平均
来源：http://hz.yj20258.top/gtrcxbhfln.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtzyehqvxn.html

[Q62] 分组占比
来源：http://hz.aizwys.cn/gtlyobfrbp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhengqikj.top/gtiyanfdxt.html

[Q63] 开启事务
来源：http://hz.svipenyu.cn/gtfeonjdlx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hammf.cn/gtqraiwgiv.html

[Q64] 提交事务
来源：http://hz.shuidangran.top/gttwvchdea.html

COMMIT;
来源：http://hz.cheryme.top/gtpfqlpoqr.html

[Q65] 回滚事务
来源：http://hz.zhijiandao.cn/gtoeqhijmw.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtsaxdshjo.html

[Q66] 行锁查询
来源：http://hz.yongpay.top/gtbxzzezdx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hysaishi.cn/gttirrgpqj.html

[Q67] 设置隔离级别
来源：http://hz.chenlongwang.top/gtfinkcbzl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hammf.cn/gtacduydze.html

[Q68] 保存点
来源：http://hz.meibo888.top/gtihyaamsu.html

SAVEPOINT sp1;
来源：http://hz.cucudq.cn/gtgrfnjvuj.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtkhnvhqio.html

[Q69] 查看执行计划
来源：http://hz.daxiang520.top/gtnzzzzdrm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.iojbl.cn/gtetuuugpo.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gtfnnrqtuh.html

ANALYZE TABLE users;
来源：http://hz.nwbrower.top/gtfxbizigl.html

[Q71] 查看建表语句
来源：http://hz.cashguo.top/gtyfqktwqt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aizwys.cn/gtfignqaut.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtsclumqyq.html

SHOW INDEX FROM users;
来源：http://hz.iojbl.cn/gttbsyhkpf.html

[Q73] 查看表状态
来源：http://hz.sweek.top/gtyxjzwdqh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fengsongda.top/gtgxpgnaqa.html

[Q74] 强制使用索引
来源：http://hz.jqgfzy.top/gtlvcsjrzz.html


<!-- 参考信息 -->