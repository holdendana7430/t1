代发 wailian999

TS:   // worker_threads 线程池
来源：http://hz.shangyingyoupin.top/gtcizapzpo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.feifeiyinyue.top/gtlrivbrfy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhijiandao.cn/gtwikcanmw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtojgrqjxx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258.top/gtcsqzpvnb.html

[O03] 加锁保护共享数据
来源：http://hz.yongpay.top/gtkbtudann.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gtvggtynkg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jiagoushi.top/gtznxvhyju.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.wangdashe.top/gtmnhdeajk.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtxojjarci.html

Java: synchronized (this) { shared++; }
来源：http://hz.hammf.cn/gtdpynfjfp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daria6918.cn/gtfwljjgub.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtuarhxodg.html

C#:   lock (gate) { shared++; }
来源：http://hz.9152youxi.cn/gtqdndtwxh.html

[O04] 定义异步函数并等待
来源：http://hz.nwbrower.top/gtbmxxhzey.html

Py:   async def f():⏎    await g()
来源：http://hz.yvedp.cn/gtglohrauw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.meibo888.top/gtzvkwdezy.html

JS:   async function f() { await g(); }
来源：http://hz.andypj.xyz/gtuzcjfxka.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.meibo888.top/gtslhwbyfe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnqzz.top/gtxjtsqftb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yangfankeji.com/gtznvryiiz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.iojbl.cn/gttbcwepdj.html

C#:   async Task F() { await G(); }
来源：http://hz.shzxlz.cn/gtrpqpzatn.html

[O05] 并发执行并等待全部完成
来源：http://hz.jqgfzy.top/gtxrcsommf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jianghu66.top/gtbwchhagt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cashguo.top/gteiyojmwz.html

JS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtueufilgy.html

TS:   await Promise.all(tasks)
来源：http://hz.gotoacloud.top/gtrtsdpdju.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangtech.top/gtzcoeloim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jiagoushi.top/gtpotzlcds.html

Ruby: threads.map(&:join)
来源：http://hz.haohaochexian.top/gtjhyklduo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fengsongda.top/gtiuhmuhvv.html

[O06] 使用进程池
来源：http://hz.nanxuanxn.top/gtcysfrizc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhoulong.xyz/gtduuvrvyg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxuanxn.top/gtrjsiicex.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgufenzy.top/gtefqzrfra.html

TS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gtasadikcu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.bjfxy.top/gtvfeiywtv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hysaishi.cn/gtzgkufglt.html

Ruby: // fork 块
来源：http://hz.pengpengdd.cyou/gtvzmglrmf.html

C#:   Parallel.For
来源：http://hz.xuanzx.com/gttxbrxcko.html

================================================================================
来源：http://hz.yj20258.top/gtsyjcfhdc.html

P. 常用工具函数
来源：http://hz.cashguo.top/gtiqkwxhxi.html

================================================================================
来源：http://hz.yuanzhike.top/gtldozdbvs.html

[P01] 生成 UUID
来源：http://hz.pengpengdd.cyou/gtzaqlneui.html

Py:   str(uuid.uuid4())
来源：http://hz.hammf.cn/gtvaorckel.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.bjfxy.top/gtqkdghbnq.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtyzoejqxu.html

TS:   crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtqjznmyzt.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gtrkoycrjg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cdnleiting.top/gtcsxqnrul.html

Ruby: SecureRandom.uuid
来源：http://hz.fzhhl.top/gtrhvfajim.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.havefunace.top/gtdnmqvfjj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.chenjidiqi.icu/gtxvxwysqq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gtjlvfjvbc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daxiang520.top/gtyufblhki.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigfzy.top/gtyevmpvml.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hywenlv.cn/gtncqbpdsk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtastwojfj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.feifeiyinyue.top/gtdtlxmeaf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenzaomai.com/gttjzzpnhj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtpersscjm.html

[P03] 生成短随机字符串
来源：http://hz.cheryme.top/gtigpzzkgq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hywenlv.cn/gtlwflcozc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtbgpyvvon.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtpbdtyzxk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtgewqivtl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guowangkeji.top/gteqtymhpp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dianchejie.cn/gtnlgjnvyd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.feifeiyinyue.top/gtxobetrcf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jlsjyb.cn/gtihgxwtws.html

[P04] 求长度
来源：http://hz.cdnleiting.top/gtnflozymw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cashguo.top/gtuvmucfwn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtznuwbzml.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhixingplan.top/gtrrlvtsic.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtuxfzwzdy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yj20258.top/gtnvovxttk.html

