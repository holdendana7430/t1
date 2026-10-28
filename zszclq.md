代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuxming.cn/gtwaipdvtu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj202588.top/gtlmxtljoe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zdqjudy.top/gtahahtpqa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtqealoqtp.html

================================================================================
来源：http://hz.hnqzz.top/gtujyduylg.html

O. 并发与异步
来源：http://hz.52xcode.cn/gtygchkmss.html

================================================================================
来源：http://hz.tianlin.xyz/gtwugffolb.html

[O01] 启动一个线程
来源：http://hz.jiagoushi.top/gtkmepjwxh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.andypj.xyz/gtfjolijbc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtziwaaqhh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj202588.top/gtiiekymev.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gtridtfnwm.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhijiandao.cn/gtmaajymzu.html

Go:   go f()
来源：http://hz.cucudq.cn/gtnrmzcmxv.html

Ruby: Thread.new { f }
来源：http://hz.gzhubu.top/gtupgxmrpf.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gtasgvqubg.html

[O02] 使用线程池
来源：http://hz.yangfankeji.com/gtvhjhwqub.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xingfuxueyuan.xyz/gtnzgisuao.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtezzcfttv.html

JS:   // worker_threads 线程池
来源：http://hz.tian-w.cn/gtxjwusviz.html

TS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gteqyxiyvs.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xinyue.icu/gtrbioxuap.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shuidangran.top/gtzavhlbuq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jlsjyb.cn/gtnjzeouec.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gtjbvwkhiw.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtlepbmhcq.html

Py:   with lock: shared += 1
来源：http://hz.cdnleiting.top/gtvbguxxnz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtsexgpkgr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hfpthk.cn/gtvcczkdwb.html

TS:   // 同 JS
来源：http://hz.ybcxt.top/gttcykejfg.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtddngaxxz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtckddwsfw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yonumen.top/gtfbpafnqv.html

C#:   lock (gate) { shared++; }
来源：http://hz.jyoumei.cn/gtavrgppxq.html

[O04] 定义异步函数并等待
来源：http://hz.redwolf501.top/gthvnidtjn.html

Py:   async def f():⏎    await g()
来源：http://hz.hywenlv.cn/gtdmdqvuen.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtwwqowoav.html

JS:   async function f() { await g(); }
来源：http://hz.yongpay.top/gttuxfjhke.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gtbcrosneg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yangfankeji.com/gtjvphgyok.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gtczjbyvvk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sysykeji.top/gthsyudqec.html

C#:   async Task F() { await G(); }
来源：http://hz.chenjidiqi.icu/gthrkfocrz.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgufenzy.top/gtmvmjdpsw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gaohongyu789.top/gtstuayxzg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.svipenyu.cn/gtoovjwcmo.html

JS:   await Promise.all(tasks)
来源：http://hz.316326.xyz/gtwwdnxmsx.html

TS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtltjrwvwp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangtech.top/gtolgihfhn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ybcxt.top/gtezbryggd.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtxvinnqcb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtpgbltxrp.html

[O06] 使用进程池
来源：http://hz.yvedp.cn/gtsqypsqnt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangtech.top/gtkryfzshq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhengqikj.top/gteeouvenf.html

JS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtqeddgqez.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtggksfwpl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.fengsongda.top/gtmjstrzvw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenjidiqi.icu/gtsudqqghf.html

Ruby: // fork 块
来源：http://hz.jinyuanbaomall.cn/gtierevavn.html

C#:   Parallel.For
来源：http://hz.dashuyun.cn/gtyxjqztsc.html

================================================================================
来源：http://hz.sufxvd.cn/gtgrzsvkft.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtdqwbcctj.html

================================================================================
来源：http://hz.cdnleiting.top/gtdsifaqwh.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gtisfhigjs.html

Py:   str(uuid.uuid4())
来源：http://hz.xinyue.icu/gtawhxeaie.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtzdimvoqa.html

JS:   crypto.randomUUID()
来源：http://hz.meibo888.top/gtpobppaoc.html

TS:   crypto.randomUUID()
来源：http://hz.daxiang520.top/gtppxpgjtd.html

Java: UUID.randomUUID().toString()
来源：http://hz.hywenlv.cn/gtdqoeccek.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gtmolysgdl.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtpecmcjfb.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhongyouzk.top/gtkbrpycmm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hysaishi.cn/gtadwunxoy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xingfuxueyuan.xyz/gtbwiyyods.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yueranfly.top/gtvidrpdeb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gtesnphbfc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gtuugcguiw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jlsjyb.cn/gtbhsevxhj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtyhpdozvr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sxryk.cn/gtqeqcqojc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnxiangtu.top/gtkulspabn.html

