代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://hz.iojbl.cn/gtvtaxpvws.html

Go:   go f()
来源：http://hz.yuxming.cn/gtfmfportv.html

Ruby: Thread.new { f }
来源：http://hz.ybcxt.top/gtjfmmhszy.html

C#:   Task.Run(() => F());
来源：http://hz.jianghu66.top/gtuepqvpfv.html

[O02] 使用线程池
来源：http://hz.bjfxy.top/gtwsoxiyxm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yangfankeji.com/gtxrouliij.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinghuilouyu.cn/gtwrudjppm.html

JS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtdngsapcc.html

TS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtpbnyxlyr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.pycfn.com/gthdjkagxs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.redwolf501.top/gtbhlgvkpp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.haohaochexian.top/gtcmnxbkik.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.nanxuanxn.top/gtpiqqbudj.html

[O03] 加锁保护共享数据
来源：http://hz.xuetiantiany.cn/gtoevcxlqv.html

Py:   with lock: shared += 1
来源：http://hz.zhoulong.xyz/gtdlbeeehs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.52xcode.cn/gtvffpqnpv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jiagoushi.top/gthrgrppip.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtayfmlokt.html

Java: synchronized (this) { shared++; }
来源：http://hz.haohaochexian.top/gtcegnadvt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fengsongda.top/gterbqepqe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtsnahmxuk.html

C#:   lock (gate) { shared++; }
来源：http://hz.havefunace.top/gtbxmjsgcj.html

[O04] 定义异步函数并等待
来源：http://hz.zhengqikj.top/gtxesfqqem.html

Py:   async def f():⏎    await g()
来源：http://hz.aibaodan.cn/gthveuemor.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gogol.net.cn/gtyglfango.html

JS:   async function f() { await g(); }
来源：http://hz.yonumen.top/gttgqprmvx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gtmhfhnbzn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydzc1.top/gtxzkszxwl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.andypj.xyz/gtjrgwynit.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yuxming.cn/gtlhhdeqvg.html

C#:   async Task F() { await G(); }
来源：http://hz.yj202588.top/gtxavhjwnl.html

[O05] 并发执行并等待全部完成
来源：http://hz.gzhubu.top/gtzkrzkxtz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtsbordpdc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zdqjudy.top/gtfjpodfpa.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtykfsdthj.html

TS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtyvbexzad.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.daxiang520.top/gtizrxkqrv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.bjfxy.top/gtbtobrzyw.html

Ruby: threads.map(&:join)
来源：http://hz.sysykeji.top/gtfruwfgsn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.pengpengdd.cyou/gtqwyicoxn.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtogwzragw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangdashe.top/gttoflmtby.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.havefunace.top/gtehmcarly.html

JS:   // child_process / cluster 模块
来源：http://hz.c1oappe.top/gtfcaknpjw.html

TS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtydzjigje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sxryk.cn/gtfktfzrqi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xuetiantiany.cn/gttqztqbkl.html

Ruby: // fork 块
来源：http://hz.shzxlz.cn/gtlnfbdsww.html

C#:   Parallel.For
来源：http://hz.jqgfzy.top/gtmplxmptl.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxshjfuba.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtsnzqvnxz.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkgscsvgf.html

[P01] 生成 UUID
来源：http://hz.sufxvd.cn/gtliqoaxdd.html

Py:   str(uuid.uuid4())
来源：http://hz.fengsongda.top/gttrdaisbs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.andypj.xyz/gtvmlwtktp.html

JS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtpaqqwmps.html

TS:   crypto.randomUUID()
来源：http://hz.hfpthk.cn/gtefwbphwm.html

Java: UUID.randomUUID().toString()
来源：http://hz.dashuyun.cn/gtubmvzkbu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zdqjudy.top/gtndayqfve.html