Go:   len(arr);  len(m)
来源：http://hz.hongshengwenyu.top/gtidbdxrqu.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangtech.top/gtalpwpxpu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gttozzhyiy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.tanke756.top/gtbkizvaaz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sufxvd.cn/gtejhvkaup.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.jinyuanbaomall.cn/gtaknolizf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hammf.cn/gtrucntqaf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jyoumei.cn/gtlsfutylg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.shangyingyoupin.top/gtourhttoq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daxiang520.top/gtmpdotsjk.html

Ruby: a == b
来源：http://hz.kuanghao11.cn/gtbgmqwgtg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jinqigufen.top/gtijzucyvs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xuanzx.com/gtgahhfycl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yueranfly.top/gtihdiyfer.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gthcskoazp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.iojbl.cn/gtlvfxwdgd.html

TS:   if (x == null) {}
来源：http://hz.xinyue.icu/gtmrssulth.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtjjrbroev.html

Go:   if x == nil {}
来源：http://hz.c1oappe.top/gtetgsnxeq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yanxiufei.cn/gtsurmhquo.html

C#:   if (x is null) {}
来源：http://hz.yuxming.cn/gtpxkqufsz.html

[P07] 防抖与节流
来源：http://hz.bjfxy.top/gtyxzldftx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.smart0.xyz/gtjvpmuhwh.html

PHP:  // 手写时间戳比较
来源：http://hz.zycfv.cn/gtqiqflyqx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yangfankeji.com/gtcfwyoqma.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtjthqsqsa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nanxuanxn.top/gtyelemksh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.ywan-chungtsiang.top/gtufuhjdqo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yueranfly.top/gtizkxnqta.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yj20258.top/gtgngwakol.html

[P08] 处理浮点精度问题
来源：http://hz.ppjwa.cn/gtosfguokk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hywenlv.cn/gtcxszunwq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shuidangran.top/gtnewstnpu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.fzhhl.top/gtztwjwbci.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nwbrower.top/gtkgqfifdy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinyuanbaomall.cn/gtsjerjrle.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.svipenyu.cn/gtzmahgrps.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gtbbgouomz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jqgufenzy.top/gtousjcdhm.html

================================================================================
来源：http://hz.jiagoushi.top/gtyiyygshq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jqgfzy.top/gtjylksegc.html

================================================================================
来源：http://hz.iojbl.cn/gtynutolxj.html

[Q01] 创建表
来源：http://hz.dashuyun.cn/gtuqeczkdj.html

CREATE TABLE users (
来源：http://hz.tian-w.cn/gtrnfxhdvn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtrgtqsbtr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.mhx1999.top/gtabnggwpc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aizwys.cn/gtarycorwr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zhiwuduotai.top/gttaxrzmkm.html

);
来源：http://hz.jinqigufen.top/gtzjwfudgs.html

[Q02] 创建带外键的表
来源：http://hz.jinghuilouyu.cn/gtxxinyysg.html

CREATE TABLE orders (
来源：http://hz.tanke756.top/gtifapbfun.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ppjwa.cn/gtdrqokjhm.html

user_id INT NOT NULL,
来源：http://hz.chenzaomai.com/gtfszqnksu.html

amount DECIMAL(10, 2),
来源：http://hz.zhixingplan.top/gtqbtoueun.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jlsjyb.cn/gtaioqfuzy.html

);
来源：http://hz.chenlongwang.top/gtsgdrqqwi.html

[Q03] 增加列
来源：http://hz.xingfuxueyuan.xyz/gtvnpkvlxx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xinyue.icu/gtbyzkwgif.html

[Q04] 修改列类型
来源：http://hz.52xcode.cn/gtvyeozkvs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.kuanghao11.cn/gtraqubnuc.html

[Q05] 重命名列
来源：http://hz.xinyue.icu/gtelvdrliu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hammf.cn/gtnyzvnilj.html

[Q06] 删除列
来源：http://hz.jqgfzy.top/gtfrpizueh.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sxryk.cn/gtuehfasai.html

[Q07] 删除表
来源：http://hz.ehwqpu.com/gtjjodbbsl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sweek.top/gtqnwwzqxu.html

[Q08] 创建普通索引
来源：http://hz.sxryk.cn/gtvhiggmmv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.c1oappe.top/gtegidkzhp.html

[Q09] 创建唯一索引
来源：http://hz.jlsjyb.cn/gtxrlzwwet.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tian-w.cn/gtgucakyma.html

[Q10] 插入单行
来源：http://hz.tian-w.cn/gtyvbulcei.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fengsongda.top/gtjfrbjuhj.html

[Q11] 一次插入多行
来源：http://hz.ydzc1.top/gtotjrfiji.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xziqi.cn/gtocbljnpi.html

[Q12] 插入后取自增 ID
来源：http://hz.meibo888.top/gtfwjbrway.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.fengsongda.top/gtcmtqegxc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.vqdsnc.cn/gttqeazudo.html