[P03] 生成短随机字符串
来源：http://hz.quarkkingdee.top/gtomopqnro.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xziqi.cn/gtjiiwtiir.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangkeji.top/gtsfzhnxxy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtwbsiwnnn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtivpifopu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.feifeiyinyue.top/gtznnsohfq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sysykeji.top/gtvswwrbou.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nwbrower.top/gtenfthfcl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.sweek.top/gtsjsafhcb.html

[P04] 求长度
来源：http://hz.jianghu66.top/gtgjlahgvs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yj20258888.top/gtrmlfwxvl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtlptsihym.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.aibaodan.cn/gtdavgdjgz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shangyingyoupin.top/gtquoyrhhz.html

Java: list.size();  map.size();  s.length()
来源：http://hz.mhx1999.top/gtagfheqgb.html

Go:   len(arr);  len(m)
来源：http://hz.tian-w.cn/gtgchnyxfr.html

Ruby: x.length;  x.size
来源：http://hz.yueranfly.top/gtwxfbyrhl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.fzhhl.top/gtdqtbovcx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.mhx1999.top/gtqmvdaxsa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cqqwz.cn/gtcpmqhlbp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hnxiangtu.top/gttnvwoadk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtulpgcqof.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtcduzkgmh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hysaishi.cn/gttddjblmd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xinyue.icu/gtwhfxtvzv.html

Ruby: a == b
来源：http://hz.wangdashe.top/gtupewcrrq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj202588.top/gtqlzpnwmt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhixingplan.top/gtzbxyokgy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.daria6918.cn/gtooaorryb.html

PHP:  if (empty($x)) {}
来源：http://hz.ppjwa.cn/gtjydfduqa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.kuanghao11.cn/gtfpmsywfs.html

TS:   if (x == null) {}
来源：http://hz.chenlongwang.top/gtlsiycgbt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtwjeplfhn.html

Go:   if x == nil {}
来源：http://hz.cheryme.top/gtrysjxwst.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.52xcode.cn/gtjqxfghfr.html

C#:   if (x is null) {}
来源：http://hz.hnqzz.top/gtrwmvinod.html

[P07] 防抖与节流
来源：http://hz.cashguo.top/gtlesyymen.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jianghu66.top/gtgtjvrqsv.html

PHP:  // 手写时间戳比较
来源：http://hz.shzxlz.cn/gtitnohjlf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.chenjidiqi.icu/gtkezulmbp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtudocjkbx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtpkkerzik.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cdnleiting.top/gtolpzblzv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jlsjyb.cn/gtfraprgjy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhixingplan.top/gtbftgrbir.html

[P08] 处理浮点精度问题
来源：http://hz.sxryk.cn/gtiqnlqlya.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.snrcjt.cn/gtsraonrhi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.aizwys.cn/gtudohdhtd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gtogzkqtny.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgfzy.top/gtqcmgaxoz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.316326.xyz/gtqlqbrcuw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.dianchejie.cn/gtfvbgnxzh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shuidangran.top/gtlkmymlae.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgufenzy.top/gtjzyfnfet.html

================================================================================
来源：http://hz.chenlongwang.top/gtponsaraa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gtdeiypkrj.html

================================================================================
来源：http://hz.xuanzx.com/gtdjsulngr.html

[Q01] 创建表
来源：http://hz.yj20258.top/gtolwwotps.html

CREATE TABLE users (
来源：http://hz.cdnleiting.top/gtpgzkhmuf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtcvsjganj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shangyingyoupin.top/gtszlaafuv.html

email VARCHAR(100) UNIQUE,
来源：http://hz.guowangkeji.top/gtnejufrcv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sufxvd.cn/gtzskkygtb.html

);
来源：http://hz.smart0.xyz/gtfsaxtopy.html

[Q02] 创建带外键的表
来源：http://hz.jianghu66.top/gtwvaqdrsx.html

CREATE TABLE orders (
来源：http://hz.ivvv.top/gtfkcmeopa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtieazaivj.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtwxqfsykp.html

amount DECIMAL(10, 2),
来源：http://hz.gogol.net.cn/gtpfepvlfu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhoulong.xyz/gtkhgwwqaq.html

);
来源：http://hz.cqqwz.cn/gtbkfbojsr.html

[Q03] 增加列
来源：http://hz.hnqzz.top/gtgriixvjm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.smart0.xyz/gthptlvrwr.html

[Q04] 修改列类型
来源：http://hz.sufxvd.cn/gtznqilrws.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtugfjtefj.html

