代发 wailian999

[O02] 使用线程池
来源：http://hz.yueranfly.top/gtuiudlzqj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jianghu66.top/gtutcnvmjy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jlsjyb.cn/gtenagwhbr.html

JS:   // worker_threads 线程池
来源：http://hz.yongpay.top/gtfhgtbdod.html

TS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtktocvgvl.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtropirwgw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cashguo.top/gtveluufxr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.snrcjt.cn/gthecauhrn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guannengcc.top/gtappauwjs.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtzdmtyfah.html

Py:   with lock: shared += 1
来源：http://hz.ivvv.top/gtbiqzyttb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gtccudtpbm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtwovgfhvp.html

TS:   // 同 JS
来源：http://hz.hfpthk.cn/gtnmgfsrth.html

Java: synchronized (this) { shared++; }
来源：http://hz.andypj.xyz/gtwulceryk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jianghu66.top/gtzyklobaa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hysaishi.cn/gtujgktsmu.html

C#:   lock (gate) { shared++; }
来源：http://hz.ehwqpu.com/gtuhurigtd.html

[O04] 定义异步函数并等待
来源：http://hz.jinqigufen.top/gtggvouvfi.html

Py:   async def f():⏎    await g()
来源：http://hz.zdqjudy.top/gttfcvajud.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtxkocbuby.html

JS:   async function f() { await g(); }
来源：http://hz.xuetiantiany.cn/gtsdfshlrg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.c1oappe.top/gtiaradbdo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pycfn.com/gtsxcrdlgm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.havefunace.top/gttxtfwimj.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cdnleiting.top/gtoyhnfkay.html

C#:   async Task F() { await G(); }
来源：http://hz.guowangkeji.top/gtscdpiuqe.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenlongwang.top/gtpbedznpm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.haohaochexian.top/gtqsvndyss.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gthwcjhgla.html

JS:   await Promise.all(tasks)
来源：http://hz.ywan-chungtsiang.top/gtpryydoid.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtkgyxqkal.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.smart0.xyz/gtrihyvwfq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ppjwa.cn/gtcngcebof.html

Ruby: threads.map(&:join)
来源：http://hz.xylfe.cn/gtjnvuftdz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gturnfmzjv.html

[O06] 使用进程池
来源：http://hz.zycfv.cn/gtrwzsbgrp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtdrsfbqar.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aizwys.cn/gtbytycvtk.html

JS:   // child_process / cluster 模块
来源：http://hz.snrcjt.cn/gtspzcfzvd.html

TS:   // child_process / cluster 模块
来源：http://hz.jinqigufen.top/gthyftmwlm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangshuangyany.cn/gtjhheapyq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydjk.org.cn/gtylkpcjmh.html

Ruby: // fork 块
来源：http://hz.ywan-chungtsiang.top/gtrkdfkwci.html

C#:   Parallel.For
来源：http://hz.yueranfly.top/gtfdklliqe.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvozwpxkc.html

P. 常用工具函数
来源：http://hz.hfpthk.cn/gtxkvlmleo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbvgtnnxy.html

[P01] 生成 UUID
来源：http://hz.jinqigufen.top/gtfmpjjpow.html

Py:   str(uuid.uuid4())
来源：http://hz.haohaochexian.top/gtxttpipcb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.meibo888.top/gtrgfpetca.html

JS:   crypto.randomUUID()
来源：http://hz.redwolf501.top/gtsjflrwso.html

TS:   crypto.randomUUID()
来源：http://hz.pengpengdd.cyou/gtzqxinjdh.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtcnuwcjjv.html

Go:   // 用 github.com/google/uuid
来源：http://hz.fzhhl.top/gtstmrryaf.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gthwtmwprr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinqigfzy.top/gtsccpowka.html