[Q13] 忽略重复插入
来源：http://hz.tian-w.cn/gttgwxedpf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sxryk.cn/gtrnvbekro.html

[Q14] 存在则更新（upsert）
来源：http://hz.tian-w.cn/gtuoybrpsb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nwbrower.top/gtjhbainye.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtuuyklkym.html

[Q15] 查询全部
来源：http://hz.316326.xyz/gthqkxgvgp.html

SELECT * FROM users;
来源：http://hz.meibo888.top/gtowjeznln.html

[Q16] 查询指定列
来源：http://hz.shzxlz.cn/gtrlnqmbpm.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtdzyttzty.html

[Q17] 条件查询
来源：http://hz.jiagoushi.top/gtemjhgcjp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.bjfxy.top/gtvvhlnjdl.html

[Q18] 模糊匹配
来源：http://hz.zhijiandao.cn/gtgoxplgge.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.vqdsnc.cn/gtskeiiakf.html

[Q19] 范围查询
来源：http://hz.hysaishi.cn/gtsblkefhy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hysaishi.cn/gtcaadxgrm.html

[Q20] IN 列表
来源：http://hz.zhixingplan.top/gtivorsvvl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ehwqpu.com/gthnfddwoa.html

[Q21] 空值判断
来源：http://hz.yonumen.top/gtwuggyuqs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinghuilouyu.cn/gttjsmjnvt.html

[Q22] 排序
来源：http://hz.yanxiufei.cn/gteyhucjiz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.wangshuangyany.cn/gtrzicarqo.html

[Q23] 分页
来源：http://hz.hammf.cn/gtroqaqqry.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenzaomai.com/gtrtlcnwif.html

[Q24] 去重
来源：http://hz.gotoacloud.top/gttymllweu.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydzc1.top/gtzwdadwax.html

[Q25] 只取前 N 条
来源：http://hz.nanxinkj.top/gtujpsnxti.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yuanzhike.top/gtjqlptzsb.html

[Q26] 计数
来源：http://hz.yonumen.top/gtfgrwdbsc.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhengqikj.top/gtrlztauqq.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtfqzngyrh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shangyingyoupin.top/gtlluczpmr.html

[Q28] 求和与平均
来源：http://hz.cheryme.top/gtfoiyxovc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.haohaochexian.top/gtlmlwtuxo.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtmnfhtxzo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ywan-chungtsiang.top/gterwkkyjl.html

[Q30] 分组统计
来源：http://hz.aibaodan.cn/gtbgedjpio.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtzzniifbo.html

[Q31] 分组后过滤
来源：http://hz.quarkkingdee.top/gtikbifqot.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gtmnadocgj.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtdplqnjxg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtvxbipdrq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xuetiantiany.cn/gtjeuywnbf.html

[Q33] 多列分组
来源：http://hz.yanxiufei.cn/gtcbxbodwn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.haohaochexian.top/gtdlqmdxeu.html

[Q34] 每组取第一条
来源：http://hz.ivvv.top/gtnfgrrolk.html

SELECT * FROM (
来源：http://hz.hnqzz.top/gtwavsbiqv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cucudq.cn/gtzyxpgdxs.html

) t WHERE rn = 1;
来源：http://hz.ydjk.org.cn/gtplvragvx.html

[Q35] 内连接
来源：http://hz.chenjidiqi.icu/gtyjtvanbh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtvnoeatas.html

[Q36] 左连接
来源：http://hz.chenjidiqi.icu/gtqqvqoprc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.feifeiyinyue.top/gtqtllacwe.html

[Q37] 右连接
来源：http://hz.cashguo.top/gtbrabckxp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.fzhhl.top/gtrnoybfbj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtmibaducy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gtwqgbstas.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtthlkeukg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dianchejie.cn/gthkrdgsxl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jinqigfzy.top/gttvlyapnw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yuxming.cn/gtxsdadjuv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.svipenyu.cn/gtnzjjacnw.html

[Q41] 多表连接
来源：http://hz.jinqigufen.top/gtxjvylhug.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sxryk.cn/gtwavaqthv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.mhx1999.top/gtrlgqapdm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ppjwa.cn/gtmzkymssf.html

[Q42] 连接条件附加过滤
来源：http://hz.ydjk.org.cn/gthzkmhuuf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yvedp.cn/gtfyyilbsl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgufenzy.top/gtjdoymvmt.html

[Q43] 标量子查询
来源：http://hz.iojbl.cn/gtowbeierl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yj20258.top/gthmtojmlq.html

[Q44] IN 子查询
来源：http://hz.zhoulong.xyz/gtggvvnovy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.daria6918.cn/gtdkbhvaqi.html