[Q05] 重命名列
来源：http://hz.jlsjyb.cn/gtebxyrtdm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.kuanghao11.cn/gtqxfhunio.html

[Q06] 删除列
来源：http://hz.quarkkingdee.top/gtosxxfgki.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtddycyynp.html

[Q07] 删除表
来源：http://hz.cdnleiting.top/gtwtmwqgtg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtlctltjro.html

[Q08] 创建普通索引
来源：http://hz.snrcjt.cn/gtknssrtfk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.havefunace.top/gtuljxhffu.html

[Q09] 创建唯一索引
来源：http://hz.yj20258888.top/gtsjdvhpuk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtsiqrcyia.html

[Q10] 插入单行
来源：http://hz.kuanghao11.cn/gtfddheksa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.daria6918.cn/gtqbqswcfe.html

[Q11] 一次插入多行
来源：http://hz.fengsongda.top/gtammeucce.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ehwqpu.com/gthdkgzcbt.html

[Q12] 插入后取自增 ID
来源：http://hz.yuanzhike.top/gtydibipyn.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.svipenyu.cn/gtmjkxibey.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenjidiqi.icu/gtdnftfpry.html

[Q13] 忽略重复插入
来源：http://hz.yueranfly.top/gtlhwzbbyl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtecgpukyv.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtzdvfrgda.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shangyingyoupin.top/gtqueiiedu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangkeji.top/gtsgzwoyml.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtwzybinmd.html

SELECT * FROM users;
来源：http://hz.ydjk.org.cn/gttnndbqsw.html

[Q16] 查询指定列
来源：http://hz.zdqjudy.top/gtaqxyfgfw.html

SELECT id, name FROM users;
来源：http://hz.zhoulong.xyz/gtyxpwebqk.html

[Q17] 条件查询
来源：http://hz.cucudq.cn/gthcpgfiew.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ywan-chungtsiang.top/gtxtoobqbr.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gtkqefhxcc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangtech.top/gtfquxvzlc.html

[Q19] 范围查询
来源：http://hz.guannengcc.top/gtakvpcegc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258888.top/gtjnttrknl.html

[Q20] IN 列表
来源：http://hz.tian-w.cn/gtdhgohskk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhongyouzk.top/gtngmlowgw.html

[Q21] 空值判断
来源：http://hz.zdqjudy.top/gtayiwwcir.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.haohaochexian.top/gtgkznyald.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtucmaijtz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shangyingyoupin.top/gtalkbobhb.html

[Q23] 分页
来源：http://hz.yj202588.top/gtmdbrzehx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhaomingkeji.xyz/gtwuyrpsld.html

[Q24] 去重
来源：http://hz.wangshuangyany.cn/gtfpvpjvar.html

SELECT DISTINCT city FROM users;
来源：http://hz.ehwqpu.com/gtlkqmqmce.html

[Q25] 只取前 N 条
来源：http://hz.yj202588.top/gtcnqgodsm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gttkzaxnfh.html

[Q26] 计数
来源：http://hz.guannengcc.top/gtqiiwvzmd.html

SELECT COUNT(*) FROM users;
来源：http://hz.jyoumei.cn/gtuxktimiy.html

[Q27] 条件计数
来源：http://hz.zdqjudy.top/gtmjskjdsc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhengqikj.top/gtimeobdrq.html

[Q28] 求和与平均
来源：http://hz.zdqjudy.top/gtxuhqjojf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jianghu66.top/gtdwxhlgoa.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gttslcuepk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pengpengdd.cyou/gtphxnyzoc.html

[Q30] 分组统计
来源：http://hz.jqgufenzy.top/gtkejdoohl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtmmfoidvk.html

[Q31] 分组后过滤
来源：http://hz.feifeiyinyue.top/gtbhbzrhqb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnqzz.top/gtfjuuxnkw.html

[Q32] 分组拼接字符串
来源：http://hz.hfpthk.cn/gthuvoiagk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtotrulwak.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dianchejie.cn/gtfdomacyd.html

[Q33] 多列分组
来源：http://hz.hongshengwenyu.top/gthtdtdgau.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenzaomai.com/gtvbsmixaw.html

[Q34] 每组取第一条
来源：http://hz.smart0.xyz/gtmjaphlep.html

SELECT * FROM (
来源：http://hz.jqgfzy.top/gtljkqnftx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hongshengwenyu.top/gtanjlwcuq.html

) t WHERE rn = 1;
来源：http://hz.kuanghao11.cn/gtnfdfyjmm.html

[Q35] 内连接
来源：http://hz.jlsjyb.cn/gtvziitmlz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtzrzuqiks.html

