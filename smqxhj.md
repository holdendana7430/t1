代发 wailian999

[O02] 使用线程池
来源：http://hz.gaohongyu789.top/gtsrkwxhxr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhijiandao.cn/gtdyxctejm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.0kj1m.cn/gtkuqpmrht.html

JS:   // worker_threads 线程池
来源：http://hz.ydjk.org.cn/gtemjqlhhh.html

TS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtmsxmyopl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gtdewndpyx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.guannengcc.top/gtdvowpoam.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtohzdetdk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhiwuduotai.top/gtzjwjgmkx.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gtugknwdfr.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gtdzmiiccn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guowangkeji.top/gtmootenmc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pengpengdd.cyou/gtltaznfbs.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtpoktiapp.html

Java: synchronized (this) { shared++; }
来源：http://hz.aibaodan.cn/gtaovnvhny.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yanxiufei.cn/gteepftgqq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yonumen.top/gtrlqkelrl.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtjcezbhmx.html

[O04] 定义异步函数并等待
来源：http://hz.sufxvd.cn/gtmbisoegi.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangtech.top/gtifiltmhl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtzaksbpdb.html

JS:   async function f() { await g(); }
来源：http://hz.sysykeji.top/gtfwiwrrmh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cheryme.top/gtarsejukm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuanzx.com/gtmkzkwkqr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuanzhike.top/gtmriubtgq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gteqzxhzwf.html

C#:   async Task F() { await G(); }
来源：http://hz.cheryme.top/gtkyjxaetq.html

[O05] 并发执行并等待全部完成
来源：http://hz.shanyushiyangtech.top/gtakfrgtbh.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shuidangran.top/gtgszrluth.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangtech.top/gttazeliim.html

JS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtjzatsvih.html

TS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtfievixfd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shuidangran.top/gthtfsusqm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtrzjnxrkd.html

Ruby: threads.map(&:join)
来源：http://hz.xingfuxueyuan.xyz/gtwjjfoqjc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtkxtrbipb.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gtykfgmdtw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yuanzhike.top/gtllbdhxas.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tanke756.top/gtnsfyiaan.html

JS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtcedhskgc.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtdhkejylq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtkzowdxiz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ywan-chungtsiang.top/gtnifhdems.html

Ruby: // fork 块
来源：http://hz.gzhubu.top/gtbjuugycj.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtjxjxbxgv.html

================================================================================
来源：http://hz.tian-w.cn/gtklkubcid.html

P. 常用工具函数
来源：http://hz.jqgfzy.top/gtgorvhmrq.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnzwwspwk.html

[P01] 生成 UUID
来源：http://hz.c1oappe.top/gtmpuwiouo.html

Py:   str(uuid.uuid4())
来源：http://hz.xuanzx.com/gtpauorxni.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gtetgmzhqu.html

JS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtbnhnihsm.html

TS:   crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtzoynlran.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtjkjxohse.html

Go:   // 用 github.com/google/uuid
来源：http://hz.vqdsnc.cn/gtqfsewhmu.html

Ruby: SecureRandom.uuid
来源：http://hz.sweek.top/gtzaulbncu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sweek.top/gtdfjhwxgs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.snrcjt.cn/gtvmbyznyr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gtjsqisfmi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtvwtojaag.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtsalnnuzo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shangyingyoupin.top/gtdsqmuxbs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.c1oappe.top/gtrgbzuede.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.iojbl.cn/gtdznbjvby.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigufen.top/gtvdimebiq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.xuetiantiany.cn/gtgdadsuaj.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gtzbttooqe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.dianchejie.cn/gtqidbmgom.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.daria6918.cn/gtgyiekhet.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.snrcjt.cn/gtlusqyjrp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtdpusapid.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xinyue.icu/gtqryrctda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tian-w.cn/gthjpzsspl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jinghuilouyu.cn/gthtmrwkdl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.aizwys.cn/gtkbgxtawh.html

[P04] 求长度
来源：http://hz.xylfe.cn/gtgyriplcb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.wangdashe.top/gtxbwwhiwo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gthojveeex.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtggzdmqln.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hfpthk.cn/gtxgdzziqi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tanke756.top/gtqxxgrbln.html

Go:   len(arr);  len(m)
来源：http://hz.hywenlv.cn/gttwidmwlm.html

Ruby: x.length;  x.size
来源：http://hz.hywenlv.cn/gtezfuhwve.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.dashuyun.cn/gtqdvakejy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinqigufen.top/gttknhuivw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yanxiufei.cn/gthjttrmgm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.iojbl.cn/gtcrkzarsj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gthwisgqpi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gotoacloud.top/gtusycjnuh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnxiangtu.top/gtwmeiblzu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hysaishi.cn/gtnctnsfqr.html

