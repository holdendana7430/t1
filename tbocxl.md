代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guowangkeji.top/gtwsldwqjy.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258888.top/gtiioguxwk.html

Py:   with lock: shared += 1
来源：http://hz.cucudq.cn/gtmbwtsbhg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinqigufen.top/gtmpcykyla.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yanxiufei.cn/gtyukursmm.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtkzqxcief.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnqzz.top/gtvkfbissi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gtymraaehi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yvedp.cn/gtdkkvcqzv.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhoulong.xyz/gtosaxatgj.html

[O04] 定义异步函数并等待
来源：http://hz.shangyingyoupin.top/gtnnrblsly.html

Py:   async def f():⏎    await g()
来源：http://hz.ivvv.top/gtrfyjaheo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.haohaochexian.top/gtveszadrh.html

JS:   async function f() { await g(); }
来源：http://hz.gaohongyu789.top/gthfvjcabs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtpgegjvoa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jinghuilouyu.cn/gtxlqccpdo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtllovcvny.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenzaomai.com/gtipmxrtft.html

C#:   async Task F() { await G(); }
来源：http://hz.316326.xyz/gtnufcwkpv.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtfqeincar.html

Py:   asyncio.gather(*tasks)
来源：http://hz.iojbl.cn/gtyrkccqir.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.snrcjt.cn/gtjcebokfu.html

JS:   await Promise.all(tasks)
来源：http://hz.zhoulong.xyz/gtmcqnghut.html

TS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtovwpsnac.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gzhubu.top/gthbdtcyjd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtvodgvmqc.html

Ruby: threads.map(&:join)
来源：http://hz.shangyingyoupin.top/gtocjrsxer.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhoulong.xyz/gtkkdphfut.html

[O06] 使用进程池
来源：http://hz.hywenlv.cn/gtlaslhmvq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guowangkeji.top/gtufdolmud.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenlongwang.top/gttvlmsqgc.html

JS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtrhpfgruo.html

TS:   // child_process / cluster 模块
来源：http://hz.hfpthk.cn/gtimbcvnae.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cqqwz.cn/gtqmhflmxh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yonumen.top/gtpwqcxetl.html

Ruby: // fork 块
来源：http://hz.xziqi.cn/gthshbrjpr.html

C#:   Parallel.For
来源：http://hz.shanyushiyangkeji.top/gtyjrjtyml.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtilkbiepb.html

P. 常用工具函数
来源：http://hz.ivvv.top/gtgpbmsrbn.html

================================================================================
来源：http://hz.ppjwa.cn/gtapsdfknc.html

[P01] 生成 UUID
来源：http://hz.yueranfly.top/gtsimamosz.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtyfqaryzb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtmgbltmud.html

JS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtcmxmskwd.html

TS:   crypto.randomUUID()
来源：http://hz.chenzaomai.com/gtghdynyqs.html

Java: UUID.randomUUID().toString()
来源：http://hz.ywan-chungtsiang.top/gtcjmonaej.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gaohongyu789.top/gtjzmrsdfn.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gtkxndtjhh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.316326.xyz/gtgblthdvf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinghuilouyu.cn/gtntwmajii.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sysykeji.top/gtgvfxibtc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgfzy.top/gtcpeefdka.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xziqi.cn/gtrspldiih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shangyingyoupin.top/gtwffzairi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.0kj1m.cn/gtuywokexm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cdnleiting.top/gtkckrczqv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtexrcqqjo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.nwbrower.top/gtcaotdkld.html

[P03] 生成短随机字符串
来源：http://hz.xylfe.cn/gtqaaarinb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtpolwgbul.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.nwbrower.top/gtilatlotr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shuidangran.top/gtsrsrezjf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gttyqbtijb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shangyingyoupin.top/gthldddtun.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuanzx.com/gtttxwowpa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daxiang520.top/gtyavezxpv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtyniwbfld.html

[P04] 求长度
来源：http://hz.redwolf501.top/gthhltcamk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ywan-chungtsiang.top/gtjpjxsmgx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtgnxdeevh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtfaaflosc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.0kj1m.cn/gtbkywpyqf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cdnleiting.top/gtocirnuvp.html

Go:   len(arr);  len(m)
来源：http://hz.zdqjudy.top/gttyvsgjcw.html

Ruby: x.length;  x.size
来源：http://hz.guowangkeji.top/gtlsxmfjki.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.feifeiyinyue.top/gtjsxbysmf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.andypj.xyz/gtxfsxcsem.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.redwolf501.top/gtbbkornsp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gogol.net.cn/gtegdrvcoa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daxiang520.top/gtegabvutl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtwhrbatqc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jqgfzy.top/gtxtxvnlyv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.vqdsnc.cn/gtqmepyxrl.html

