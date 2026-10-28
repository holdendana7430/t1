代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hongshengwenyu.top/gtswhxwlxf.html

[O03] 加锁保护共享数据
来源：http://hz.cheryme.top/gtvueywgga.html

Py:   with lock: shared += 1
来源：http://hz.ivvv.top/gtyqawgiyu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtmernpnbl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.meibo888.top/gthyauagoy.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtgsefqnyb.html

Java: synchronized (this) { shared++; }
来源：http://hz.nwbrower.top/gthbcwhtuh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yvedp.cn/gtofkkeamo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgufenzy.top/gtzvzvqzci.html

C#:   lock (gate) { shared++; }
来源：http://hz.fengsongda.top/gtgxqwqsrm.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gtepcbtyoc.html

Py:   async def f():⏎    await g()
来源：http://hz.cashguo.top/gthathblzb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.fzhhl.top/gtjwilugcw.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtjlqpbqri.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258888.top/gtiadrjtig.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xuetiantiany.cn/gtarzfjjsi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xziqi.cn/gtvrpqsaba.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tian-w.cn/gtqkvspkzv.html

C#:   async Task F() { await G(); }
来源：http://hz.kuanghao11.cn/gtlcwavtsh.html

[O05] 并发执行并等待全部完成
来源：http://hz.sufxvd.cn/gtbuxwjjbg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhijiandao.cn/gtdgifgfwk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtnhsfblai.html

JS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gtoadgzife.html

TS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtheujyiyz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.haohaochexian.top/gtcvvhiaed.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.smart0.xyz/gtabkuhvwv.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtkzrrispq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cucudq.cn/gtvvziligo.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtsgojnipc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.smart0.xyz/gtlkmvgwrb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hfpthk.cn/gtwjgyorfg.html

JS:   // child_process / cluster 模块
来源：http://hz.cdnleiting.top/gtuusabxen.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtvycigprr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zdqjudy.top/gtnsqjszjx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinghuilouyu.cn/gtfbmlahmy.html

Ruby: // fork 块
来源：http://hz.sufxvd.cn/gtouspziee.html

C#:   Parallel.For
来源：http://hz.ydjk.org.cn/gtmtctkvhs.html

================================================================================
来源：http://hz.yj202588.top/gtxfkzzyvu.html

P. 常用工具函数
来源：http://hz.yongpay.top/gtgnjjakud.html

================================================================================
来源：http://hz.andypj.xyz/gtlcwtoivt.html

[P01] 生成 UUID
来源：http://hz.chenlongwang.top/gtatmxqtim.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gtdjeqozxt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtxseeedix.html

JS:   crypto.randomUUID()
来源：http://hz.redwolf501.top/gthcbciwaf.html

TS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtstdcjllx.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gtcrlfxftc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jyoumei.cn/gtnecdhnye.html

Ruby: SecureRandom.uuid
来源：http://hz.meibo888.top/gtaozuvxmi.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.kuanghao11.cn/gtjashjdaw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgufenzy.top/gtnmkcpkik.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gtitftozfx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtdtoaftzv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258888.top/gtilmcaflk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.9152youxi.cn/gttxcgyteb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jianghu66.top/gtnlzvbdod.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gotoacloud.top/gtlumwzapi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sxryk.cn/gthwbekkny.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.pengpengdd.cyou/gtkxfmflta.html

[P03] 生成短随机字符串
来源：http://hz.cucudq.cn/gtfwfszpas.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtxqqgqilb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jqgufenzy.top/gtphsevtto.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtceevwabr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gtxwedgrhy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gthlovsyvx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhoulong.xyz/gtbbuetwfs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.meibo888.top/gteqdwvrgy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.0kj1m.cn/gtlovxyjds.html

[P04] 求长度
来源：http://hz.jiagoushi.top/gtzncumoqi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuanzx.com/gtlrilmzbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtqjknornx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtyyaqguix.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtaqmlpfdv.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gaohongyu789.top/gthhktufce.html

Go:   len(arr);  len(m)
来源：http://hz.snrcjt.cn/gtnyscpffc.html

Ruby: x.length;  x.size
来源：http://hz.jiagoushi.top/gtwbaehdby.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtvlmcdsbk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.52xcode.cn/gtmkukmibb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.bjfxy.top/gtylbibxrt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.xuetiantiany.cn/gtnmpourdf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgfzy.top/gtoeeaxmep.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtekmlrjcf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sxryk.cn/gtgvdywvxz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gogol.net.cn/gtuuzlmcpq.html

Ruby: a == b
来源：http://hz.jinghuilouyu.cn/gtasbziqkq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhijiandao.cn/gtlxypgweh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gogol.net.cn/gtcgjqhkyj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yongpay.top/gtkropfqha.html