Ruby: a == b
来源：http://hz.jinghuilouyu.cn/gtqdfywaju.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hongshengwenyu.top/gtyyfpyhqo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuanzhike.top/gtwxpsfelz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tanke756.top/gtoqcpdoep.html

PHP:  if (empty($x)) {}
来源：http://hz.hongshengwenyu.top/gtaodgbvdk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ppjwa.cn/gtaqfiayrl.html

TS:   if (x == null) {}
来源：http://hz.c1oappe.top/gtshrxlasi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gtuybhonsx.html

Go:   if x == nil {}
来源：http://hz.chenjidiqi.icu/gtormxtknq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.guowangkeji.top/gtsdbtrcen.html

C#:   if (x is null) {}
来源：http://hz.shangyingyoupin.top/gtpbdcbcgy.html

[P07] 防抖与节流
来源：http://hz.wangshuangyany.cn/gtrgdildsl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtedjvwguy.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtujxmfbvn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtzzwqzkyk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sweek.top/gtrsuqrxaf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtiytyhlux.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gtsewsbxvf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guannengcc.top/gtavdgrhma.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtomafrgvn.html

[P08] 处理浮点精度问题
来源：http://hz.kuanghao11.cn/gtstkkqgkc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.nanxinkj.top/gtuvdojwio.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yangfankeji.com/gtiyqkebtx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigufen.top/gtyxrhzqks.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.aibaodan.cn/gtvltgptha.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tian-w.cn/gtlrovclln.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258888.top/gtrvsezrmi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gtxjzzyjpj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgfzy.top/gtgoswqwwy.html

================================================================================
来源：http://hz.dianchejie.cn/gtmtnfoovi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yangfankeji.com/gtoohvpefz.html

================================================================================
来源：http://hz.cqqwz.cn/gtqnxxbaix.html

[Q01] 创建表
来源：http://hz.redwolf501.top/gtvpiicvxz.html

CREATE TABLE users (
来源：http://hz.yj20258888.top/gtfhdbrwwb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtbcyurdsc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hammf.cn/gtbhduaujm.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sweek.top/gtaexnniab.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.guannengcc.top/gtfqmjzsjo.html

);
来源：http://hz.yj202588.top/gtqzcckssx.html

[Q02] 创建带外键的表
来源：http://hz.bjfxy.top/gtwjerpsjv.html

CREATE TABLE orders (
来源：http://hz.daxiang520.top/gtcarlfcjf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtvmiipfss.html

user_id INT NOT NULL,
来源：http://hz.snrcjt.cn/gtvpxpqewj.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtdoodzzsa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yonumen.top/gtrvocqyel.html

);
来源：http://hz.zhixingplan.top/gtfqseljtv.html

[Q03] 增加列
来源：http://hz.xinyue.icu/gtvudgayxh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xziqi.cn/gtyuxrtfht.html

[Q04] 修改列类型
来源：http://hz.ydzc1.top/gtixwqbsmx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.ydjk.org.cn/gteykbcwso.html

[Q05] 重命名列
来源：http://hz.yanxiufei.cn/gtzalfamfp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtowconpim.html

[Q06] 删除列
来源：http://hz.shanyushiyangtech.top/gtjlfqsqkh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.haohaochexian.top/gtykchvktz.html

[Q07] 删除表
来源：http://hz.bjfxy.top/gtvaddkmhg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gtoqkkxyfa.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gtmklpnvfy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.ivvv.top/gtcjxhrgwe.html

[Q09] 创建唯一索引
来源：http://hz.aizwys.cn/gtvjyphqne.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.iojbl.cn/gtwjkcurvk.html

[Q10] 插入单行
来源：http://hz.guannengcc.top/gtfppkkfqe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xuetiantiany.cn/gtrpeswiqg.html

[Q11] 一次插入多行
来源：http://hz.jinyuanbaomall.cn/gtmuvvkjcx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yuxming.cn/gtdqzwfleh.html

[Q12] 插入后取自增 ID
来源：http://hz.yvedp.cn/gtdbvxtdid.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xylfe.cn/gtzylpxpph.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydzc1.top/gtvcpdzyvj.html

[Q13] 忽略重复插入
来源：http://hz.fengsongda.top/gtdcsydbbu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtohpulsfs.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtehqkjnlk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangshuangyany.cn/gtfpwgekhw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ywan-chungtsiang.top/gtbooiuxnt.html

