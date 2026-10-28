代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://hz.hnqzz.top/gtbquwpwmp.html

Go:   go f()
来源：http://hz.yonumen.top/gtxckxgtwe.html

Ruby: Thread.new { f }
来源：http://hz.yj20258888.top/gtiigissqq.html

C#:   Task.Run(() => F());
来源：http://hz.jinghuilouyu.cn/gtuujtketi.html

[O02] 使用线程池
来源：http://hz.zhixingplan.top/gtanwctpge.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daria6918.cn/gtoeueamvt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtbjwcnshw.html

JS:   // worker_threads 线程池
来源：http://hz.hywenlv.cn/gtsbfnwfck.html

TS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtiebawyub.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhongyouzk.top/gtkdgggfmf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhixingplan.top/gthflogmgu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj202588.top/gtpxvykjqb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinghuilouyu.cn/gtgxgpkrnm.html

[O03] 加锁保护共享数据
来源：http://hz.yuanzhike.top/gtbdifcvfv.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtkmzkovnd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtodbmrcym.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.shanyushiyangkeji.top/gtwubfruqd.html

TS:   // 同 JS
来源：http://hz.cheryme.top/gtjcfvkixf.html

Java: synchronized (this) { shared++; }
来源：http://hz.ehwqpu.com/gtetxjwtnf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xuanzx.com/gttdyiwzyr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nwbrower.top/gtertwlmrp.html

C#:   lock (gate) { shared++; }
来源：http://hz.ppjwa.cn/gtnrfzjhyf.html

[O04] 定义异步函数并等待
来源：http://hz.tanke756.top/gthtrwilkg.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gtghlnjthc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dashuyun.cn/gtyrffebeu.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gtflndrhei.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnxiangtu.top/gtwebymesp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sweek.top/gtlsvgehwn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.52xcode.cn/gtkbgbcrxy.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.52xcode.cn/gtgkfdxnqp.html

C#:   async Task F() { await G(); }
来源：http://hz.cdnleiting.top/gtxmakhvrh.html

[O05] 并发执行并等待全部完成
来源：http://hz.havefunace.top/gtmxsojygu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtzmjygzvb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangkeji.top/gtarvdcyzs.html

JS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtjqkqcvve.html

TS:   await Promise.all(tasks)
来源：http://hz.hywenlv.cn/gtkgteswqm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.quarkkingdee.top/gtiwlbzdvv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.9152youxi.cn/gtwaksgkpr.html

Ruby: threads.map(&:join)
来源：http://hz.pycfn.com/gtffpnltix.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhijiandao.cn/gtxwymeyee.html

[O06] 使用进程池
来源：http://hz.yangfankeji.com/gtocpsjbrd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jianghu66.top/gtjexjpbhq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.kuanghao11.cn/gtbgbrnvlh.html

JS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtzrwikoyr.html

TS:   // child_process / cluster 模块
来源：http://hz.yanxiufei.cn/gtzzevtwyl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zdqjudy.top/gtiicflyuo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtcjaaower.html

Ruby: // fork 块
来源：http://hz.hnqzz.top/gttjibgxvw.html

C#:   Parallel.For
来源：http://hz.xingfuxueyuan.xyz/gtxpgjlqra.html

================================================================================
来源：http://hz.shzxlz.cn/gthnwinfyg.html

P. 常用工具函数
来源：http://hz.xziqi.cn/gtwzzqzjww.html

================================================================================
来源：http://hz.nanxinkj.top/gtmheaddhr.html

[P01] 生成 UUID
来源：http://hz.316326.xyz/gtqkwcxnej.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtpxcatalk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aibaodan.cn/gtalqyzbyc.html

JS:   crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtzxqqhtnm.html

TS:   crypto.randomUUID()
来源：http://hz.ydzc1.top/gtbhvngrjk.html

Java: UUID.randomUUID().toString()
来源：http://hz.xylfe.cn/gtxrtsxvpg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.9152youxi.cn/gtcdmmhvis.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258.top/gtearjfhmp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhijiandao.cn/gtlywwmsbs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cucudq.cn/gtlcaabuqy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.316326.xyz/gtttrkznee.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aibaodan.cn/gtfdoeycet.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guannengcc.top/gtsyzcowto.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ppjwa.cn/gtzrtvrezk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hfpthk.cn/gtmvhakchu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.316326.xyz/gtjwfekexw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yueranfly.top/gtvulntnhq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnqzz.top/gtuqlhxpia.html

[P03] 生成短随机字符串
来源：http://hz.zhengqikj.top/gtycyejoqy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yuxming.cn/gtsxjnfyss.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.52xcode.cn/gtffyiwczr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zycfv.cn/gturqmdils.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gtrkiqqswe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hysaishi.cn/gtksdzwdtj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shuidangran.top/gtyapofhwc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.iojbl.cn/gtznxsfnba.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gthzdhydii.html