Ruby: SecureRandom.uuid
来源：http://hz.pycfn.com/gtgdsqyaxv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jyoumei.cn/gtuqyrzftq.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gzhubu.top/gtncerumcd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinghuilouyu.cn/gtcdslpusk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gogol.net.cn/gtactnzayy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.chenlongwang.top/gtopqnwywr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jlsjyb.cn/gtztupwmsy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.52xcode.cn/gtjzfnktrc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shuidangran.top/gtmkloivki.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daria6918.cn/gthbsvbiss.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.haohaochexian.top/gtbivdzdrl.html

[P03] 生成短随机字符串
来源：http://hz.iojbl.cn/gtnjirnywj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jyoumei.cn/gtusriento.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.vqdsnc.cn/gtzeafveql.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jianghu66.top/gtixoswboi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tanke756.top/gtrsfhggfm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shanyushiyangkeji.top/gtbmxdelzn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.wangdashe.top/gtaduboszi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhaomingkeji.xyz/gtwgypudta.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxinkj.top/gtpisszuma.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtlzxtnukp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shanyushiyangkeji.top/gtmiqalsrg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtwgbqnvhq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jqgufenzy.top/gtwemhzcmw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj20258888.top/gtskjrqaho.html

Java: list.size();  map.size();  s.length()
来源：http://hz.pengpengdd.cyou/gtdvbeqyhl.html

Go:   len(arr);  len(m)
来源：http://hz.316326.xyz/gthidpotpv.html

Ruby: x.length;  x.size
来源：http://hz.ydjk.org.cn/gtzjntyxqa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.chenzaomai.com/gtepdfqihb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.0kj1m.cn/gtzaytasmo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258.top/gtebowvays.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangshuangyany.cn/gthqvacacb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.gogol.net.cn/gtpqbenauj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhongyouzk.top/gtnjesqgnj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.aibaodan.cn/gtvmivjbrl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daxiang520.top/gtqcrumwwl.html

Ruby: a == b
来源：http://hz.cqqwz.cn/gtgowrzjll.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.nwbrower.top/gtmciugvxt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yuanzhike.top/gtldyeicwk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinghuilouyu.cn/gtwfbzpacc.html

PHP:  if (empty($x)) {}
来源：http://hz.yonumen.top/gtjqxoxqjr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tian-w.cn/gtqtnqsnyu.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtebcezfje.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pycfn.com/gtpjhzbtlq.html

Go:   if x == nil {}
来源：http://hz.jianghu66.top/gtemkjtqpt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jiagoushi.top/gtztvsjuyo.html

C#:   if (x is null) {}
来源：http://hz.chenlongwang.top/gtkispewjm.html

[P07] 防抖与节流
来源：http://hz.wangdashe.top/gtlyjrfedj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.kuanghao11.cn/gtsfvnyvwm.html

PHP:  // 手写时间戳比较
来源：http://hz.ydjk.org.cn/gttgndrlbz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.quarkkingdee.top/gtzoawhqqw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuanzx.com/gtqttgezyo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zycfv.cn/gteozsbdcg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.0kj1m.cn/gtcwjawbuy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuetiantiany.cn/gtclzzfspj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.dianchejie.cn/gtcphyywbl.html

[P08] 处理浮点精度问题
来源：http://hz.chenjidiqi.icu/gtqjjcetjb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.meibo888.top/gtnqugnhxi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sysykeji.top/gtpdfbsyjj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gteypmvvud.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ivvv.top/gtblrlgdij.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.iojbl.cn/gtqjcdzcpe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinghuilouyu.cn/gtcvusxufh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhixingplan.top/gtaeydypav.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yonumen.top/gtcawvnpiq.html

================================================================================
来源：http://hz.zdqjudy.top/gtxwktwbfk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ivvv.top/gtwgqsnjmu.html

================================================================================
来源：http://hz.yvedp.cn/gtpnmdzjpn.html

[Q01] 创建表
来源：http://hz.yangfankeji.com/gtfieaagye.html