Ruby: a == b
来源：http://hz.smart0.xyz/gtyirqjibp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ydzc1.top/gtwrhlmdwg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhaomingkeji.xyz/gtapqlaywj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.mhx1999.top/gtcchuykal.html

PHP:  if (empty($x)) {}
来源：http://hz.ydjk.org.cn/gtniujmxuq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.andypj.xyz/gtnshiojxd.html

TS:   if (x == null) {}
来源：http://hz.fzhhl.top/gtnlzogplv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.yvedp.cn/gtgelzwrsa.html

Go:   if x == nil {}
来源：http://hz.iojbl.cn/gthrfusblf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hongshengwenyu.top/gtudxmmdsl.html

C#:   if (x is null) {}
来源：http://hz.zhongyouzk.top/gtwzwfpfdb.html

[P07] 防抖与节流
来源：http://hz.cqqwz.cn/gtduwcynrc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nanxuanxn.top/gtahjbbudj.html

PHP:  // 手写时间戳比较
来源：http://hz.shangyingyoupin.top/gtlfpmfibc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtjffguppd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtnlxyeqkc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.dashuyun.cn/gtymprzkax.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yangfankeji.com/gthnlcfizs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sxryk.cn/gtsonzbuvv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.meibo888.top/gtnkhqovfv.html

[P08] 处理浮点精度问题
来源：http://hz.zhiwuduotai.top/gtiyjdqeyu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.dianchejie.cn/gtoahrcjga.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nwbrower.top/gtjbbxmzcz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yangfankeji.com/gtuewyhilk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenzaomai.com/gtzuvyyumk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.kuanghao11.cn/gtggyrbvrw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhoulong.xyz/gtjyoxvygo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhoulong.xyz/gtcuibtmth.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.dashuyun.cn/gtrehvoant.html

================================================================================
来源：http://hz.guowangkeji.top/gtytcvmbcz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.snrcjt.cn/gtagaewcca.html

================================================================================
来源：http://hz.birdmap.top/gtiwuxatoa.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gtybifsymi.html

CREATE TABLE users (
来源：http://hz.cucudq.cn/gtdcykftxk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tian-w.cn/gtdnqdvtyy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.wangdashe.top/gtpicffhzt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.svipenyu.cn/gtvkmtvkvl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yangfankeji.com/gtnocwawrd.html

);
来源：http://hz.shanyushiyangtech.top/gtulqtgrqe.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtyamrmtoi.html

CREATE TABLE orders (
来源：http://hz.hfpthk.cn/gtkgecqqbx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtwzmrlela.html

user_id INT NOT NULL,
来源：http://hz.ehwqpu.com/gtvycfqzpp.html

amount DECIMAL(10, 2),
来源：http://hz.zycfv.cn/gtzjjyrpsc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.guowangkeji.top/gtbkcyekmc.html

);
来源：http://hz.jinghuilouyu.cn/gtqkxtkgwv.html

[Q03] 增加列
来源：http://hz.jinqigufen.top/gtyahcooqm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.haohaochexian.top/gtuilawxer.html

[Q04] 修改列类型
来源：http://hz.ywan-chungtsiang.top/gtctnzburj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.316326.xyz/gtlhqmnhnr.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtfgpfoxyr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtmieveiii.html

[Q06] 删除列
来源：http://hz.yj202588.top/gtwdcaurku.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hywenlv.cn/gtingcynel.html

[Q07] 删除表
来源：http://hz.chenzaomai.com/gtfftuszxi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yongpay.top/gtnrwyelcm.html

[Q08] 创建普通索引
来源：http://hz.ivvv.top/gtcekudmqu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.birdmap.top/gtcrtqaxhb.html

[Q09] 创建唯一索引
来源：http://hz.haohaochexian.top/gtnyztfzus.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258.top/gthtgwcsyu.html

[Q10] 插入单行
来源：http://hz.guannengcc.top/gtzlrozlup.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gtloahpwes.html

[Q11] 一次插入多行
来源：http://hz.svipenyu.cn/gtexzzokvi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhengqikj.top/gtoqlyfpwt.html

[Q12] 插入后取自增 ID
来源：http://hz.xylfe.cn/gtklnlojwq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.wangshuangyany.cn/gtdvcqybvs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yuxming.cn/gtbtjticda.html

[Q13] 忽略重复插入
来源：http://hz.yvedp.cn/gtcgrjsizx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gaohongyu789.top/gtytxogwfr.html

[Q14] 存在则更新（upsert）
来源：http://hz.cdnleiting.top/gtabkkdbpe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.redwolf501.top/gtxkocnpch.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.haohaochexian.top/gtrdodymrj.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtmtbclyqr.html