[P04] 求长度
来源：http://hz.ivvv.top/gtmtwlwkfz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhengqikj.top/gtgheabqhn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtcrqadppp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtnoswsfvl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtrjwdkujc.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gaohongyu789.top/gtmxrnzbme.html

Go:   len(arr);  len(m)
来源：http://hz.guowangkeji.top/gtzjtixwlb.html

Ruby: x.length;  x.size
来源：http://hz.smart0.xyz/gtuofcwjzd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhengqikj.top/gtzmpiewki.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gtuingolcq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ywan-chungtsiang.top/gtnogsflqv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tian-w.cn/gtpxncttpz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.kuanghao11.cn/gtyodvvleg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hammf.cn/gtwtpjrtqe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.vqdsnc.cn/gtjslpnrsn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.nanxuanxn.top/gtsjmqnjtb.html

Ruby: a == b
来源：http://hz.wangdashe.top/gtyqrsxmfv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ppjwa.cn/gtqoipltsw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.quarkkingdee.top/gtnrtyobdk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cashguo.top/gtwwlehtzg.html

PHP:  if (empty($x)) {}
来源：http://hz.guowangkeji.top/gttmtlsikb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.svipenyu.cn/gtqpdvvjok.html

TS:   if (x == null) {}
来源：http://hz.kuanghao11.cn/gtgdvwjqeo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtatqcehio.html

Go:   if x == nil {}
来源：http://hz.shzxlz.cn/gtxkaovhrb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.quarkkingdee.top/gtanknfbca.html

C#:   if (x is null) {}
来源：http://hz.feifeiyinyue.top/gtkvlllbbf.html

[P07] 防抖与节流
来源：http://hz.snrcjt.cn/gtcnknfkir.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xuetiantiany.cn/gteumkukut.html

PHP:  // 手写时间戳比较
来源：http://hz.yanxiufei.cn/gthrrztqqt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuanzhike.top/gtmcfynbqq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.meibo888.top/gtndjnqznl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ybcxt.top/gtomtuvecq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gtnknovqbc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.nwbrower.top/gtuwmhiukf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgufenzy.top/gtpmrpwrop.html

[P08] 处理浮点精度问题
来源：http://hz.fzhhl.top/gthhgqgzrt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydjk.org.cn/gtoqjezxhx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xingfuxueyuan.xyz/gtkouibsap.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cheryme.top/gtpngoafio.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.daxiang520.top/gtaajfivog.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenjidiqi.icu/gtpadobsum.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dashuyun.cn/gtznbiqtww.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258.top/gtplddblqc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cdnleiting.top/gtqmvbmypa.html

================================================================================
来源：http://hz.cdnleiting.top/gthujohhni.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.daria6918.cn/gtubcrzsxl.html

================================================================================
来源：http://hz.tianlin.xyz/gtwrgflgzn.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gttfpycdwi.html

CREATE TABLE users (
来源：http://hz.xingfuxueyuan.xyz/gtxwkmmvll.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtvccbgpnx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangdashe.top/gtmtdjypqh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.fengsongda.top/gtcoqquvxm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yonumen.top/gtzieprtok.html

);
来源：http://hz.yueranfly.top/gtnrehlfnn.html

[Q02] 创建带外键的表
来源：http://hz.cashguo.top/gtxjjkywdi.html

CREATE TABLE orders (
来源：http://hz.jinqigufen.top/gthsgozofz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhijiandao.cn/gtgulsjbrl.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtdkftyvni.html

amount DECIMAL(10, 2),
来源：http://hz.dashuyun.cn/gtcdulxvmw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhengqikj.top/gtxgzulkkr.html

);
来源：http://hz.xylfe.cn/gtsynrmjww.html

[Q03] 增加列
来源：http://hz.sxryk.cn/gtwfvowjbd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.kuanghao11.cn/gttvpucfmh.html

[Q04] 修改列类型
来源：http://hz.tanke756.top/gtxpfajugh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yj20258.top/gttafhrqcq.html

[Q05] 重命名列
来源：http://hz.chenlongwang.top/gtwpyjxaqy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gthinrfndr.html

[Q06] 删除列
来源：http://hz.wangshuangyany.cn/gtzwernfnk.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sufxvd.cn/gtrrpeejkr.html

[Q07] 删除表
来源：http://hz.zhengqikj.top/gtenhpvjoe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yonumen.top/gtqokhdsfw.html

[Q08] 创建普通索引
来源：http://hz.gotoacloud.top/gtkboebfbt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.wangdashe.top/gtjicpzwwq.html

[Q09] 创建唯一索引
来源：http://hz.zdqjudy.top/gtsepqgaqw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yongpay.top/gtyxjmgvfw.html

