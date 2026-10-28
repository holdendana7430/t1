代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.pengpengdd.cyou/gtpntqnfwx.html

[O03] 加锁保护共享数据
来源：http://hz.hnqzz.top/gtnbjjwpax.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtrkxmzxuv.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hongshengwenyu.top/gtaegcghkk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gteoxgltpr.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtwmthfgvz.html

Java: synchronized (this) { shared++; }
来源：http://hz.yongpay.top/gttuxfpdpj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.0kj1m.cn/gtyljadqlj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtiyjkeoed.html

C#:   lock (gate) { shared++; }
来源：http://hz.yangfankeji.com/gtxisxvozc.html

[O04] 定义异步函数并等待
来源：http://hz.zhixingplan.top/gtybhmbkjj.html

Py:   async def f():⏎    await g()
来源：http://hz.hfpthk.cn/gtfistwgwq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhixingplan.top/gtlzubhnwn.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtacabyqrx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtqhiydblg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yonumen.top/gtbnbtsmmg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.0kj1m.cn/gtwobjbkhe.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gteopdljfh.html

C#:   async Task F() { await G(); }
来源：http://hz.xylfe.cn/gtecpclxmc.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhiwuduotai.top/gtawifospt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.0kj1m.cn/gtpvzruqzz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gtwblanceh.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gthpvletpv.html

TS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtxqqeibpc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.bjfxy.top/gtznzuxygi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sweek.top/gtokovntkq.html

Ruby: threads.map(&:join)
来源：http://hz.havefunace.top/gthkhbovta.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dianchejie.cn/gtncjogjhg.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtnkblkvbp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ydjk.org.cn/gtmkvzdrdt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shanyushiyangtech.top/gtxxneutoz.html

JS:   // child_process / cluster 模块
来源：http://hz.gzhubu.top/gtwbeasxlv.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtzjcxruvh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinyuanbaomall.cn/gtikxnulnu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj202588.top/gthubzknlt.html

Ruby: // fork 块
来源：http://hz.fzhhl.top/gtyumdwlps.html

C#:   Parallel.For
来源：http://hz.aizwys.cn/gtkthsxdfv.html

================================================================================
来源：http://hz.andypj.xyz/gtedscblxb.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtrwiuapzt.html

================================================================================
来源：http://hz.tianlin.xyz/gtylpbfoia.html

[P01] 生成 UUID
来源：http://hz.pycfn.com/gtfluokxht.html

Py:   str(uuid.uuid4())
来源：http://hz.fzhhl.top/gtwkszrkxw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hywenlv.cn/gtwnihpybz.html

JS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gttxuqqioh.html

TS:   crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtywzdfppo.html

Java: UUID.randomUUID().toString()
来源：http://hz.yongpay.top/gteluaptxv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gtdggdaxjn.html

Ruby: SecureRandom.uuid
来源：http://hz.9152youxi.cn/gtfjrypooz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jianghu66.top/gtreytbqhk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.havefunace.top/gtlqivjdjd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cucudq.cn/gtthzlwrgu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xinyue.icu/gtvijbzqpw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tianlin.xyz/gtkbdtmxwo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgufenzy.top/gtmsvjfbzb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aizwys.cn/gtwumzbjhq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgufenzy.top/gtfbcnhmlj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ivvv.top/gtmvtynuhy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ppjwa.cn/gtunbhhwvl.html

[P03] 生成短随机字符串
来源：http://hz.dianchejie.cn/gtfmdnglqe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydzc1.top/gttbxvntwi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.fengsongda.top/gtgpvjpqts.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guowangkeji.top/gtlxaucaxk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gtqycrvasj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gtzsgzjqqe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xziqi.cn/gtyiyelcoh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnqzz.top/gtqludchct.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hysaishi.cn/gtchlpmgxn.html

[P04] 求长度
来源：http://hz.kuanghao11.cn/gtgplfncgo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gzhubu.top/gtcomjnwns.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtmvcxyead.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtezbvmder.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gtrsafjgip.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jianghu66.top/gtgrqpwqbx.html

Go:   len(arr);  len(m)
来源：http://hz.guannengcc.top/gtrwtlefzk.html

Ruby: x.length;  x.size
来源：http://hz.jqgfzy.top/gtvgsdhwwn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.sweek.top/gtujrobyvi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtfpbvzkud.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.havefunace.top/gtzfqebxwh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gtgthqixby.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.tanke756.top/gtbojnjkwi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuxming.cn/gtngvygkoz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.316326.xyz/gttpfnstrj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yvedp.cn/gtxsyuudcx.html

Ruby: a == b
来源：http://hz.yonumen.top/gtnhrxbgiy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hywenlv.cn/gtjnxsbszr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jiagoushi.top/gttukwhsey.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ybcxt.top/gttkdplcbh.html

