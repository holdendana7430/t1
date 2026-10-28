代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtgqltimzw.html

[O03] 加锁保护共享数据
来源：http://hz.gaohongyu789.top/gtmgojiuio.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtjyuodomf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xinyue.icu/gtzrlucvmu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.andypj.xyz/gtjxdwqjrq.html

TS:   // 同 JS
来源：http://hz.pycfn.com/gturlaqbza.html

Java: synchronized (this) { shared++; }
来源：http://hz.jqgufenzy.top/gtlfzzzpgn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jyoumei.cn/gtsmcykohv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhixingplan.top/gtyatniebh.html

C#:   lock (gate) { shared++; }
来源：http://hz.zdqjudy.top/gthawctvbo.html

[O04] 定义异步函数并等待
来源：http://hz.zhoulong.xyz/gttleebrpu.html

Py:   async def f():⏎    await g()
来源：http://hz.havefunace.top/gttmirzavv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.mhx1999.top/gtwmqtczdq.html

JS:   async function f() { await g(); }
来源：http://hz.fzhhl.top/gtlojepjhm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtmimnaeyn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtrupdlkdx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.guannengcc.top/gtlbddxohm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.zycfv.cn/gtvemeptep.html

C#:   async Task F() { await G(); }
来源：http://hz.sufxvd.cn/gtjqlgfofz.html

[O05] 并发执行并等待全部完成
来源：http://hz.pycfn.com/gtywfxhzpq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hfpthk.cn/gtpilfwiii.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.wangdashe.top/gtirwoaafa.html

JS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtfjnetsam.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtcovgmcrr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangtech.top/gtejflljey.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.fengsongda.top/gtbmshnizl.html

Ruby: threads.map(&:join)
来源：http://hz.gaohongyu789.top/gtvdinusfs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenzaomai.com/gtdulkmnvr.html

[O06] 使用进程池
来源：http://hz.aibaodan.cn/gthdzaaxun.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gtrtysbtxh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangdashe.top/gtgnlztnmy.html

JS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtbbqbihyk.html

TS:   // child_process / cluster 模块
来源：http://hz.bjfxy.top/gttmxglspx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xziqi.cn/gtgdycqumm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ywan-chungtsiang.top/gtdehnvdwl.html

Ruby: // fork 块
来源：http://hz.hywenlv.cn/gtbgkcidyq.html

C#:   Parallel.For
来源：http://hz.xingfuxueyuan.xyz/gtmwospwoz.html

================================================================================
来源：http://hz.jianghu66.top/gtapvaakuk.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtcbyjswag.html

================================================================================
来源：http://hz.xinyue.icu/gtyyzuhfbv.html

[P01] 生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtoxytlxjt.html

Py:   str(uuid.uuid4())
来源：http://hz.zhixingplan.top/gtxdbsdtwd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zycfv.cn/gtjkajgnzn.html

JS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtxjkqorxg.html

TS:   crypto.randomUUID()
来源：http://hz.hammf.cn/gteoafdalv.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnxiangtu.top/gtplywadbu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.feifeiyinyue.top/gthoehhzkp.html

Ruby: SecureRandom.uuid
来源：http://hz.cucudq.cn/gtzfrybzyj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.redwolf501.top/gtbuokfbkn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.c1oappe.top/gtmlimqrnc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangkeji.top/gteaisdrzi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xuanzx.com/gtqeuwvpma.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangtech.top/gtrvyidxgi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yj20258.top/gtswetreir.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtrjialsfz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yuanzhike.top/gtowczqhyn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xziqi.cn/gtybugzdzm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guowangkeji.top/gtncwthrnj.html

[P03] 生成短随机字符串
来源：http://hz.52xcode.cn/gtkwwrjbas.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangkeji.top/gteqgxngor.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hywenlv.cn/gtzhptsjfm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.chenzaomai.com/gtrtbinyan.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtrznhjjri.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.iojbl.cn/gtodleqsoa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.dashuyun.cn/gtnldwtdqh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gtczbhrjti.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jlsjyb.cn/gtavrpvhnc.html

[P04] 求长度
来源：http://hz.jqgfzy.top/gtwdarogim.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shzxlz.cn/gtvgnvjxkv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtkntjxnku.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.tianlin.xyz/gtxsrlkaia.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nanxinkj.top/gtxdvcsgus.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgufenzy.top/gtbdwsbwlv.html

Go:   len(arr);  len(m)
来源：http://hz.tianlin.xyz/gtvemzwxrx.html

Ruby: x.length;  x.size
来源：http://hz.hongshengwenyu.top/gtsxdqebki.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.52xcode.cn/gtnicvrjzd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhijiandao.cn/gtxfescoyn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.quarkkingdee.top/gtaezdlqir.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.guannengcc.top/gtoeeotmmn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hammf.cn/gtmtxwonot.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtfpkdagqo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.daria6918.cn/gtutelovvq.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.ydjk.org.cn/gtisalalrn.html