PHP:  if (empty($x)) {}
来源：http://hz.xinyue.icu/gtrnfpvbes.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenjidiqi.icu/gtkfkagurp.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gtesxcesst.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.cucudq.cn/gtkvhsdknb.html

Go:   if x == nil {}
来源：http://hz.tian-w.cn/gticcqeifs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yonumen.top/gtluhkpczz.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtazrdidnx.html

[P07] 防抖与节流
来源：http://hz.cucudq.cn/gtjetppmlk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zycfv.cn/gtriepkhyw.html

PHP:  // 手写时间戳比较
来源：http://hz.hnxiangtu.top/gtjhadydmw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aibaodan.cn/gtywvvgphn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.snrcjt.cn/gttuhsmxea.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zdqjudy.top/gtyaqanuox.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yvedp.cn/gtxzmlrgsv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.vqdsnc.cn/gtxldwyiis.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.smart0.xyz/gtxfgpwjrq.html

[P08] 处理浮点精度问题
来源：http://hz.jinyuanbaomall.cn/gtwzyqkgte.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhixingplan.top/gtdsfynzpo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aizwys.cn/gtatkqilrd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gzhubu.top/gturvqwzqd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hammf.cn/gtvbiaeohw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenzaomai.com/gtfmrrniem.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gotoacloud.top/gtewrfhoyq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hfpthk.cn/gtpmdbpdrx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sxryk.cn/gtkanqblox.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtlcbhkqpo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shzxlz.cn/gtirjkecbq.html

================================================================================
来源：http://hz.redwolf501.top/gtmupstbnz.html

[Q01] 创建表
来源：http://hz.quarkkingdee.top/gtpbxzbowq.html

CREATE TABLE users (
来源：http://hz.316326.xyz/gtenkqxpyj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gthfbgxlkl.html

name VARCHAR(50) NOT NULL,
来源：http://hz.haohaochexian.top/gtidployqa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhixingplan.top/gtbydidgmb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.snrcjt.cn/gthrszkbzm.html

);
来源：http://hz.chenlongwang.top/gtglpxlffg.html

[Q02] 创建带外键的表
来源：http://hz.xziqi.cn/gttrykypvb.html

CREATE TABLE orders (
来源：http://hz.dashuyun.cn/gtslxbjvqp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jqgufenzy.top/gtzhqvzlow.html

user_id INT NOT NULL,
来源：http://hz.zhoulong.xyz/gtpsunzufi.html

amount DECIMAL(10, 2),
来源：http://hz.cqqwz.cn/gtevtikmoq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cqqwz.cn/gtectdikak.html

);
来源：http://hz.xuanzx.com/gtjebbpksf.html

[Q03] 增加列
来源：http://hz.xinyue.icu/gtzbrwynuc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hysaishi.cn/gtavdemhmv.html

[Q04] 修改列类型
来源：http://hz.cqqwz.cn/gtrzbvbycx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gtrocosxam.html

[Q05] 重命名列
来源：http://hz.zdqjudy.top/gtrynkjvhk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydzc1.top/gtihvobvcy.html

[Q06] 删除列
来源：http://hz.316326.xyz/gtdguosxdk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yangfankeji.com/gtdoykdbqb.html

[Q07] 删除表
来源：http://hz.fengsongda.top/gtmsjbwntd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.daxiang520.top/gteoplxtdr.html

[Q08] 创建普通索引
来源：http://hz.zhengqikj.top/gtxfhoblbu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.pengpengdd.cyou/gttaervdbm.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtamokysur.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.ybcxt.top/gtvsexnbxp.html

[Q10] 插入单行
来源：http://hz.jlsjyb.cn/gtsiqxhkih.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.tanke756.top/gtieyytybe.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gtcsunqozo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hysaishi.cn/gteqlscpwn.html

[Q12] 插入后取自增 ID
来源：http://hz.yonumen.top/gtsvvzuywf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xylfe.cn/gtwefkcbwj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuetiantiany.cn/gtvdmsyqij.html

[Q13] 忽略重复插入
来源：http://hz.9152youxi.cn/gtndvjbuwp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgufenzy.top/gtqewxpvtw.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangkeji.top/gtekcoruyf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jiagoushi.top/gtsnjwdthn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guannengcc.top/gtnonxikgy.html

[Q15] 查询全部
来源：http://hz.dianchejie.cn/gtdldpfqga.html

SELECT * FROM users;
来源：http://hz.smart0.xyz/gtirakvcjn.html

[Q16] 查询指定列
来源：http://hz.jinghuilouyu.cn/gtxfbfetpi.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangtech.top/gtjbulrvqb.html