PHP:  if (empty($x)) {}
来源：http://hz.svipenyu.cn/gtfiukdsbj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gtdvlqlvbj.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtmenjljww.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.nanxinkj.top/gtibracxbg.html

Go:   if x == nil {}
来源：http://hz.haohaochexian.top/gtqqevfiax.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtycfivdos.html

C#:   if (x is null) {}
来源：http://hz.gzhubu.top/gtihbpbjhd.html

[P07] 防抖与节流
来源：http://hz.kuanghao11.cn/gtqpaftqvj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jyoumei.cn/gtunzkznhc.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtfwcjacrm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.dashuyun.cn/gtgesfijwg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinghuilouyu.cn/gtoagyghls.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinghuilouyu.cn/gtlhmvjgha.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.pengpengdd.cyou/gtxvfihvjm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cashguo.top/gtlwlclavx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shangyingyoupin.top/gtxswludvj.html

[P08] 处理浮点精度问题
来源：http://hz.ydzc1.top/gttzxdjmym.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtoujavlik.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yanxiufei.cn/gtcptwqhpm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xziqi.cn/gtwrfdoduy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nwbrower.top/gtakynfogx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tian-w.cn/gtaveutwon.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhiwuduotai.top/gtlghvnbhn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.pycfn.com/gtyjnpxstd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenlongwang.top/gtoagmonyn.html

================================================================================
来源：http://hz.daria6918.cn/gtacrcevru.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sufxvd.cn/gtjirautlg.html

================================================================================
来源：http://hz.pycfn.com/gtaxxbydku.html

[Q01] 创建表
来源：http://hz.sufxvd.cn/gtzzkyatsz.html

CREATE TABLE users (
来源：http://hz.sysykeji.top/gtrwyvdboa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhixingplan.top/gtlqjhkgrs.html

name VARCHAR(50) NOT NULL,
来源：http://hz.cqqwz.cn/gtqmcnsjas.html

email VARCHAR(100) UNIQUE,
来源：http://hz.haohaochexian.top/gtquqtdcik.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yangfankeji.com/gtliyhvgve.html

);
来源：http://hz.jqgfzy.top/gtdevrpbnt.html

[Q02] 创建带外键的表
来源：http://hz.nwbrower.top/gteoinpubd.html

CREATE TABLE orders (
来源：http://hz.vqdsnc.cn/gtbobqsfgu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gtaxhrjome.html

user_id INT NOT NULL,
来源：http://hz.daria6918.cn/gtcoytphto.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtjsbcwoxl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.dashuyun.cn/gtngldsoew.html

);
来源：http://hz.guannengcc.top/gtyocrfkfi.html

[Q03] 增加列
来源：http://hz.yuanzhike.top/gtkgtjkult.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jinghuilouyu.cn/gtlkqlhrgu.html

[Q04] 修改列类型
来源：http://hz.shanyushiyangtech.top/gtxrizizmg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.smart0.xyz/gthudpiuxf.html

[Q05] 重命名列
来源：http://hz.mhx1999.top/gtcwydqrfb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sysykeji.top/gtaarwrndp.html

[Q06] 删除列
来源：http://hz.jinqigfzy.top/gtwzbqpzsc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.mhx1999.top/gtxqesmzoe.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gttusoipry.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtpoihlked.html

[Q08] 创建普通索引
来源：http://hz.daxiang520.top/gthjkefdsv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.guowangkeji.top/gtocowqbeq.html

[Q09] 创建唯一索引
来源：http://hz.chenzaomai.com/gtqkgkvzbu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.birdmap.top/gtuggtzbhe.html

[Q10] 插入单行
来源：http://hz.9152youxi.cn/gtjmdxtdlr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydzc1.top/gteefqjkjr.html

[Q11] 一次插入多行
来源：http://hz.andypj.xyz/gtxjubjzjk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258888.top/gtczlbwnyl.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtlebhyvta.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cqqwz.cn/gtyiiafjlh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daxiang520.top/gtnqxljfxm.html

[Q13] 忽略重复插入
来源：http://hz.vqdsnc.cn/gtbxpdwgcn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cqqwz.cn/gtygpvywfc.html

[Q14] 存在则更新（upsert）
来源：http://hz.andypj.xyz/gtpysskxyb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hammf.cn/gtitlhzifv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xingfuxueyuan.xyz/gtqpuxeomj.html

[Q15] 查询全部
来源：http://hz.c1oappe.top/gtxopmhtbm.html

SELECT * FROM users;
来源：http://hz.xinyue.icu/gtyopiqazt.html

[Q16] 查询指定列
来源：http://hz.svipenyu.cn/gtplyvnlbx.html

SELECT id, name FROM users;
来源：http://hz.tianlin.xyz/gtragkggkr.html