[P02] MD5 / SHA256 摘要
来源：http://hz.feifeiyinyue.top/gtxymabfto.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhongyouzk.top/gtyaqiiskg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daria6918.cn/gtrbknaezb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.feifeiyinyue.top/gtqmghptqh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gotoacloud.top/gthpnqpnfr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gtgqddkuee.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hfpthk.cn/gtidmsmbbm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangdashe.top/gtldvdhqit.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cucudq.cn/gtdbgixgtk.html

[P03] 生成短随机字符串
来源：http://hz.dianchejie.cn/gtousopbcq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yanxiufei.cn/gtwdyjsnba.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangtech.top/gtymndqoge.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtjfbeictg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtmpzpfomz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuxming.cn/gtmazugcnc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cdnleiting.top/gtdcehzsfj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gotoacloud.top/gtjqteiacb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.9152youxi.cn/gtquyjbwmm.html

[P04] 求长度
来源：http://hz.cashguo.top/gtvnjjglpi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nwbrower.top/gthjxtcwwn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtmtlybaep.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xziqi.cn/gtvbdeopld.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gzhubu.top/gtgeguyill.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gzhubu.top/gtesgiajqr.html

Go:   len(arr);  len(m)
来源：http://hz.xuanzx.com/gthmgwhqli.html

Ruby: x.length;  x.size
来源：http://hz.ppjwa.cn/gtzqhzneda.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuanzhike.top/gtnappikoo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jinyuanbaomall.cn/gtkkijtham.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yangfankeji.com/gtcdchiehk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shangyingyoupin.top/gtatwkwxmr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.shuidangran.top/gtprkbxnma.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtibzssbuy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hnxiangtu.top/gttzgmjgul.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuanzx.com/gtxltqyhxf.html

Ruby: a == b
来源：http://hz.tanke756.top/gtjspyqniy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daxiang520.top/gtqovyhrlz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jianghu66.top/gtypdglerj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.birdmap.top/gtaindvcnr.html

PHP:  if (empty($x)) {}
来源：http://hz.snrcjt.cn/gtcakytacf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.pycfn.com/gtaksdphdr.html

TS:   if (x == null) {}
来源：http://hz.ppjwa.cn/gtsazguwxu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtnicceihv.html

Go:   if x == nil {}
来源：http://hz.andypj.xyz/gttcdufxal.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hnxiangtu.top/gtsqpczyjp.html

C#:   if (x is null) {}
来源：http://hz.cheryme.top/gtsulzdzth.html

[P07] 防抖与节流
来源：http://hz.hnxiangtu.top/gtclajiaxt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yanxiufei.cn/gtusoqcrdc.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtwdxadgaj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shzxlz.cn/gtqqdkhvgg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtwtpvjahn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fengsongda.top/gtgqpnllug.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.andypj.xyz/gtupocubbg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hongshengwenyu.top/gtfcivpjmn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xylfe.cn/gtutgjwbeu.html

[P08] 处理浮点精度问题
来源：http://hz.cheryme.top/gtsgibocoi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jiagoushi.top/gtrwatwowp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ybcxt.top/gtgcmsioqh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yuanzhike.top/gtarvmrnft.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtvoekpukq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.0kj1m.cn/gtemdixdwl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.xingfuxueyuan.xyz/gtxifywhaq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhengqikj.top/gtpawnmpty.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.xylfe.cn/gtturidoqo.html

================================================================================
来源：http://hz.cashguo.top/gttgnwuhxs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.birdmap.top/gtnplbistz.html

================================================================================
来源：http://hz.daria6918.cn/gtiewyzbak.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gtxridvptb.html

CREATE TABLE users (
来源：http://hz.yj20258.top/gtqvpnksth.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.snrcjt.cn/gtjcxcaqfz.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yvedp.cn/gtxmijqndb.html

email VARCHAR(100) UNIQUE,
来源：http://hz.mhx1999.top/gtmdbwnbwx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.316326.xyz/gtxnkvrhpo.html

);
来源：http://hz.pengpengdd.cyou/gtanuxrlhu.html