Ruby: a == b
来源：http://hz.hywenlv.cn/gtbvkvzbgl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtctccbncv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shuidangran.top/gtpdvzzjmk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.tianlin.xyz/gtbgmewnyz.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtnmiwklyh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ydzc1.top/gtoaqanvrj.html

TS:   if (x == null) {}
来源：http://hz.zhijiandao.cn/gtavqpinsh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtphydlukb.html

Go:   if x == nil {}
来源：http://hz.yvedp.cn/gtutngqxsh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.kuanghao11.cn/gtlxdtxrik.html

C#:   if (x is null) {}
来源：http://hz.jinqigfzy.top/gtrtusimjl.html

[P07] 防抖与节流
来源：http://hz.chenlongwang.top/gtegjlxdpr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.pycfn.com/gtygrsvuvd.html

PHP:  // 手写时间戳比较
来源：http://hz.shanyushiyangkeji.top/gtqblkvudp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hongshengwenyu.top/gtegaforxq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtcgichhin.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xuanzx.com/gthlcwpjmk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.316326.xyz/gtdchjcirq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yuxming.cn/gtocsldmqi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xinyue.icu/gtseakgfrk.html

[P08] 处理浮点精度问题
来源：http://hz.havefunace.top/gtclodywar.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gthwiyqaei.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.hnqzz.top/gthmwldqrz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.gaohongyu789.top/gtcvydhtqc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yanxiufei.cn/gtebtnauxs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.c1oappe.top/gtfnxryipg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hywenlv.cn/gtvdfyiwtt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhixingplan.top/gtefgmixpe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pengpengdd.cyou/gtxlbetfya.html

================================================================================
来源：http://hz.guannengcc.top/gtpgwvdjmr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sweek.top/gthqrapvfq.html

================================================================================
来源：http://hz.quarkkingdee.top/gteehlgeet.html

[Q01] 创建表
来源：http://hz.meibo888.top/gtjngkcrfr.html

CREATE TABLE users (
来源：http://hz.0kj1m.cn/gthiowtxlk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtnnbqxctf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.jianghu66.top/gthujmuwnk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.dashuyun.cn/gtmhxnsdrp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.c1oappe.top/gtnaoctrks.html

);
来源：http://hz.nanxinkj.top/gtxngrijgp.html

[Q02] 创建带外键的表
来源：http://hz.fengsongda.top/gtieupzaji.html

CREATE TABLE orders (
来源：http://hz.zhengqikj.top/gtkfyqlqqe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtjshvmdjd.html

user_id INT NOT NULL,
来源：http://hz.aizwys.cn/gtmiojzrei.html

amount DECIMAL(10, 2),
来源：http://hz.zhongyouzk.top/gtykyrdzky.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.vqdsnc.cn/gtpxonssvg.html

);
来源：http://hz.andypj.xyz/gtcszlczjv.html

[Q03] 增加列
来源：http://hz.hnxiangtu.top/gtenrgswsb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.daria6918.cn/gtclvvivfh.html

[Q04] 修改列类型
来源：http://hz.sysykeji.top/gtygippglq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yongpay.top/gtqzjpzotm.html

[Q05] 重命名列
来源：http://hz.xuetiantiany.cn/gtsdqnfjhl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ehwqpu.com/gtkedhoiot.html

[Q06] 删除列
来源：http://hz.meibo888.top/gtibwzmzap.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ivvv.top/gtqsnnibgf.html

[Q07] 删除表
来源：http://hz.hywenlv.cn/gtuinoprhn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xuetiantiany.cn/gthvjafdgg.html

[Q08] 创建普通索引
来源：http://hz.wangdashe.top/gtbqtayntc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.tanke756.top/gtytohobig.html

[Q09] 创建唯一索引
来源：http://hz.aizwys.cn/gtodivciue.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.svipenyu.cn/gtmwupujft.html

[Q10] 插入单行
来源：http://hz.zhiwuduotai.top/gtbcyldaco.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ehwqpu.com/gtywsppyev.html

[Q11] 一次插入多行
来源：http://hz.jinghuilouyu.cn/gtfjrepvzn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.snrcjt.cn/gtbwifcipb.html

[Q12] 插入后取自增 ID
来源：http://hz.zhixingplan.top/gteocvcdvj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shangyingyoupin.top/gtszflfzwa.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gteafpvsoj.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gtyvwveeam.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xuetiantiany.cn/gtghnpvbdv.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuanzx.com/gtspfowvwa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yuanzhike.top/gtywslccal.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jiagoushi.top/gtzzlfdxsk.html

[Q15] 查询全部
来源：http://hz.daria6918.cn/gtewjhzmzv.html