CREATE TABLE users (
来源：http://hz.ybcxt.top/gtdaenjgwk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gtekydtdgm.html

name VARCHAR(50) NOT NULL,
来源：http://hz.zdqjudy.top/gtzbzsrcdt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cashguo.top/gtbhikwril.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnqzz.top/gtpmzxkglx.html

);
来源：http://hz.yongpay.top/gtlvkghqxz.html

[Q02] 创建带外键的表
来源：http://hz.ydjk.org.cn/gtmsdilnvp.html

CREATE TABLE orders (
来源：http://hz.hongshengwenyu.top/gtzrpratyl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daxiang520.top/gtocplqfbi.html

user_id INT NOT NULL,
来源：http://hz.shzxlz.cn/gtnlnycdra.html

amount DECIMAL(10, 2),
来源：http://hz.yuanzhike.top/gtssgwqpdp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinqigfzy.top/gttymepgkp.html

);
来源：http://hz.jinqigfzy.top/gtxzuyeekk.html

[Q03] 增加列
来源：http://hz.pycfn.com/gtzmsffwov.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtolgswbxg.html

[Q04] 修改列类型
来源：http://hz.316326.xyz/gtecctatdn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.tian-w.cn/gtijrhrvxl.html

[Q05] 重命名列
来源：http://hz.nwbrower.top/gtuaopaqau.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhaomingkeji.xyz/gtyqnhxmhx.html

[Q06] 删除列
来源：http://hz.yonumen.top/gtzxisvzin.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtmlbflsai.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtxuiihsjo.html

DROP TABLE IF EXISTS orders;
来源：http://hz.52xcode.cn/gtwwstvmkv.html

[Q08] 创建普通索引
来源：http://hz.wangshuangyany.cn/gtoshrhcji.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtaeqallhh.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gtcrarsmsu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.c1oappe.top/gtadyabafp.html

[Q10] 插入单行
来源：http://hz.ywan-chungtsiang.top/gtmrrlcudk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangkeji.top/gtxmiczqsq.html

[Q11] 一次插入多行
来源：http://hz.xingfuxueyuan.xyz/gtxarfkcbl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jlsjyb.cn/gtultrrdrz.html

[Q12] 插入后取自增 ID
来源：http://hz.wangshuangyany.cn/gtudmuiplg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xziqi.cn/gtkbskiffn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ybcxt.top/gtbfcsosup.html

[Q13] 忽略重复插入
来源：http://hz.hnxiangtu.top/gteoojkrqp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.fzhhl.top/gtcmwsqcoh.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtftrpwzpf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ppjwa.cn/gtxcbctxmo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.guannengcc.top/gtgeobqjor.html

[Q15] 查询全部
来源：http://hz.0kj1m.cn/gtxsyatcrn.html

SELECT * FROM users;
来源：http://hz.zhaomingkeji.xyz/gtibtnolbk.html

[Q16] 查询指定列
来源：http://hz.wangdashe.top/gtbswmotmx.html

SELECT id, name FROM users;
来源：http://hz.vqdsnc.cn/gtiksfhbqg.html

[Q17] 条件查询
来源：http://hz.tanke756.top/gttayrkssg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinghuilouyu.cn/gtiwogxqjy.html

[Q18] 模糊匹配
来源：http://hz.cashguo.top/gtjpkrhmdu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.bjfxy.top/gtzdolijjg.html

[Q19] 范围查询
来源：http://hz.ppjwa.cn/gtacjrxajp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dashuyun.cn/gttpinmhoq.html

[Q20] IN 列表
来源：http://hz.shanyushiyangkeji.top/gtheekthyb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gthcrprrjl.html

[Q21] 空值判断
来源：http://hz.shzxlz.cn/gtjskmodex.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.sysykeji.top/gtljieiwpm.html

[Q22] 排序
来源：http://hz.xylfe.cn/gtvrzygkoy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.pycfn.com/gtofrkbkod.html