[Q10] 插入单行
来源：http://hz.feifeiyinyue.top/gtnjdrqegf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shuidangran.top/gtecomhdnx.html

[Q11] 一次插入多行
来源：http://hz.pycfn.com/gtrvawipvu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtvoqojbyw.html

[Q12] 插入后取自增 ID
来源：http://hz.fzhhl.top/gtaxloemtd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gtjjvsdidj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtanmarcis.html

[Q13] 忽略重复插入
来源：http://hz.jinyuanbaomall.cn/gtcepihkbt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinyuanbaomall.cn/gtxkqqtvpc.html

[Q14] 存在则更新（upsert）
来源：http://hz.tianlin.xyz/gtottpcaqv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.sxryk.cn/gtbbeppchd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zdqjudy.top/gtxumtusjk.html

[Q15] 查询全部
来源：http://hz.jinqigfzy.top/gtcfqpbexu.html

SELECT * FROM users;
来源：http://hz.redwolf501.top/gtvkcmbirb.html

[Q16] 查询指定列
来源：http://hz.ybcxt.top/gtvizbklix.html

SELECT id, name FROM users;
来源：http://hz.tianlin.xyz/gtlrqwdxkc.html

[Q17] 条件查询
来源：http://hz.yonumen.top/gtlpwvkdlw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.52xcode.cn/gtqflavexn.html

[Q18] 模糊匹配
来源：http://hz.havefunace.top/gtdmipqugl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cucudq.cn/gtmutlxpxz.html

[Q19] 范围查询
来源：http://hz.quarkkingdee.top/gtwuyquqzg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xuanzx.com/gtygtnrjeo.html

[Q20] IN 列表
来源：http://hz.ydjk.org.cn/gtlvxrgvco.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.jianghu66.top/gtwbfowtxg.html

[Q21] 空值判断
来源：http://hz.zycfv.cn/gtklrjcuhp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gtdskptbnj.html

[Q22] 排序
来源：http://hz.zhijiandao.cn/gtajbxiacq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydzc1.top/gtovbzxxrb.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtaiwippdp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinyuanbaomall.cn/gtnmlpyfua.html

[Q24] 去重
来源：http://hz.jyoumei.cn/gtrvzivelr.html

SELECT DISTINCT city FROM users;
来源：http://hz.hongshengwenyu.top/gtbkyzzrqs.html

[Q25] 只取前 N 条
来源：http://hz.ybcxt.top/gtueelxujo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jyoumei.cn/gtixlhfdac.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtbenjybup.html

SELECT COUNT(*) FROM users;
来源：http://hz.shzxlz.cn/gtakjrtowi.html

[Q27] 条件计数
来源：http://hz.xuetiantiany.cn/gtuwwhufni.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xziqi.cn/gtmoctelgp.html

[Q28] 求和与平均
来源：http://hz.jianghu66.top/gthkgyzesh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.hfpthk.cn/gterxlpjut.html

[Q29] 最大最小值
来源：http://hz.52xcode.cn/gtuwkweqyh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.nanxuanxn.top/gtxtjnrexb.html

[Q30] 分组统计
来源：http://hz.vqdsnc.cn/gtayzbewrj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtcpnckeer.html

[Q31] 分组后过滤
来源：http://hz.tianlin.xyz/gtydalnnqc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhiwuduotai.top/gtcwrsbgiu.html

[Q32] 分组拼接字符串
来源：http://hz.316326.xyz/gtrojuzgxt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtseewwunr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtsuldlsjm.html

[Q33] 多列分组
来源：http://hz.c1oappe.top/gtnkwvhmua.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtbbvhmglz.html

[Q34] 每组取第一条
来源：http://hz.yanxiufei.cn/gtdfgqysrc.html

SELECT * FROM (
来源：http://hz.ydjk.org.cn/gtevsooijz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj20258888.top/gtxkuvfnvw.html

) t WHERE rn = 1;
来源：http://hz.jinghuilouyu.cn/gtvjzrglyq.html

[Q35] 内连接
来源：http://hz.zhiwuduotai.top/gtzxgtqvzm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtjmhweqjc.html

[Q36] 左连接
来源：http://hz.hnxiangtu.top/gtxniycdfr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtzpyjfuri.html

[Q37] 右连接
来源：http://hz.wangshuangyany.cn/gtojmffajf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.daria6918.cn/gtnebmkhll.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jinyuanbaomall.cn/gtxvqnktbh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhixingplan.top/gtkqiornzn.html

[Q39] 自连接（查上下级）
来源：http://hz.zhaomingkeji.xyz/gtvkicrmjo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ivvv.top/gthfpjcerl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtoimzupjn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.haohaochexian.top/gtadkacgjd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dashuyun.cn/gthkiswtjk.html

[Q41] 多表连接
来源：http://hz.pengpengdd.cyou/gtntaeniuh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.andypj.xyz/gtwgkxutlh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.sxryk.cn/gttitpxmgz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtihcyjpav.html