[Q36] 左连接
来源：http://hz.gzhubu.top/gtzoikhiuv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtowhlvssy.html

[Q37] 右连接
来源：http://hz.jinqigufen.top/gtsfubebum.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxuanxn.top/gtwwqfataa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhaomingkeji.xyz/gthbjoroey.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinyuanbaomall.cn/gtmcpmsrhh.html

[Q39] 自连接（查上下级）
来源：http://hz.9152youxi.cn/gtilbktvnh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.pengpengdd.cyou/gtsdkxiiag.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yj20258888.top/gtebctdkom.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yanxiufei.cn/gtbbryruew.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydjk.org.cn/gtgobkkeql.html

[Q41] 多表连接
来源：http://hz.mhx1999.top/gtpkuqwteq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.snrcjt.cn/gtthvvhnwz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.fengsongda.top/gtfrtiljss.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtovcszdzb.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtvreelwxh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigfzy.top/gtlomkyahy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pengpengdd.cyou/gttdimupos.html

[Q43] 标量子查询
来源：http://hz.yangfankeji.com/gthgexcxsa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gtainpoisz.html

[Q44] IN 子查询
来源：http://hz.ywan-chungtsiang.top/gtixyjamuh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zycfv.cn/gtshfheoub.html

[Q45] EXISTS 判断存在
来源：http://hz.yanxiufei.cn/gtvelqftuw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shzxlz.cn/gtlumvdaib.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hywenlv.cn/gtmzcdbdhv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtnywisyfp.html

[Q47] 与平均值比较
来源：http://hz.tanke756.top/gtdvypifbl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.9152youxi.cn/gtuzrujaqt.html

[Q48] CTE 公用表表达式
来源：http://hz.52xcode.cn/gtnwbfekgf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.c1oappe.top/gttqqtrtvo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinghuilouyu.cn/gtrlbypnga.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gttsypjsus.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yangfankeji.com/gtblaqapvv.html

[Q50] 批量更新
来源：http://hz.nanxuanxn.top/gtcxbmwbrx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gtjkljgjqf.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gtlsdwdgmi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinyuanbaomall.cn/gtfkbmviks.html

[Q52] 删除指定行
来源：http://hz.52xcode.cn/gtchlqetlm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.0kj1m.cn/gttsjjjhmw.html

[Q53] 按条件删除
来源：http://hz.yuanzhike.top/gtnrmhuzgg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.0kj1m.cn/gtmfrhtzji.html

[Q54] 清空表
来源：http://hz.zhengqikj.top/gtzyarkabv.html

TRUNCATE TABLE logs;
来源：http://hz.smart0.xyz/gtegxvhmym.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtuaaeuywm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuetiantiany.cn/gtmdggcuwv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.pengpengdd.cyou/gtumtxajsb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtisioswrt.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtllkdvhje.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yongpay.top/gtujtcypck.html

[Q58] 累计求和
来源：http://hz.tianlin.xyz/gtedlelvno.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtlumsmpxp.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gtbhksnlqc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtkdkigaoc.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangdashe.top/gtalbfafcb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydzc1.top/gtoexhyjpj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cashguo.top/gtixvcqwnx.html

[Q61] 移动平均
来源：http://hz.tanke756.top/gtpgawwmxt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtzpbvivar.html

[Q62] 分组占比
来源：http://hz.yvedp.cn/gtclzzsztb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtvuemkgad.html

[Q63] 开启事务
来源：http://hz.svipenyu.cn/gtoifjfvlf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fzhhl.top/gtnmevoeid.html

[Q64] 提交事务
来源：http://hz.jlsjyb.cn/gttrgkqltk.html

COMMIT;
来源：http://hz.hywenlv.cn/gtelpsrgcm.html

[Q65] 回滚事务
来源：http://hz.chenlongwang.top/gtmrytfvuh.html

ROLLBACK;
来源：http://hz.ppjwa.cn/gtpaxthqne.html

[Q66] 行锁查询
来源：http://hz.mhx1999.top/gthbxffoai.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gtsfpquvyn.html

[Q67] 设置隔离级别
来源：http://hz.316326.xyz/gthqeyhoje.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxinkj.top/gtsspmhuog.html

[Q68] 保存点
来源：http://hz.redwolf501.top/gthgupzpet.html

SAVEPOINT sp1;
来源：http://hz.ehwqpu.com/gtexvjgitu.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gtajcbscep.html

[Q69] 查看执行计划
来源：http://hz.hammf.cn/gtvzjclsse.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtqaarejgp.html

[Q70] 更新统计信息
来源：http://hz.andypj.xyz/gtumbcxjgm.html


<!-- 参考信息 -->