SELECT * FROM users;
来源：http://hz.cashguo.top/gtaxcvhcpd.html

[Q16] 查询指定列
来源：http://hz.shzxlz.cn/gttgsguvfo.html

SELECT id, name FROM users;
来源：http://hz.zhiwuduotai.top/gtxddiovmo.html

[Q17] 条件查询
来源：http://hz.jinghuilouyu.cn/gtzhwvhbpg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.sweek.top/gtopigubmg.html

[Q18] 模糊匹配
来源：http://hz.gzhubu.top/gtmgyhpfob.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtbnfexiim.html

[Q19] 范围查询
来源：http://hz.pengpengdd.cyou/gtaxjgeyvp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sufxvd.cn/gthboppela.html

[Q20] IN 列表
来源：http://hz.xziqi.cn/gtbnijhxyf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtktzuuzdq.html

[Q21] 空值判断
来源：http://hz.xinyue.icu/gtbvoaezeo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.c1oappe.top/gtppmnixjb.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtdctfasgk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zhongyouzk.top/gtwojnyaul.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtzyrfblgm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxuanxn.top/gtaahvplvd.html

[Q24] 去重
来源：http://hz.havefunace.top/gtxlqklbtw.html

SELECT DISTINCT city FROM users;
来源：http://hz.sweek.top/gtzwlepmvu.html

[Q25] 只取前 N 条
来源：http://hz.316326.xyz/gtepruqqxw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.feifeiyinyue.top/gtmcjeomac.html

[Q26] 计数
来源：http://hz.zhiwuduotai.top/gtqiuajkju.html

SELECT COUNT(*) FROM users;
来源：http://hz.ehwqpu.com/gtfbqnzexi.html

[Q27] 条件计数
来源：http://hz.jinqigufen.top/gtlgttrthl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenlongwang.top/gttwyppwel.html

[Q28] 求和与平均
来源：http://hz.xziqi.cn/gtzismgbzc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gzhubu.top/gtwrfiwsxy.html

[Q29] 最大最小值
来源：http://hz.jinqigufen.top/gtlevvgtxo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shangyingyoupin.top/gtzlofiumn.html

[Q30] 分组统计
来源：http://hz.yvedp.cn/gtygqyoyij.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.wangshuangyany.cn/gtdbxdpouf.html

[Q31] 分组后过滤
来源：http://hz.yj20258.top/gtktofhgul.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.smart0.xyz/gtyznqqxrm.html

[Q32] 分组拼接字符串
来源：http://hz.9152youxi.cn/gtqtalgryq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtzuwikmqp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.daxiang520.top/gtulnbcbsm.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtivhoqyus.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.pycfn.com/gtlblcdpyy.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtfrnnnfoc.html

SELECT * FROM (
来源：http://hz.cucudq.cn/gtklleeywr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhaomingkeji.xyz/gtnnrlcnwk.html

) t WHERE rn = 1;
来源：http://hz.ppjwa.cn/gtzryxulxs.html

[Q35] 内连接
来源：http://hz.nanxinkj.top/gtonymojdz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtrbiixlcw.html

[Q36] 左连接
来源：http://hz.sweek.top/gtnfhufyyf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtdjbscfwo.html

[Q37] 右连接
来源：http://hz.sweek.top/gtacujnkwk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xylfe.cn/gtsdcbwhbu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sxryk.cn/gtdzecmuzv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydzc1.top/gttfibtjji.html

[Q39] 自连接（查上下级）
来源：http://hz.iojbl.cn/gtsbcmnzhy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinyuanbaomall.cn/gtwqtkdrgl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hywenlv.cn/gtilarfmkp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhijiandao.cn/gtiuawxsvf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhongyouzk.top/gtvkijjwng.html

[Q41] 多表连接
来源：http://hz.hysaishi.cn/gtdndospie.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gttaesipvb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinyuanbaomall.cn/gtivyrjgqi.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sxryk.cn/gtmgdipmxd.html

[Q42] 连接条件附加过滤
来源：http://hz.jlsjyb.cn/gtfywxkjru.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhaomingkeji.xyz/gtedodkfpy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gogol.net.cn/gtmtlrhsfd.html

[Q43] 标量子查询
来源：http://hz.xziqi.cn/gttzyvojlh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xinyue.icu/gttsemnxxr.html

[Q44] IN 子查询
来源：http://hz.chenlongwang.top/gtoxdimsfd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.xuetiantiany.cn/gtsxquymeo.html

[Q45] EXISTS 判断存在
来源：http://hz.hnxiangtu.top/gtxoebkvyi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhoulong.xyz/gtvlhtvrrl.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ehwqpu.com/gtizgvugbi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtdfgieyfv.html

[Q47] 与平均值比较
来源：http://hz.ppjwa.cn/gtldrejqtn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tanke756.top/gtjndbdllf.html