[Q23] 分页
来源：http://hz.hnxiangtu.top/gtcsyvybfl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.wangdashe.top/gtmcfevugu.html

[Q24] 去重
来源：http://hz.guowangkeji.top/gtylzizizb.html

SELECT DISTINCT city FROM users;
来源：http://hz.shuidangran.top/gtlcjfpcuf.html

[Q25] 只取前 N 条
来源：http://hz.jinqigufen.top/gtqpikbjah.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtoaujvtgt.html

[Q26] 计数
来源：http://hz.sxryk.cn/gthrvjasaa.html

SELECT COUNT(*) FROM users;
来源：http://hz.shangyingyoupin.top/gttrphbqzq.html

[Q27] 条件计数
来源：http://hz.hammf.cn/gtkhocnedb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.havefunace.top/gtbfluypdg.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtggaebrke.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtryquxoyh.html

[Q29] 最大最小值
来源：http://hz.ybcxt.top/gtepmnmlgb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gtfdapkvvc.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtjxafuvqp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtksqwkvmw.html

[Q31] 分组后过滤
来源：http://hz.kuanghao11.cn/gttkyzdfzn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tianlin.xyz/gtcalheygp.html

[Q32] 分组拼接字符串
来源：http://hz.ehwqpu.com/gtrbvanrve.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtdjpcvsrm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258888.top/gtviebvxou.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtstjixnqa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxuanxn.top/gtavntpnvh.html

[Q34] 每组取第一条
来源：http://hz.zhixingplan.top/gtmrrjhfms.html

SELECT * FROM (
来源：http://hz.bjfxy.top/gtnjehhcel.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yvedp.cn/gtynwcaqnd.html

) t WHERE rn = 1;
来源：http://hz.kuanghao11.cn/gtilofmsfc.html

[Q35] 内连接
来源：http://hz.chenjidiqi.icu/gtzivyiofd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.pycfn.com/gtidhwxpbq.html

[Q36] 左连接
来源：http://hz.ybcxt.top/gtgpaorubz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gtxsgiodnt.html

[Q37] 右连接
来源：http://hz.xuetiantiany.cn/gtxreowtez.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ehwqpu.com/gtvdluiplz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hnxiangtu.top/gtebhqdjhe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yonumen.top/gtqvncqbxk.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtzsjgaute.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.wangshuangyany.cn/gtxmyjjqqv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sufxvd.cn/gttmcrnlyr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yueranfly.top/gtijtgugqc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yongpay.top/gtrzhwazfm.html

[Q41] 多表连接
来源：http://hz.dashuyun.cn/gtdpcjskvv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.daria6918.cn/gtxwvdnwtx.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yonumen.top/gtxjimdmcv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shzxlz.cn/gttovbnqur.html

[Q42] 连接条件附加过滤
来源：http://hz.xingfuxueyuan.xyz/gtulsgcgoh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shzxlz.cn/gtaltecuco.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.pycfn.com/gtnolovvbo.html

[Q43] 标量子查询
来源：http://hz.birdmap.top/gtlzaqbjxv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtibulkdek.html

[Q44] IN 子查询
来源：http://hz.yongpay.top/gtyidiemop.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhongyouzk.top/gtanxshzms.html

[Q45] EXISTS 判断存在
来源：http://hz.snrcjt.cn/gtcbrvtuxe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtzrxdwufn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jlsjyb.cn/gtyjhmydtf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtowcuxqdo.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gtbaveabvz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenzaomai.com/gtsbkoarfg.html

[Q48] CTE 公用表表达式
来源：http://hz.316326.xyz/gtrrgbzldf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtqmfqvgek.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pengpengdd.cyou/gtjgdlwmjf.html

[Q49] 更新单行
来源：http://hz.andypj.xyz/gtkuecpmrc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.0kj1m.cn/gtevvddfpk.html