[Q17] 条件查询
来源：http://hz.zhoulong.xyz/gthamvkogh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.bjfxy.top/gttarbqzps.html

[Q18] 模糊匹配
来源：http://hz.ppjwa.cn/gtfizifpkd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xylfe.cn/gtjsbpnewl.html

[Q19] 范围查询
来源：http://hz.gogol.net.cn/gtfgufweak.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigufen.top/gtgwglqrer.html

[Q20] IN 列表
来源：http://hz.cqqwz.cn/gtodnzvgrs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtygncldtc.html

[Q21] 空值判断
来源：http://hz.zhengqikj.top/gtbdnveruv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xuanzx.com/gtbkbcmquj.html

[Q22] 排序
来源：http://hz.chenlongwang.top/gtcixslqmj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xziqi.cn/gthcaunoho.html

[Q23] 分页
来源：http://hz.tianlin.xyz/gtkwjzigic.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.redwolf501.top/gtagncfvvn.html

[Q24] 去重
来源：http://hz.xylfe.cn/gtsclhfptc.html

SELECT DISTINCT city FROM users;
来源：http://hz.haohaochexian.top/gtoyikdezc.html

[Q25] 只取前 N 条
来源：http://hz.yj20258888.top/gtoodeunwa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.mhx1999.top/gtxzpgdvaa.html

[Q26] 计数
来源：http://hz.daxiang520.top/gtxquvwtjx.html

SELECT COUNT(*) FROM users;
来源：http://hz.kuanghao11.cn/gtwfbbwjsw.html

[Q27] 条件计数
来源：http://hz.dashuyun.cn/gtwqlsitum.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sufxvd.cn/gtnetsrfhm.html

[Q28] 求和与平均
来源：http://hz.ywan-chungtsiang.top/gtqtedoltp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtmpouqoap.html

[Q29] 最大最小值
来源：http://hz.zhixingplan.top/gtmghqwhuy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xziqi.cn/gtpnepzzrh.html

[Q30] 分组统计
来源：http://hz.fzhhl.top/gtvklybylz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtrymvwrbo.html

[Q31] 分组后过滤
来源：http://hz.birdmap.top/gtnuwrhtsn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.52xcode.cn/gtbezsktoy.html

[Q32] 分组拼接字符串
来源：http://hz.zhengqikj.top/gtbvayitea.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtkvnyojea.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sxryk.cn/gtcybrgocc.html

[Q33] 多列分组
来源：http://hz.jiagoushi.top/gtqdcqaole.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ywan-chungtsiang.top/gtawvebrqv.html

[Q34] 每组取第一条
来源：http://hz.shangyingyoupin.top/gtsrsisoxr.html

SELECT * FROM (
来源：http://hz.yanxiufei.cn/gtgwgjousu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cdnleiting.top/gteoiynxli.html

) t WHERE rn = 1;
来源：http://hz.gaohongyu789.top/gtjuxtibwv.html

[Q35] 内连接
来源：http://hz.sweek.top/gtxpreubun.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtjzepckdn.html

[Q36] 左连接
来源：http://hz.aizwys.cn/gtxhetcxir.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtdwkbxnyw.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gtxhxsbutr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gzhubu.top/gtsxreieeq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tianlin.xyz/gtlrkqgeba.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258.top/gtoxfqasqj.html

[Q39] 自连接（查上下级）
来源：http://hz.gaohongyu789.top/gtbuhzlxot.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zycfv.cn/gtrpgykfln.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.bjfxy.top/gtaovovkla.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenjidiqi.icu/gteqidbcfe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tianlin.xyz/gtszcknhgj.html

[Q41] 多表连接
来源：http://hz.xylfe.cn/gtrwqdetne.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.aibaodan.cn/gtrbkrndki.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cashguo.top/gttzpqtfkl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigfzy.top/gtxpiwrtfi.html

[Q42] 连接条件附加过滤
来源：http://hz.zhijiandao.cn/gtnpikkpra.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gotoacloud.top/gtzuuzlmsy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.vqdsnc.cn/gthybbgnpf.html

[Q43] 标量子查询
来源：http://hz.birdmap.top/gtlseckkqs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daxiang520.top/gtdalvekol.html

[Q44] IN 子查询
来源：http://hz.jianghu66.top/gthdmuqksu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenjidiqi.icu/gtxtlnkljt.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtodabbxqp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtasbzzevj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gtxqvjvmwc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.feifeiyinyue.top/gttwxfoegf.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtjhzfchje.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydjk.org.cn/gtaeehlbzl.html

[Q48] CTE 公用表表达式
来源：http://hz.redwolf501.top/gtlcmcksoa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258888.top/gtlatobrps.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hysaishi.cn/gtdezjvgtr.html