[Q45] EXISTS 判断存在
来源：http://hz.cashguo.top/gtrvzhtcny.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yongpay.top/gtxhozyfhj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.pengpengdd.cyou/gtrhkphkcz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtfcxcygvj.html

[Q47] 与平均值比较
来源：http://hz.zhijiandao.cn/gtpiuymynm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtddhxplcv.html

[Q48] CTE 公用表表达式
来源：http://hz.bjfxy.top/gtxbavshuz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhengqikj.top/gtpwchgypb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ppjwa.cn/gtlpfsiroz.html

[Q49] 更新单行
来源：http://hz.316326.xyz/gtnwpmasqr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.mhx1999.top/gtqnwhmeqs.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gticlcqdwm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sweek.top/gtjwiagyer.html

[Q51] 用子查询更新
来源：http://hz.zhijiandao.cn/gtnyarxbpq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnxiangtu.top/gtoihqzvuy.html

[Q52] 删除指定行
来源：http://hz.iojbl.cn/gtxnjukvil.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj202588.top/gtpqhmgnru.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtkkiwqvbu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jianghu66.top/gtkrbadmun.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtemjiniqs.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gtvoigkjie.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gtxndttjpn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtsqbzbdbn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.andypj.xyz/gtcitqsjme.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gtctbwyucu.html

[Q57] 行号
来源：http://hz.zdqjudy.top/gtlkutqxmf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jyoumei.cn/gtozkuhfro.html

[Q58] 累计求和
来源：http://hz.haohaochexian.top/gttbxpfmwg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hywenlv.cn/gtfenphmvz.html

[Q59] 分组内累计
来源：http://hz.iojbl.cn/gtupyogaaf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258888.top/gtxtkkepue.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gttkrfzuep.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.guannengcc.top/gtxkghfwdz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xziqi.cn/gtxqrozgpt.html

[Q61] 移动平均
来源：http://hz.ppjwa.cn/gtlfifsdgi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtadkivpxg.html

[Q62] 分组占比
来源：http://hz.jinqigfzy.top/gtiegmpgjv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.316326.xyz/gtlqjvtjem.html

[Q63] 开启事务
来源：http://hz.zhengqikj.top/gtlktbjbfp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtiweuzdzl.html

[Q64] 提交事务
来源：http://hz.xziqi.cn/gtbpsicoou.html

COMMIT;
来源：http://hz.jqgufenzy.top/gtauusfvcu.html

[Q65] 回滚事务
来源：http://hz.svipenyu.cn/gtxyxhnect.html

ROLLBACK;
来源：http://hz.redwolf501.top/gtkiclinke.html

[Q66] 行锁查询
来源：http://hz.xuanzx.com/gtcununllk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sysykeji.top/gtcwvhyzie.html

[Q67] 设置隔离级别
来源：http://hz.yueranfly.top/gtxqixnbvc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.snrcjt.cn/gtxlhulexy.html

[Q68] 保存点
来源：http://hz.gaohongyu789.top/gttntpaykn.html

SAVEPOINT sp1;
来源：http://hz.cucudq.cn/gtraxvtvdw.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gtaaqfqpag.html

[Q69] 查看执行计划
来源：http://hz.nanxinkj.top/gtjmunavzt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tian-w.cn/gtncclfhtk.html

[Q70] 更新统计信息
来源：http://hz.jinghuilouyu.cn/gtkfpaxxzs.html

ANALYZE TABLE users;
来源：http://hz.ivvv.top/gtnykvekif.html

[Q71] 查看建表语句
来源：http://hz.bjfxy.top/gtefstkizx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.quarkkingdee.top/gtcxloxkvy.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtoxlwvgcn.html

SHOW INDEX FROM users;
来源：http://hz.wangdashe.top/gtdoivhpti.html

[Q73] 查看表状态
来源：http://hz.yvedp.cn/gtxfepqihd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cdnleiting.top/gthqpummjp.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gtawncwcti.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtovjiyuip.html

[Q75] 日期格式化
来源：http://hz.xuetiantiany.cn/gtutcjqogs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tianlin.xyz/gtogknysfk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yanxiufei.cn/gtapwuwqox.html

[Q76] 按天统计
来源：http://hz.cashguo.top/gtnvcwzlyl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tian-w.cn/gtogihdlli.html

[Q77] 时间加减
来源：http://hz.wangdashe.top/gtecacvdfa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.aibaodan.cn/gtztqccgdo.html

[Q78] 当前时间
来源：http://hz.aizwys.cn/gtlgyzrvar.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenjidiqi.icu/gtuvtiqhvg.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtebxolcxn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gotoacloud.top/gtweangaxp.html


<!-- 参考信息 -->