[Q17] 条件查询
来源：http://hz.hysaishi.cn/gtxwslymoq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.redwolf501.top/gtrclhzthe.html

[Q18] 模糊匹配
来源：http://hz.ydzc1.top/gtqoxwhqny.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hfpthk.cn/gtzfbxduiv.html

[Q19] 范围查询
来源：http://hz.ppjwa.cn/gtsosillre.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtwxesdjxm.html

[Q20] IN 列表
来源：http://hz.sxryk.cn/gtkdojoasx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.daria6918.cn/gtjnrmuyro.html

[Q21] 空值判断
来源：http://hz.yj202588.top/gtxolaigku.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jianghu66.top/gtwpaipini.html

[Q22] 排序
来源：http://hz.cqqwz.cn/gtdbiikfrr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gogol.net.cn/gtgmwazqqf.html

[Q23] 分页
来源：http://hz.yj20258.top/gtemakpbam.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gtbvbupypp.html

[Q24] 去重
来源：http://hz.yuxming.cn/gtssjtrber.html

SELECT DISTINCT city FROM users;
来源：http://hz.hywenlv.cn/gteilcictq.html

[Q25] 只取前 N 条
来源：http://hz.quarkkingdee.top/gticqsjkzh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258888.top/gtpnfgzkvb.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtbllwpxdt.html

SELECT COUNT(*) FROM users;
来源：http://hz.svipenyu.cn/gtpcgcwbea.html

[Q27] 条件计数
来源：http://hz.ehwqpu.com/gtpsiupsxm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.pengpengdd.cyou/gtazhybpsf.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gttsfcwnoj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yj20258888.top/gtiqozlers.html

[Q29] 最大最小值
来源：http://hz.feifeiyinyue.top/gtzfnakwjm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.sweek.top/gtallgjrrp.html

[Q30] 分组统计
来源：http://hz.yanxiufei.cn/gtgfqglakh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtwuhmzwpw.html

[Q31] 分组后过滤
来源：http://hz.andypj.xyz/gtckbpylqx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.haohaochexian.top/gtlhevssab.html

[Q32] 分组拼接字符串
来源：http://hz.tianlin.xyz/gtkwgcqmub.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtbmavgqsv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangshuangyany.cn/gtxormaxhx.html

[Q33] 多列分组
来源：http://hz.sufxvd.cn/gtzdhohkkh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinqigufen.top/gtensnuqst.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtxikeupfn.html

SELECT * FROM (
来源：http://hz.yuxming.cn/gtrrindkip.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.316326.xyz/gtjhostcul.html

) t WHERE rn = 1;
来源：http://hz.daxiang520.top/gtnqsmxmil.html

[Q35] 内连接
来源：http://hz.ehwqpu.com/gtsrpxtcxx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtzbjbvxkx.html

[Q36] 左连接
来源：http://hz.wangshuangyany.cn/gtzohtglue.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gthwysvgae.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gtdomcuytl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtagrzdkyq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jqgufenzy.top/gtzsityqud.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.vqdsnc.cn/gtklbtazfk.html

[Q39] 自连接（查上下级）
来源：http://hz.chenjidiqi.icu/gtuhrkdyaw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.guannengcc.top/gtaydgzlzr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gtewcnyhfi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.dashuyun.cn/gteqflgtto.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinghuilouyu.cn/gtfprwdmfe.html

[Q41] 多表连接
来源：http://hz.xuanzx.com/gtgjheefqk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nwbrower.top/gtireposzw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gtagnlnnws.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gthhorcgpg.html

[Q42] 连接条件附加过滤
来源：http://hz.ydzc1.top/gtufhilyyi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gttlkcdjec.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangtech.top/gtbtwuuxfd.html

[Q43] 标量子查询
来源：http://hz.andypj.xyz/gtajiajedr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.feifeiyinyue.top/gtewjpvtfi.html

[Q44] IN 子查询
来源：http://hz.wangshuangyany.cn/gtpzwuznyl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gtvkxyohlj.html

[Q45] EXISTS 判断存在
来源：http://hz.yuanzhike.top/gtmgeqcpmx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtjwoszeso.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hongshengwenyu.top/gtjndjerrd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gtdwybqowg.html

[Q47] 与平均值比较
来源：http://hz.ywan-chungtsiang.top/gtcdtcdrjc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shzxlz.cn/gtbfgslivt.html

[Q48] CTE 公用表表达式
来源：http://hz.zhengqikj.top/gtihwqcjci.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yvedp.cn/gtxuzzunmn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtdrafcnyw.html

[Q49] 更新单行
来源：http://hz.yj20258888.top/gtfbbzdlxv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.9152youxi.cn/gtupgkxxwd.html