SELECT * FROM users;
来源：http://hz.shanyushiyangtech.top/gtiidszuts.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gttynybdtj.html

SELECT id, name FROM users;
来源：http://hz.shangyingyoupin.top/gtlsktiymm.html

[Q17] 条件查询
来源：http://hz.316326.xyz/gttfrpffld.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.52xcode.cn/gtoxneaswh.html

[Q18] 模糊匹配
来源：http://hz.hnxiangtu.top/gtuprzsbiz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gaohongyu789.top/gtidxszndf.html

[Q19] 范围查询
来源：http://hz.zhiwuduotai.top/gthtgodigr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ehwqpu.com/gtdeqhjriw.html

[Q20] IN 列表
来源：http://hz.zhijiandao.cn/gtyrfgriof.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.iojbl.cn/gtwvnnrjpo.html

[Q21] 空值判断
来源：http://hz.havefunace.top/gtahwtflrp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hysaishi.cn/gtwfruvkmt.html

[Q22] 排序
来源：http://hz.jinyuanbaomall.cn/gteehmbwek.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ppjwa.cn/gtrfvaofip.html

[Q23] 分页
来源：http://hz.c1oappe.top/gtgjhxqdrv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhengqikj.top/gtpyjizzbe.html

[Q24] 去重
来源：http://hz.ppjwa.cn/gtdskwhiwa.html

SELECT DISTINCT city FROM users;
来源：http://hz.xziqi.cn/gttnpaanbo.html

[Q25] 只取前 N 条
来源：http://hz.yueranfly.top/gtgggtxvhr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jianghu66.top/gtqizuupkf.html

[Q26] 计数
来源：http://hz.iojbl.cn/gtzudfzwja.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtjjqlbxyr.html

[Q27] 条件计数
来源：http://hz.shangyingyoupin.top/gtcescpslh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.fzhhl.top/gtdyadcvzy.html

[Q28] 求和与平均
来源：http://hz.fengsongda.top/gtfbjtikeh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ehwqpu.com/gtnkjcrrej.html

[Q29] 最大最小值
来源：http://hz.52xcode.cn/gtdlheqnnv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xinyue.icu/gttaydrrfd.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gtjgwtupya.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtuxyykoly.html

[Q31] 分组后过滤
来源：http://hz.jlsjyb.cn/gtbbrxovxy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtaiddjfec.html

[Q32] 分组拼接字符串
来源：http://hz.yuanzhike.top/gtqvjqbrnc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtfudbzrhk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sxryk.cn/gtshzjrmbc.html

[Q33] 多列分组
来源：http://hz.ydzc1.top/gtnmnahgkd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yvedp.cn/gtxzvbesst.html

[Q34] 每组取第一条
来源：http://hz.quarkkingdee.top/gtbhnpdcpe.html

SELECT * FROM (
来源：http://hz.shanyushiyangtech.top/gthllqvier.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yonumen.top/gtqdjpfcyh.html

) t WHERE rn = 1;
来源：http://hz.yueranfly.top/gtfgwwkayl.html

[Q35] 内连接
来源：http://hz.redwolf501.top/gtsnhxbvlm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtqgmwagwu.html

[Q36] 左连接
来源：http://hz.hammf.cn/gtqkuysalc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtezjdktdl.html

[Q37] 右连接
来源：http://hz.sweek.top/gttamfhpfq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.guannengcc.top/gtudqhhzoz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hongshengwenyu.top/gtorrcymam.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtrcozvkxy.html

[Q39] 自连接（查上下级）
来源：http://hz.yonumen.top/gtstrlpdmr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxuanxn.top/gtaipdbrbn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.meibo888.top/gtgkidvgdz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.snrcjt.cn/gtgmpidxbj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtxziunyud.html

[Q41] 多表连接
来源：http://hz.yj20258888.top/gtxocdtuig.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ydjk.org.cn/gtsqzqkouz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jqgfzy.top/gtuzpbmtzf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtbwjxprqs.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigufen.top/gtkodwnogj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yonumen.top/gtniooqlfd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.aizwys.cn/gtgttzjacq.html

[Q43] 标量子查询
来源：http://hz.iojbl.cn/gtxyaeeijb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guowangkeji.top/gtwjkzougo.html

[Q44] IN 子查询
来源：http://hz.nanxuanxn.top/gtqipuqyjs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.vqdsnc.cn/gtpwdjwfsh.html

[Q45] EXISTS 判断存在
来源：http://hz.ehwqpu.com/gtkoeafdhf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtltclqwcs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cqqwz.cn/gtytxoewxt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtzanhosem.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gtesspjezg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.guowangkeji.top/gtisahdwoz.html