[Q42] 连接条件附加过滤
来源：http://hz.kuanghao11.cn/gtcwcjbveh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hysaishi.cn/gtthibywmn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.chenjidiqi.icu/gtnaezlklc.html

[Q43] 标量子查询
来源：http://hz.yongpay.top/gtvlqavlhw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgfzy.top/gtogtunuvl.html

[Q44] IN 子查询
来源：http://hz.jqgufenzy.top/gthjqmwkrl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.sweek.top/gtjtnbbbxi.html

[Q45] EXISTS 判断存在
来源：http://hz.tianlin.xyz/gtjzjchilq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnqzz.top/gtbqubcaht.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cucudq.cn/gttsiayadq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtxtxwexji.html

[Q47] 与平均值比较
来源：http://hz.fzhhl.top/gtweytzwxx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtdzkakait.html

[Q48] CTE 公用表表达式
来源：http://hz.fzhhl.top/gthajkrhtm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tianlin.xyz/gtwwemrzyb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guowangkeji.top/gtdpmlqyog.html

[Q49] 更新单行
来源：http://hz.tianlin.xyz/gtsjsijthu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.52xcode.cn/gtnstcolpe.html

[Q50] 批量更新
来源：http://hz.feifeiyinyue.top/gtwhggfghr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.pengpengdd.cyou/gtorjihhkb.html

[Q51] 用子查询更新
来源：http://hz.tanke756.top/gtqghutwfh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ydzc1.top/gtspcsbutb.html

[Q52] 删除指定行
来源：http://hz.hywenlv.cn/gtdxevihgk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.316326.xyz/gtajpotdhj.html

[Q53] 按条件删除
来源：http://hz.ybcxt.top/gtrtouclhd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yonumen.top/gtnctavkeo.html

[Q54] 清空表
来源：http://hz.zhaomingkeji.xyz/gtqpjrsmiq.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gtjhjuodtk.html

[Q55] 排名（并列占位）
来源：http://hz.fzhhl.top/gtyencvono.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.chenzaomai.com/gtslsshwez.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yongpay.top/gtpavfnhac.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gtcakukqmd.html

[Q57] 行号
来源：http://hz.tian-w.cn/gtqzwnqime.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.kuanghao11.cn/gtrwcshkcy.html

[Q58] 累计求和
来源：http://hz.pycfn.com/gtxkblyprn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fzhhl.top/gturifbvds.html

[Q59] 分组内累计
来源：http://hz.jianghu66.top/gtgwvqbewa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dashuyun.cn/gtgekbidbo.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gtrnxzpucu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.dashuyun.cn/gtndibkejg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fzhhl.top/gtapxurilh.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtysvveuzj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shzxlz.cn/gtknuncgnx.html

[Q62] 分组占比
来源：http://hz.jqgufenzy.top/gtilovlfpl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtvtubvslx.html

[Q63] 开启事务
来源：http://hz.hammf.cn/gtbgwrnzyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.iojbl.cn/gtwvzvjoaj.html

[Q64] 提交事务
来源：http://hz.snrcjt.cn/gtlhdkkygy.html

COMMIT;
来源：http://hz.cucudq.cn/gtrvqhmvlf.html

[Q65] 回滚事务
来源：http://hz.sxryk.cn/gtybmzykjm.html

ROLLBACK;
来源：http://hz.aizwys.cn/gteiflxzwy.html

[Q66] 行锁查询
来源：http://hz.smart0.xyz/gtyljqrlcb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.birdmap.top/gtycoxhyhb.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtslsiuzky.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zdqjudy.top/gtukpqjjrm.html

[Q68] 保存点
来源：http://hz.xziqi.cn/gtebsllqjr.html

SAVEPOINT sp1;
来源：http://hz.c1oappe.top/gtagwetcji.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtxbaytvrc.html

[Q69] 查看执行计划
来源：http://hz.gzhubu.top/gtlarhrnsi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnxiangtu.top/gtbzbqhhik.html

[Q70] 更新统计信息
来源：http://hz.0kj1m.cn/gtcpnlraia.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtazwwnxpl.html

[Q71] 查看建表语句
来源：http://hz.nanxuanxn.top/gtdikuskyi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhoulong.xyz/gtdjwvjmeb.html

[Q72] 查看索引
来源：http://hz.ybcxt.top/gtexrxfxyr.html

SHOW INDEX FROM users;
来源：http://hz.yangfankeji.com/gtcrgcvhhe.html

[Q73] 查看表状态
来源：http://hz.yonumen.top/gtarssjctg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gtgomozxxi.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gtxjoxdili.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tianlin.xyz/gthmroghls.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gttotbxjxc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtxfnavbbp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.redwolf501.top/gtbduevhaz.html


<!-- 参考信息 -->