[Q48] CTE 公用表表达式
来源：http://hz.gaohongyu789.top/gtggezzheh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pycfn.com/gtpcnoyaxw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daria6918.cn/gttaaimvmf.html

[Q49] 更新单行
来源：http://hz.hammf.cn/gtuxyyonpt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cucudq.cn/gtmsbpkejn.html

[Q50] 批量更新
来源：http://hz.haohaochexian.top/gtebqfwrbg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtlpwpprnh.html

[Q51] 用子查询更新
来源：http://hz.dianchejie.cn/gtxqgyikiq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.ehwqpu.com/gtcbzztyqy.html

[Q52] 删除指定行
来源：http://hz.ppjwa.cn/gtqtxthghu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtvyoxhdds.html

[Q53] 按条件删除
来源：http://hz.hnqzz.top/gtdywllkfi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenzaomai.com/gthowquhsj.html

[Q54] 清空表
来源：http://hz.wangdashe.top/gtasahwxbg.html

TRUNCATE TABLE logs;
来源：http://hz.tianlin.xyz/gtovhqeiea.html

[Q55] 排名（并列占位）
来源：http://hz.quarkkingdee.top/gtjnrjwkhi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tianlin.xyz/gtigqgsfki.html

[Q56] 密集排名（并列不占位）
来源：http://hz.wangshuangyany.cn/gtcwljcoki.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gthxhomcoi.html

[Q57] 行号
来源：http://hz.chenzaomai.com/gtuiqazwhe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.bjfxy.top/gtvyrnkwnh.html

[Q58] 累计求和
来源：http://hz.tianlin.xyz/gtwbtugazr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jyoumei.cn/gtfzvgjadb.html

[Q59] 分组内累计
来源：http://hz.xziqi.cn/gtzaoxyegy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.pycfn.com/gtquguxesy.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtxgmwitph.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhongyouzk.top/gtcyljjpqo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fengsongda.top/gtyzusqguj.html

[Q61] 移动平均
来源：http://hz.pengpengdd.cyou/gtnkwcvpfh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.0kj1m.cn/gtpeexykre.html

[Q62] 分组占比
来源：http://hz.andypj.xyz/gtqlctbrfm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtxyzqlqsy.html

[Q63] 开启事务
来源：http://hz.ppjwa.cn/gteuqytshl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtsnnvjmtj.html

[Q64] 提交事务
来源：http://hz.zdqjudy.top/gttoqkvbhl.html

COMMIT;
来源：http://hz.zhijiandao.cn/gtwxroyftm.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangtech.top/gtqjtslule.html

ROLLBACK;
来源：http://hz.andypj.xyz/gtplexvdan.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtelvylvlp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.feifeiyinyue.top/gtheastomk.html

[Q67] 设置隔离级别
来源：http://hz.hongshengwenyu.top/gtaxjdedvg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gtymxeajud.html

[Q68] 保存点
来源：http://hz.chenjidiqi.icu/gtycqkrffg.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtpywlpmet.html

ROLLBACK TO sp1;
来源：http://hz.pycfn.com/gtftckptpk.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtwlvtzpoy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pycfn.com/gtpawihupw.html

[Q70] 更新统计信息
来源：http://hz.ywan-chungtsiang.top/gtboriypph.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtxtfzgrdh.html

[Q71] 查看建表语句
来源：http://hz.zhoulong.xyz/gtdnembizl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aizwys.cn/gtqfgyavvt.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtcftymxhk.html

SHOW INDEX FROM users;
来源：http://hz.smart0.xyz/gtlhjmcrjx.html

[Q73] 查看表状态
来源：http://hz.ydjk.org.cn/gtmqipmlpx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gaohongyu789.top/gtikfhomiq.html

[Q74] 强制使用索引
来源：http://hz.yueranfly.top/gtcjniyvgb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.9152youxi.cn/gtzolrvqyr.html

[Q75] 日期格式化
来源：http://hz.nanxuanxn.top/gtogjpijvu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fzhhl.top/gtwlbkskat.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.c1oappe.top/gtqwhskqnn.html

[Q76] 按天统计
来源：http://hz.zycfv.cn/gtshynhuan.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydjk.org.cn/gtlvkxqdvs.html

[Q77] 时间加减
来源：http://hz.gzhubu.top/gtjokwyfoh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gzhubu.top/gtadkphsfw.html

[Q78] 当前时间
来源：http://hz.daxiang520.top/gtdkfsmqla.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinyuanbaomall.cn/gtgourjqhn.html

[Q79] 字符串拼接
来源：http://hz.bjfxy.top/gtwnuflzgi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258.top/gtwxqxsgfh.html

[Q80] 字符串截取
来源：http://hz.cheryme.top/gticnkzutf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daria6918.cn/gtfrzqclku.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtdyqbsflm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtnqocnpho.html


<!-- 参考信息 -->