[Q02] 创建带外键的表
来源：http://hz.hongshengwenyu.top/gthlbgzhnv.html

CREATE TABLE orders (
来源：http://hz.haohaochexian.top/gtrlrpcsis.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.redwolf501.top/gtdudxuuan.html

user_id INT NOT NULL,
来源：http://hz.ydzc1.top/gtsefdkgnm.html

amount DECIMAL(10, 2),
来源：http://hz.birdmap.top/gtvpzpajjf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hfpthk.cn/gtpbcaqber.html

);
来源：http://hz.zdqjudy.top/gtlkeeyprx.html

[Q03] 增加列
来源：http://hz.yvedp.cn/gtwohkndri.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ydjk.org.cn/gtbcqqauds.html

[Q04] 修改列类型
来源：http://hz.tianlin.xyz/gtsjcvrimk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.chenlongwang.top/gttlvadjsw.html

[Q05] 重命名列
来源：http://hz.daria6918.cn/gthydtmdmh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258888.top/gtybdobvzw.html

[Q06] 删除列
来源：http://hz.ywan-chungtsiang.top/gtqpgpamtb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.snrcjt.cn/gtrapgpcpg.html

[Q07] 删除表
来源：http://hz.c1oappe.top/gtixcjlsgs.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jyoumei.cn/gtsqurswer.html

[Q08] 创建普通索引
来源：http://hz.tianlin.xyz/gtgfppupor.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtfquupwea.html

[Q09] 创建唯一索引
来源：http://hz.shuidangran.top/gtgcualqqh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.tian-w.cn/gtlbzngzbd.html

[Q10] 插入单行
来源：http://hz.nwbrower.top/gtfmismmyn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.andypj.xyz/gtllqvegvv.html

[Q11] 一次插入多行
来源：http://hz.sysykeji.top/gtnuenbwzm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.mhx1999.top/gtczvyyxhr.html

[Q12] 插入后取自增 ID
来源：http://hz.cheryme.top/gtnhsvihlc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gtulhmmipk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtbjagebbu.html

[Q13] 忽略重复插入
来源：http://hz.kuanghao11.cn/gtjjddpihk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xuanzx.com/gtbkttyaso.html

[Q14] 存在则更新（upsert）
来源：http://hz.cheryme.top/gttohgkfjs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtupacizhn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.iojbl.cn/gtsackgnnw.html

[Q15] 查询全部
来源：http://hz.xuanzx.com/gtlwdccadw.html

SELECT * FROM users;
来源：http://hz.yongpay.top/gtlonahnjp.html

[Q16] 查询指定列
来源：http://hz.xuetiantiany.cn/gtznvnouly.html

SELECT id, name FROM users;
来源：http://hz.cqqwz.cn/gtbnobpwlh.html

[Q17] 条件查询
来源：http://hz.hnxiangtu.top/gtekoerosa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yangfankeji.com/gtqvsqelkm.html

[Q18] 模糊匹配
来源：http://hz.tanke756.top/gtdmzunnyk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zdqjudy.top/gthkknpwjl.html

[Q19] 范围查询
来源：http://hz.andypj.xyz/gtppyknxot.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhijiandao.cn/gtnjidodfv.html

[Q20] IN 列表
来源：http://hz.smart0.xyz/gtuzanbvty.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenzaomai.com/gtjlsnguaj.html

[Q21] 空值判断
来源：http://hz.wangdashe.top/gtilvobiix.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtyppzcbkf.html

[Q22] 排序
来源：http://hz.hongshengwenyu.top/gtjjqagtyu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jinqigfzy.top/gtcwmhtobz.html

[Q23] 分页
来源：http://hz.vqdsnc.cn/gtgqjxequm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yanxiufei.cn/gtnvxvcpen.html

[Q24] 去重
来源：http://hz.hysaishi.cn/gtccvddfbc.html