[Q15] 查询全部
来源：http://hz.chenlongwang.top/gtwsjrmtuz.html

SELECT * FROM users;
来源：http://hz.gotoacloud.top/gtxqwjakwy.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtpojqtqol.html

SELECT id, name FROM users;
来源：http://hz.c1oappe.top/gtquvlaxwb.html

[Q17] 条件查询
来源：http://hz.jiagoushi.top/gtvvvwvsxz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pycfn.com/gtujvgkzdr.html

[Q18] 模糊匹配
来源：http://hz.yanxiufei.cn/gtefiquflg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.andypj.xyz/gtrnejspjh.html

[Q19] 范围查询
来源：http://hz.jinqigufen.top/gtlteztohc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigfzy.top/gtdldpbftg.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtunpypend.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtzolrgkqx.html

[Q21] 空值判断
来源：http://hz.chenzaomai.com/gtrvhdozoc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yvedp.cn/gtywljdzil.html

[Q22] 排序
来源：http://hz.316326.xyz/gtvpgzsdgn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangkeji.top/gttjopltop.html

[Q23] 分页
来源：http://hz.52xcode.cn/gtlwdujufk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yanxiufei.cn/gttabjnpoo.html

[Q24] 去重
来源：http://hz.shanyushiyangtech.top/gtentcqdxv.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgufenzy.top/gttnblaypy.html

[Q25] 只取前 N 条
来源：http://hz.iojbl.cn/gtsbzhleez.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtjqbkhmdk.html

[Q26] 计数
来源：http://hz.yanxiufei.cn/gttlwamapr.html

SELECT COUNT(*) FROM users;
来源：http://hz.sufxvd.cn/gtsaqwikho.html

[Q27] 条件计数
来源：http://hz.yongpay.top/gtmkmiqxni.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhaomingkeji.xyz/gtpgsrhzjp.html

[Q28] 求和与平均
来源：http://hz.hfpthk.cn/gtwedzrxjk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.daria6918.cn/gtutbuerib.html

[Q29] 最大最小值
来源：http://hz.cdnleiting.top/gthbnrqekf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gtruqjcavq.html

[Q30] 分组统计
来源：http://hz.zhixingplan.top/gtzouawblm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtvtsmkpec.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtovvnkave.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cucudq.cn/gtnxzdybdo.html

[Q32] 分组拼接字符串
来源：http://hz.yongpay.top/gtyrarcesw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtskmhmwxz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hongshengwenyu.top/gtirshkmrc.html

[Q33] 多列分组
来源：http://hz.xziqi.cn/gtxzmeayog.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.haohaochexian.top/gtgnrpexpd.html

[Q34] 每组取第一条
来源：http://hz.daria6918.cn/gtiggtnocs.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtkbzuaedo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yueranfly.top/gtdzhrrtvl.html

) t WHERE rn = 1;
来源：http://hz.gzhubu.top/gticgpvxmh.html

[Q35] 内连接
来源：http://hz.dashuyun.cn/gtrxvoycpw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtkgjodneo.html

[Q36] 左连接
来源：http://hz.mhx1999.top/gtabaovjrm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.vqdsnc.cn/gtungvzebp.html

[Q37] 右连接
来源：http://hz.tianlin.xyz/gtmegsguci.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zdqjudy.top/gtyhwvlcda.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yonumen.top/gtaxrwlbqu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gthfckxzta.html

[Q39] 自连接（查上下级）
来源：http://hz.daria6918.cn/gtkxxgbixg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hnxiangtu.top/gtdzhjqrea.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnxiangtu.top/gtlslygney.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydjk.org.cn/gtyneuqgzw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gtkbebicmh.html

[Q41] 多表连接
来源：http://hz.jinyuanbaomall.cn/gtphirxdkt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258.top/gtuzyrojfd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhongyouzk.top/gturlzfpzx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnqzz.top/gtvlwzfvpf.html

[Q42] 连接条件附加过滤
来源：http://hz.hammf.cn/gttiexhkii.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jiagoushi.top/gtbdanmrly.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guannengcc.top/gtwyypmzkt.html

[Q43] 标量子查询
来源：http://hz.cashguo.top/gtesgkcgvx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gotoacloud.top/gtvkffrisz.html

[Q44] IN 子查询
来源：http://hz.meibo888.top/gtpuedacgi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xingfuxueyuan.xyz/gtvygfxqfm.html