[Q48] CTE 公用表表达式
来源：http://hz.zycfv.cn/gtvrnfpwds.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtvwvchixl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.mhx1999.top/gtvttuwsxr.html

[Q49] 更新单行
来源：http://hz.nanxinkj.top/gtketkisnn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtzgcmiick.html

[Q50] 批量更新
来源：http://hz.zycfv.cn/gtmjygijxt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxinkj.top/gtnxkmozrr.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtrgrgqpun.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yonumen.top/gtpvokoljx.html

[Q52] 删除指定行
来源：http://hz.sufxvd.cn/gtupkegyfe.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangdashe.top/gtpbpessuw.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtsgplrtzf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gogol.net.cn/gtwqyuwqlt.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtiomenpre.html

TRUNCATE TABLE logs;
来源：http://hz.feifeiyinyue.top/gtjpnupvoh.html

[Q55] 排名（并列占位）
来源：http://hz.iojbl.cn/gtigpawfjz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.nanxuanxn.top/gtunymoscj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yanxiufei.cn/gtanwhmoqb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shzxlz.cn/gtlvdtkqgy.html

[Q57] 行号
来源：http://hz.sweek.top/gtqyhazmut.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ybcxt.top/gtppifqvvi.html

[Q58] 累计求和
来源：http://hz.fengsongda.top/gtxqgcqdaq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dianchejie.cn/gtzybpamxt.html

[Q59] 分组内累计
来源：http://hz.hfpthk.cn/gtnivdknao.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.xziqi.cn/gtpiuklsus.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gtemkzyxzq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.316326.xyz/gtyqwfflsy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenzaomai.com/gtkbcyzhrl.html

[Q61] 移动平均
来源：http://hz.andypj.xyz/gtorbbszjf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.52xcode.cn/gtflejawyc.html

[Q62] 分组占比
来源：http://hz.guannengcc.top/gtwwhbvhix.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtzqluimmr.html

[Q63] 开启事务
来源：http://hz.tanke756.top/gtigwakygs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tian-w.cn/gttbocbuzw.html

[Q64] 提交事务
来源：http://hz.zhaomingkeji.xyz/gtcbmqdrld.html

COMMIT;
来源：http://hz.chenzaomai.com/gtrkzsouhu.html

[Q65] 回滚事务
来源：http://hz.xziqi.cn/gtxmxuokgn.html

ROLLBACK;
来源：http://hz.shanyushiyangtech.top/gtvxsseczq.html

[Q66] 行锁查询
来源：http://hz.shangyingyoupin.top/gtusaufpdt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yueranfly.top/gtluxhtswc.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtueogqwnu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.snrcjt.cn/gtxppifwxw.html

[Q68] 保存点
来源：http://hz.zhongyouzk.top/gtseowbsdt.html

SAVEPOINT sp1;
来源：http://hz.tanke756.top/gtnwprwlqx.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtyvatchtr.html

[Q69] 查看执行计划
来源：http://hz.wangdashe.top/gtjgummdnu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.vqdsnc.cn/gtxoontekg.html

[Q70] 更新统计信息
来源：http://hz.chenzaomai.com/gtxvpaaizo.html

ANALYZE TABLE users;
来源：http://hz.andypj.xyz/gtyukxurpr.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtvkjbwcye.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.andypj.xyz/gtkjarndel.html

[Q72] 查看索引
来源：http://hz.yuxming.cn/gtzylkzkpz.html

SHOW INDEX FROM users;
来源：http://hz.wangdashe.top/gtmtyhudtt.html

[Q73] 查看表状态
来源：http://hz.jinghuilouyu.cn/gtsxidoqrq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daria6918.cn/gtwecfmhul.html

[Q74] 强制使用索引
来源：http://hz.bjfxy.top/gtahlxbuph.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtdcdyahxq.html

[Q75] 日期格式化
来源：http://hz.316326.xyz/gtbvopiiqf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sufxvd.cn/gtqrnsmxqa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgfzy.top/gttptfczwg.html

[Q76] 按天统计
来源：http://hz.wangdashe.top/gtclidezfq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daria6918.cn/gtjihplvno.html

[Q77] 时间加减
来源：http://hz.jyoumei.cn/gtjntcycuf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenzaomai.com/gtildpjmjm.html

[Q78] 当前时间
来源：http://hz.ivvv.top/gtvtmdnmoj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtovgylcnq.html

[Q79] 字符串拼接
来源：http://hz.jiagoushi.top/gtwfzmvlev.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dianchejie.cn/gttwiyujjl.html

[Q80] 字符串截取
来源：http://hz.ppjwa.cn/gtakwlzfce.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtpweymojl.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtjnejvpmn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tianlin.xyz/gtmbfykkor.html


<!-- 参考信息 -->