SELECT DISTINCT city FROM users;
来源：http://hz.cashguo.top/gtfjcxgltr.html

[Q25] 只取前 N 条
来源：http://hz.jinqigfzy.top/gtavjtregr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxuanxn.top/gtgsjrpxws.html

[Q26] 计数
来源：http://hz.tianlin.xyz/gtofxkhciw.html

SELECT COUNT(*) FROM users;
来源：http://hz.smart0.xyz/gthvmwtxtl.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtuyoevnyg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gtngtqdpcg.html

[Q28] 求和与平均
来源：http://hz.zdqjudy.top/gtunucaedk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jyoumei.cn/gtbcidvunv.html

[Q29] 最大最小值
来源：http://hz.316326.xyz/gtcyniiqjw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.guannengcc.top/gtkjulixpu.html

[Q30] 分组统计
来源：http://hz.shuidangran.top/gtmuzwatuh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtxrsupypj.html

[Q31] 分组后过滤
来源：http://hz.yj20258888.top/gtidpkpfil.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gthzwyixnn.html

[Q32] 分组拼接字符串
来源：http://hz.gogol.net.cn/gtoiczzbes.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtacdswcnl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hammf.cn/gtcosxafpz.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtnmcaepdb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yanxiufei.cn/gtxcqvtgaj.html

[Q34] 每组取第一条
来源：http://hz.52xcode.cn/gtuzueioen.html

SELECT * FROM (
来源：http://hz.meibo888.top/gtsysxtovy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sufxvd.cn/gtyymwbcuu.html

) t WHERE rn = 1;
来源：http://hz.dashuyun.cn/gtezelhbiu.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtcbqwytvq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtusrvthim.html

[Q36] 左连接
来源：http://hz.shuidangran.top/gtzrsdcmqe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.shuidangran.top/gtjgsdnypb.html

[Q37] 右连接
来源：http://hz.snrcjt.cn/gtvjctelyz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hammf.cn/gtdvaieqqs.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtpesparyp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yanxiufei.cn/gtfolyxwbn.html

[Q39] 自连接（查上下级）
来源：http://hz.xylfe.cn/gtncvgacgb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangdashe.top/gtehfgjidc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yanxiufei.cn/gtoyfdojnw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gtgjvbkvyy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtjyhsevgx.html

[Q41] 多表连接
来源：http://hz.cqqwz.cn/gtmtwrhtma.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hammf.cn/gtsuodyoet.html

JOIN users u ON u.id = o.user_id
来源：http://hz.guowangkeji.top/gtgnifywsn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.quarkkingdee.top/gtkpvetgdd.html

[Q42] 连接条件附加过滤
来源：http://hz.ydzc1.top/gtxadmbhpj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cashguo.top/gtepszjamm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtbcdnbenq.html

[Q43] 标量子查询
来源：http://hz.fengsongda.top/gtbnrqjspg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gtvlizitqp.html

[Q44] IN 子查询
来源：http://hz.redwolf501.top/gtftkszhmy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yanxiufei.cn/gtfzbmnyac.html

[Q45] EXISTS 判断存在
来源：http://hz.andypj.xyz/gtzmwxdnrr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hongshengwenyu.top/gtawbfbfko.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gtqmlnowho.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtlyrusnxh.html

[Q47] 与平均值比较
来源：http://hz.jiagoushi.top/gtlwrcejcg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.andypj.xyz/gtyyzpsftv.html

[Q48] CTE 公用表表达式
来源：http://hz.chenzaomai.com/gtcfrpqnbq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.pengpengdd.cyou/gtdtrnvyzx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gaohongyu789.top/gtetkadfvg.html

[Q49] 更新单行
来源：http://hz.nanxuanxn.top/gtvraxavet.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.havefunace.top/gtavbbipkt.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtxvfrmiqb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhaomingkeji.xyz/gtewlaqkao.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gtupjnoyhy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cucudq.cn/gtjdnuncvd.html