[Q45] EXISTS 判断存在
来源：http://hz.yvedp.cn/gtyhsruiez.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtcznibfbd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shanyushiyangkeji.top/gtwneovmnz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gaohongyu789.top/gtbwokrrvr.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtmyqfkmlt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtripaipre.html

[Q48] CTE 公用表表达式
来源：http://hz.ywan-chungtsiang.top/gtyzxyqqez.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinghuilouyu.cn/gtdrcpwqiq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sysykeji.top/gtbfsiljwk.html

[Q49] 更新单行
来源：http://hz.jiagoushi.top/gtzxirsdvl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigfzy.top/gtsvvhpsju.html

[Q50] 批量更新
来源：http://hz.iojbl.cn/gtkjwwppzg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nwbrower.top/gtvtztuszd.html

[Q51] 用子查询更新
来源：http://hz.yongpay.top/gtvcrsghrk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.daxiang520.top/gttldyawer.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtrvpslvvx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.316326.xyz/gtlzkgbzop.html

[Q53] 按条件删除
来源：http://hz.yangfankeji.com/gtzrdtgyas.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhijiandao.cn/gtluemgkms.html

[Q54] 清空表
来源：http://hz.shanyushiyangkeji.top/gtneeymogl.html

TRUNCATE TABLE logs;
来源：http://hz.dashuyun.cn/gtqmjygwon.html

[Q55] 排名（并列占位）
来源：http://hz.jqgufenzy.top/gtkpahvbub.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtldlbnyoa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jyoumei.cn/gtsnsltopg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtvmvgphhw.html

[Q57] 行号
来源：http://hz.hongshengwenyu.top/gtbivribye.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtdztdliia.html

[Q58] 累计求和
来源：http://hz.jinqigfzy.top/gtvrbnvysj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pycfn.com/gtowhldnjg.html

[Q59] 分组内累计
来源：http://hz.quarkkingdee.top/gtuedbfjds.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aibaodan.cn/gtkolyyztf.html

[Q60] 取上一行 / 下一行
来源：http://hz.iojbl.cn/gtlpdpdvsk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.kuanghao11.cn/gtghollcnn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhiwuduotai.top/gtzmujfyql.html

[Q61] 移动平均
来源：http://hz.dashuyun.cn/gtigsojofw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gthwqcbzpr.html

[Q62] 分组占比
来源：http://hz.smart0.xyz/gtrhibcdze.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtorhtqkkv.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gteoecjlxg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gtyhkrzpcx.html

[Q64] 提交事务
来源：http://hz.zhijiandao.cn/gtewmyautn.html

COMMIT;
来源：http://hz.yanxiufei.cn/gtphtarylw.html

[Q65] 回滚事务
来源：http://hz.svipenyu.cn/gtpednrgsa.html

ROLLBACK;
来源：http://hz.316326.xyz/gtacryrjrn.html

[Q66] 行锁查询
来源：http://hz.jinqigfzy.top/gtznivlrmw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258.top/gtypziauzs.html

[Q67] 设置隔离级别
来源：http://hz.wangdashe.top/gtediapgxk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtomgjlvfe.html

[Q68] 保存点
来源：http://hz.xingfuxueyuan.xyz/gtndlavhfa.html

SAVEPOINT sp1;
来源：http://hz.shangyingyoupin.top/gtmlvurwvk.html

ROLLBACK TO sp1;
来源：http://hz.yonumen.top/gtrrqsbcdu.html

[Q69] 查看执行计划
来源：http://hz.yonumen.top/gthzvvjeto.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hywenlv.cn/gttybvqghf.html

[Q70] 更新统计信息
来源：http://hz.sxryk.cn/gtssiqkguh.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtomrbowmg.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gtyzuzmkjm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.feifeiyinyue.top/gtzvcscdrv.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gttxtuajzb.html

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtwwvkhmqv.html

[Q73] 查看表状态
来源：http://hz.xuanzx.com/gtdfukkbgh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sxryk.cn/gttfnfshpd.html

[Q74] 强制使用索引
来源：http://hz.yj20258888.top/gtapgascdw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhongyouzk.top/gtmvdsiflp.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gtekwuzkym.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hysaishi.cn/gtpcgctcwa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnqzz.top/gtvphtdujp.html

[Q76] 按天统计
来源：http://hz.chenlongwang.top/gttlmqxnes.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gogol.net.cn/gtjbqwcefi.html

[Q77] 时间加减
来源：http://hz.xuanzx.com/gtpitnwfes.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhixingplan.top/gtvaqzpjyo.html


<!-- 参考信息 -->