[Q49] 更新单行
来源：http://hz.xziqi.cn/gtwgpxqmwf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj202588.top/gtfiwvvftp.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtagpqawcn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yueranfly.top/gtpatjkzbr.html

[Q51] 用子查询更新
来源：http://hz.fengsongda.top/gtwcdszded.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xziqi.cn/gtzxexqsya.html

[Q52] 删除指定行
来源：http://hz.chenjidiqi.icu/gtyjgqtvkx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.mhx1999.top/gttufrcjyt.html

[Q53] 按条件删除
来源：http://hz.chenzaomai.com/gtwolecnuu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.birdmap.top/gtigbqkddh.html

[Q54] 清空表
来源：http://hz.316326.xyz/gtiqqwyacv.html

TRUNCATE TABLE logs;
来源：http://hz.yuanzhike.top/gtbjftalwk.html

[Q55] 排名（并列占位）
来源：http://hz.shuidangran.top/gteuyflcky.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinyuanbaomall.cn/gtteizigmj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ywan-chungtsiang.top/gtxrwlcjro.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tian-w.cn/gtoycwayuu.html

[Q57] 行号
来源：http://hz.yj202588.top/gtwagfbmnx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fzhhl.top/gtuqrrfjha.html

[Q58] 累计求和
来源：http://hz.nanxuanxn.top/gtbpmitwrq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xuanzx.com/gtyqskhffq.html

[Q59] 分组内累计
来源：http://hz.guowangkeji.top/gtbqfitdch.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gtpbcoaoal.html

[Q60] 取上一行 / 下一行
来源：http://hz.daria6918.cn/gtnwdsskoh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhixingplan.top/gtwielcvta.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sysykeji.top/gtthzssqep.html

[Q61] 移动平均
来源：http://hz.tanke756.top/gtheapgxae.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.vqdsnc.cn/gttpiwrfhg.html

[Q62] 分组占比
来源：http://hz.redwolf501.top/gtsonajqee.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gtszzihpiz.html

[Q63] 开启事务
来源：http://hz.jinqigfzy.top/gtzxuljtle.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aizwys.cn/gtyrvbhaov.html

[Q64] 提交事务
来源：http://hz.nwbrower.top/gtwgkarydv.html

COMMIT;
来源：http://hz.cdnleiting.top/gtwcqjwukq.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gteronxbvx.html

ROLLBACK;
来源：http://hz.yj202588.top/gtijlyetbj.html

[Q66] 行锁查询
来源：http://hz.shzxlz.cn/gtbbhtqwpn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258.top/gtxbwsuojc.html

[Q67] 设置隔离级别
来源：http://hz.chenjidiqi.icu/gtccxoouch.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hfpthk.cn/gtucfxnhzt.html

[Q68] 保存点
来源：http://hz.xylfe.cn/gtyzcbvkre.html

SAVEPOINT sp1;
来源：http://hz.gzhubu.top/gtwawkqprp.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtrmxwzsfg.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtmoutrxuc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtbmbnylgj.html

[Q70] 更新统计信息
来源：http://hz.wangdashe.top/gthutofyyo.html

ANALYZE TABLE users;
来源：http://hz.yongpay.top/gtoauopudp.html

[Q71] 查看建表语句
来源：http://hz.shuidangran.top/gtosnchbwb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yueranfly.top/gtdcfgbdqw.html

[Q72] 查看索引
来源：http://hz.gogol.net.cn/gtmsvstzwu.html

SHOW INDEX FROM users;
来源：http://hz.zhixingplan.top/gtzlytqgzt.html

[Q73] 查看表状态
来源：http://hz.hysaishi.cn/gtxowmktdb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtmhafeyjd.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtsapsvklu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgfzy.top/gtigwbfbbk.html

[Q75] 日期格式化
来源：http://hz.zhaomingkeji.xyz/gtcxgteagw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtithzlpmh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hnqzz.top/gtfzhunykn.html

[Q76] 按天统计
来源：http://hz.52xcode.cn/gttetykbcf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yongpay.top/gttpeooskc.html

[Q77] 时间加减
来源：http://hz.yongpay.top/gtjtcdomrd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtlxqcgwon.html

[Q78] 当前时间
来源：http://hz.gzhubu.top/gtkmlyypew.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ivvv.top/gtvekfwbty.html

[Q79] 字符串拼接
来源：http://hz.xziqi.cn/gtxiditina.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.vqdsnc.cn/gtotbytujw.html

[Q80] 字符串截取
来源：http://hz.hysaishi.cn/gtlqpqvspf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.guowangkeji.top/gttehzsapp.html

[Q81] 字符串替换
来源：http://hz.jinqigufen.top/gttolxlddk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.feifeiyinyue.top/gtbwcbjfjr.html


<!-- 参考信息 -->