[Q52] 删除指定行
来源：http://hz.yongpay.top/gtzsrpqcnn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sxryk.cn/gtvxfiswzt.html

[Q53] 按条件删除
来源：http://hz.sufxvd.cn/gtnbwaczuv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jiagoushi.top/gtsxfuprui.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtgdwgwfjb.html

TRUNCATE TABLE logs;
来源：http://hz.jianghu66.top/gtkkgaxyin.html

[Q55] 排名（并列占位）
来源：http://hz.zhengqikj.top/gtfhdibwzz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yvedp.cn/gtswxpmfzq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuanzx.com/gtszgapoaj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtoquzanjz.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtxiktmgyd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shangyingyoupin.top/gtodhwoksq.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtqkosxuvh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.fengsongda.top/gtjfdvjmlx.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gtmpwvihml.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yvedp.cn/gtplbzgspj.html

[Q60] 取上一行 / 下一行
来源：http://hz.pengpengdd.cyou/gtvkgcqjvt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.guannengcc.top/gtjsnxdykj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenzaomai.com/gtnbjhvjpx.html

[Q61] 移动平均
来源：http://hz.yongpay.top/gtvdrxcszn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtmjeymiyx.html

[Q62] 分组占比
来源：http://hz.hnqzz.top/gtetpcialq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtebildjsl.html

[Q63] 开启事务
来源：http://hz.cqqwz.cn/gttdkvathd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cashguo.top/gtqamqpohj.html

[Q64] 提交事务
来源：http://hz.sufxvd.cn/gtmhjqiuta.html

COMMIT;
来源：http://hz.gzhubu.top/gtonxxqwqt.html

[Q65] 回滚事务
来源：http://hz.ydzc1.top/gtcuchyvnk.html

ROLLBACK;
来源：http://hz.yanxiufei.cn/gthebrtrps.html

[Q66] 行锁查询
来源：http://hz.xuetiantiany.cn/gtzvwsgrie.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhengqikj.top/gtdbjgvyuz.html

[Q67] 设置隔离级别
来源：http://hz.yj20258.top/gtunorzfpi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.birdmap.top/gtskyrilup.html

[Q68] 保存点
来源：http://hz.yj202588.top/gtejqkvzcg.html

SAVEPOINT sp1;
来源：http://hz.ehwqpu.com/gtszyrgsav.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gtlratallw.html

[Q69] 查看执行计划
来源：http://hz.gotoacloud.top/gtbtjoqhxd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhengqikj.top/gtwicbjboj.html

[Q70] 更新统计信息
来源：http://hz.gogol.net.cn/gtugelrgry.html

ANALYZE TABLE users;
来源：http://hz.316326.xyz/gthjjmywfw.html

[Q71] 查看建表语句
来源：http://hz.smart0.xyz/gtwkkiamwg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.guannengcc.top/gtkwoxlzld.html

[Q72] 查看索引
来源：http://hz.ehwqpu.com/gtyrltveum.html

SHOW INDEX FROM users;
来源：http://hz.hnqzz.top/gtvrxeudio.html

[Q73] 查看表状态
来源：http://hz.andypj.xyz/gtqnyylmwm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258888.top/gtkpujlbah.html

[Q74] 强制使用索引
来源：http://hz.tian-w.cn/gtuarhgjtf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xylfe.cn/gtzbfflesp.html

[Q75] 日期格式化
来源：http://hz.yj20258.top/gtislrtnlu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangdashe.top/gtxawoenig.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cashguo.top/gtdogjlkry.html

[Q76] 按天统计
来源：http://hz.jqgufenzy.top/gtsblfirck.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cdnleiting.top/gthkzaqonj.html

[Q77] 时间加减
来源：http://hz.aizwys.cn/gtdbwdivfl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daria6918.cn/gttubrbabg.html


<!-- 参考信息 -->