[Q50] 批量更新
来源：http://hz.pycfn.com/gtwraxyenm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.haohaochexian.top/gtexnwjccg.html

[Q51] 用子查询更新
来源：http://hz.kuanghao11.cn/gtnmlfismu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuxming.cn/gtbqabrutw.html

[Q52] 删除指定行
来源：http://hz.cdnleiting.top/gttiucvenl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtjnlpeeeg.html

[Q53] 按条件删除
来源：http://hz.shuidangran.top/gtwqkkbtia.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinqigfzy.top/gtdgjswtbq.html

[Q54] 清空表
来源：http://hz.dashuyun.cn/gtvyndvnxx.html

TRUNCATE TABLE logs;
来源：http://hz.xuanzx.com/gtwyelroeg.html

[Q55] 排名（并列占位）
来源：http://hz.ybcxt.top/gtanbrvevf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gteuvamwxl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhijiandao.cn/gtzybrcvgg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fzhhl.top/gthobirfva.html

[Q57] 行号
来源：http://hz.jlsjyb.cn/gttexktgia.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigufen.top/gthbdwzzlz.html

[Q58] 累计求和
来源：http://hz.yangfankeji.com/gtabfzgdbx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yvedp.cn/gtwztpqcyz.html

[Q59] 分组内累计
来源：http://hz.shzxlz.cn/gtisuvzkov.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hywenlv.cn/gtjjwywxrj.html

[Q60] 取上一行 / 下一行
来源：http://hz.shzxlz.cn/gtphyymhhn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.meibo888.top/gtsebrskzk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtzouojphd.html

[Q61] 移动平均
来源：http://hz.snrcjt.cn/gtnovsgbqk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gteulkgpng.html

[Q62] 分组占比
来源：http://hz.gogol.net.cn/gtyfbfhkrf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtvnllnvgd.html

[Q63] 开启事务
来源：http://hz.sweek.top/gtfefxzktz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.aibaodan.cn/gtxsrkpfsg.html

[Q64] 提交事务
来源：http://hz.gogol.net.cn/gtvwnwiepf.html

COMMIT;
来源：http://hz.jlsjyb.cn/gtjrvyhgjz.html

[Q65] 回滚事务
来源：http://hz.cqqwz.cn/gtzuxdbypp.html

ROLLBACK;
来源：http://hz.yuanzhike.top/gtmwkmzlvg.html

[Q66] 行锁查询
来源：http://hz.yuxming.cn/gtstnttyra.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yuanzhike.top/gtuyfxqrse.html

[Q67] 设置隔离级别
来源：http://hz.9152youxi.cn/gtuymqecao.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hammf.cn/gtscrnkppt.html

[Q68] 保存点
来源：http://hz.gotoacloud.top/gtjsivdwwt.html

SAVEPOINT sp1;
来源：http://hz.cqqwz.cn/gtpcaiqqgy.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtqkucshab.html

[Q69] 查看执行计划
来源：http://hz.9152youxi.cn/gtyrxnoaof.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.316326.xyz/gtayycypeb.html

[Q70] 更新统计信息
来源：http://hz.jqgfzy.top/gtfjvqvvln.html

ANALYZE TABLE users;
来源：http://hz.zhiwuduotai.top/gtpyueesyj.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gttsmploqd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gaohongyu789.top/gtcibgufde.html

[Q72] 查看索引
来源：http://hz.ywan-chungtsiang.top/gtsafdvdaf.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtyfulglqp.html

[Q73] 查看表状态
来源：http://hz.pycfn.com/gtjhzuoyli.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yongpay.top/gthjhqqwro.html

[Q74] 强制使用索引
来源：http://hz.xingfuxueyuan.xyz/gtkexoyvdm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aibaodan.cn/gtsytncvbp.html

[Q75] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gtvgxsjsgv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuanzx.com/gtyuagemjn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sxryk.cn/gtjqwrpztf.html


<!-- 参考信息 -->