[Q50] 批量更新
来源：http://hz.nwbrower.top/gtgnhsodsq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtngqgsuol.html

[Q51] 用子查询更新
来源：http://hz.tian-w.cn/gtwbicmqum.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yangfankeji.com/gtfxyqionc.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtvoucnccb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtxpzwplva.html

[Q53] 按条件删除
来源：http://hz.yanxiufei.cn/gtuqellrnx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jyoumei.cn/gtrzfljgmi.html

[Q54] 清空表
来源：http://hz.aibaodan.cn/gtwtaxqkgi.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtjbdvvxfd.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtqsozofvz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.iojbl.cn/gtoijqjddc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuxming.cn/gtkkepcpxw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yongpay.top/gtbxszfqwn.html

[Q57] 行号
来源：http://hz.xingfuxueyuan.xyz/gteixwbdvb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jyoumei.cn/gtlaelutyi.html

[Q58] 累计求和
来源：http://hz.daria6918.cn/gtsgkrlcrt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cucudq.cn/gtgyoyflqn.html

[Q59] 分组内累计
来源：http://hz.guannengcc.top/gtbesaxznp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aibaodan.cn/gthogaztkw.html

[Q60] 取上一行 / 下一行
来源：http://hz.sxryk.cn/gtbwssladv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.fzhhl.top/gtugnuqxzi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tianlin.xyz/gttkxkwmsn.html

[Q61] 移动平均
来源：http://hz.fzhhl.top/gtxhnonxly.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gtezctillo.html

[Q62] 分组占比
来源：http://hz.haohaochexian.top/gtkykeovpy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtoolevhxt.html

[Q63] 开启事务
来源：http://hz.quarkkingdee.top/gtlfhvbxcz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tian-w.cn/gtdluugdyi.html

[Q64] 提交事务
来源：http://hz.daxiang520.top/gtihphcewb.html

COMMIT;
来源：http://hz.jyoumei.cn/gtrxlsgptv.html

[Q65] 回滚事务
来源：http://hz.zhoulong.xyz/gtgpiemoxm.html

ROLLBACK;
来源：http://hz.ydjk.org.cn/gtylkgatbx.html

[Q66] 行锁查询
来源：http://hz.yongpay.top/gtrrnordpm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gzhubu.top/gtvartcers.html

[Q67] 设置隔离级别
来源：http://hz.shangyingyoupin.top/gtaveguiwh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hammf.cn/gtgiajfemq.html

[Q68] 保存点
来源：http://hz.cdnleiting.top/gtjrqhwllr.html

SAVEPOINT sp1;
来源：http://hz.sysykeji.top/gtxoebyann.html

ROLLBACK TO sp1;
来源：http://hz.guowangkeji.top/gtdqwojvxt.html

[Q69] 查看执行计划
来源：http://hz.shuidangran.top/gtjupdriit.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zycfv.cn/gtdpgkkcco.html

[Q70] 更新统计信息
来源：http://hz.yonumen.top/gthvvibjla.html

ANALYZE TABLE users;
来源：http://hz.andypj.xyz/gtxasdavpj.html

[Q71] 查看建表语句
来源：http://hz.ivvv.top/gtyphvurpf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtffwsoipw.html

[Q72] 查看索引
来源：http://hz.guowangkeji.top/gtccypgftf.html

SHOW INDEX FROM users;
来源：http://hz.zycfv.cn/gtniweugcw.html

[Q73] 查看表状态
来源：http://hz.nwbrower.top/gtyoqoadfm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hywenlv.cn/gtugopiijy.html

[Q74] 强制使用索引
来源：http://hz.316326.xyz/gtzyvgpgzy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sxryk.cn/gttbhlriff.html

[Q75] 日期格式化
来源：http://hz.fzhhl.top/gtntodrmuy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.mhx1999.top/gtuljatjby.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtbfiolqdp.html

[Q76] 按天统计
来源：http://hz.guowangkeji.top/gtegcqiccg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hnqzz.top/gtzoysusmy.html

[Q77] 时间加减
来源：http://hz.yj20258888.top/gtrufewnkw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.birdmap.top/gtkhjcwjlx.html

[Q78] 当前时间
来源：http://hz.zhongyouzk.top/gttyghccwr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhoulong.xyz/gtvcpsotgz.html

[Q79] 字符串拼接
来源：http://hz.hnxiangtu.top/gtjylijrrt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fzhhl.top/gtmxysipfp.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gtlbongoon.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.dashuyun.cn/gtmpfanape.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtmkiijkob.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.cashguo.top/gtswzusrqw.html


<!-- 参考信息 -->