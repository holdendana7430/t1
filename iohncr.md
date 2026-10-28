代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://hz.ivvv.top/gtapelssyo.html

Go:   go f()
来源：http://hz.yuxming.cn/gteumyhcxy.html

Ruby: Thread.new { f }
来源：http://hz.guannengcc.top/gtgsjuahrv.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtciucbrza.html

[O02] 使用线程池
来源：http://hz.aizwys.cn/gtnryezpuv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gtmqhmjcvi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aizwys.cn/gtbfnclkqo.html

JS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtxvvqtuui.html

TS:   // worker_threads 线程池
来源：http://hz.hongshengwenyu.top/gtfgndpinv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tianlin.xyz/gtbxltseov.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.havefunace.top/gtpodfayms.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtslkobnwm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gtuumefjir.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtwnepiguk.html

Py:   with lock: shared += 1
来源：http://hz.wangdashe.top/gtpbzoaald.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj202588.top/gtzefqfqvr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.316326.xyz/gtawrrmpwk.html

TS:   // 同 JS
来源：http://hz.cdnleiting.top/gtlnwrsprw.html

Java: synchronized (this) { shared++; }
来源：http://hz.yangfankeji.com/gthhsodhgy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.wangdashe.top/gternzisgw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nanxuanxn.top/gtqgexhler.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxuanxn.top/gtqmwksykq.html

[O04] 定义异步函数并等待
来源：http://hz.wangdashe.top/gtdvxwdbzo.html

Py:   async def f():⏎    await g()
来源：http://hz.hongshengwenyu.top/gtressutrt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhaomingkeji.xyz/gtugnmcuek.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gtqgbunkdm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangshuangyany.cn/gtaibaforg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.haohaochexian.top/gtfvuxielk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtqddvpvcx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenzaomai.com/gthkamrckb.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxinkj.top/gtdvergebl.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinghuilouyu.cn/gtgripyzlt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yueranfly.top/gtxsascatr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.316326.xyz/gtxxlbgfvo.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtrofslgne.html

TS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtfbtcxxpz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zdqjudy.top/gtybpgfixb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtkjidaaqy.html

Ruby: threads.map(&:join)
来源：http://hz.ybcxt.top/gtpiljxlyx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yangfankeji.com/gtkhviudev.html

[O06] 使用进程池
来源：http://hz.iojbl.cn/gtjuzylert.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yanxiufei.cn/gtqllalofk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxuanxn.top/gtgtpvdrln.html

JS:   // child_process / cluster 模块
来源：http://hz.c1oappe.top/gtjvtmrlmb.html

TS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gthqfajvax.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ydjk.org.cn/gtggrgqtrj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigufen.top/gtyiheidtn.html

Ruby: // fork 块
来源：http://hz.yonumen.top/gthzvyyjou.html

C#:   Parallel.For
来源：http://hz.chenjidiqi.icu/gtyvkdxept.html

================================================================================
来源：http://hz.jiagoushi.top/gtjaznkokc.html

P. 常用工具函数
来源：http://hz.zhaomingkeji.xyz/gtxxgqlzbx.html

================================================================================
来源：http://hz.zhixingplan.top/gtjmooxjpj.html

[P01] 生成 UUID
来源：http://hz.hfpthk.cn/gtrhnerlne.html

Py:   str(uuid.uuid4())
来源：http://hz.bjfxy.top/gtierctuvb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hywenlv.cn/gtxkddvhxz.html

JS:   crypto.randomUUID()
来源：http://hz.snrcjt.cn/gtvbxdecul.html

TS:   crypto.randomUUID()
来源：http://hz.daxiang520.top/gtmertsntc.html

Java: UUID.randomUUID().toString()
来源：http://hz.aizwys.cn/gtjwrulbdo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hfpthk.cn/gtyxdqnzdl.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigufen.top/gtarnladbu.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.316326.xyz/gtrdsypgfb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.birdmap.top/gtpxyohtdz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangdashe.top/gtcdrxzent.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtkkkcffqs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gtpusidrmd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.daria6918.cn/gtgvtouihx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.fzhhl.top/gtukulvjfi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj202588.top/gtcpbzktop.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.iojbl.cn/gtfaaesqok.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cdnleiting.top/gtozwicmma.html

[P03] 生成短随机字符串
来源：http://hz.vqdsnc.cn/gtblmebxav.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgfzy.top/gtudjmdonm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yueranfly.top/gtodmmdstr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.meibo888.top/gtbhnllrna.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gthropycra.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ybcxt.top/gtrziubdhk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.hammf.cn/gtdgsrscxo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgufenzy.top/gtdxduxhvo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zycfv.cn/gtngzdcecl.html

[P04] 求长度
来源：http://hz.tanke756.top/gtqqxtphtw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtvbibbowt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtyosudncr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtiffjrugb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtjdmvfwdt.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigfzy.top/gtefajpkhx.html

Go:   len(arr);  len(m)
来源：http://hz.yj20258.top/gtuvtcvuol.html

Ruby: x.length;  x.size
来源：http://hz.svipenyu.cn/gtdxielopg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtrkypxsfm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yj202588.top/gtpdsdddow.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sysykeji.top/gtdvokhehs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sufxvd.cn/gtfdpzkxvk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zdqjudy.top/gtdnlcglqq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtyqympurb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xinyue.icu/gtqazdijyu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jianghu66.top/gtqqmwmkij.html

Ruby: a == b
来源：http://hz.cheryme.top/gtepuhjzud.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ybcxt.top/gtcohrhcnb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.redwolf501.top/gturlztckc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jqgfzy.top/gthcckrcdj.html

PHP:  if (empty($x)) {}
来源：http://hz.hysaishi.cn/gtiedrsbii.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnxiangtu.top/gtqtmnvnys.html

TS:   if (x == null) {}
来源：http://hz.guannengcc.top/gtwmsdtnzk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtluvjlfcr.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtdeippndp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.tian-w.cn/gtdwgsneyv.html

C#:   if (x is null) {}
来源：http://hz.sxryk.cn/gtmpaibpuf.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtefgyskwm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.nwbrower.top/gterlwveel.html

PHP:  // 手写时间戳比较
来源：http://hz.jinyuanbaomall.cn/gtyopvtlny.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nanxuanxn.top/gtodranudc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtpacdtwvs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhijiandao.cn/gttimfsxph.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.nanxinkj.top/gtmwnkumso.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.snrcjt.cn/gtwelskwnd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shzxlz.cn/gtopcslcqx.html

[P08] 处理浮点精度问题
来源：http://hz.52xcode.cn/gtvucphicu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sysykeji.top/gtrrrexsux.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.mhx1999.top/gtyuilunri.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.ywan-chungtsiang.top/gttpwqhcoa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtmnhzqwrg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.bjfxy.top/gtdtxnguaz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.havefunace.top/gtvrtzbshd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xingfuxueyuan.xyz/gtxtvlbtqf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.aizwys.cn/gttxogdyat.html

================================================================================
来源：http://hz.vqdsnc.cn/gttjaxaedq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.quarkkingdee.top/gtbowymlae.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbvrdhhsx.html

[Q01] 创建表
来源：http://hz.hfpthk.cn/gtycrgpvos.html

CREATE TABLE users (
来源：http://hz.aibaodan.cn/gtepxskqtn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtzufflyrc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hongshengwenyu.top/gtvqjuwjxi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuanzhike.top/gtaubmvkou.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenjidiqi.icu/gtghugfsdg.html

);
来源：http://hz.shuidangran.top/gtgbhmisgy.html

[Q02] 创建带外键的表
来源：http://hz.chenlongwang.top/gtjrnguiwl.html

CREATE TABLE orders (
来源：http://hz.dianchejie.cn/gtbrpcgzpk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtabfhojnx.html

user_id INT NOT NULL,
来源：http://hz.meibo888.top/gttgzgsthh.html

amount DECIMAL(10, 2),
来源：http://hz.shzxlz.cn/gtecyftzhj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.52xcode.cn/gtjwgghjpm.html

);
来源：http://hz.xylfe.cn/gtncrlylsc.html

[Q03] 增加列
来源：http://hz.guannengcc.top/gtqxiscjmy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hysaishi.cn/gtbqjzapop.html

[Q04] 修改列类型
来源：http://hz.yueranfly.top/gtyefwifkp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hnqzz.top/gtfolthzrh.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtqwrwblnt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fzhhl.top/gtenamxjkp.html

[Q06] 删除列
来源：http://hz.hnxiangtu.top/gtwwptptii.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.bjfxy.top/gtkiqetiix.html

[Q07] 删除表
来源：http://hz.cucudq.cn/gtivkptpmx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.svipenyu.cn/gtboxtdcuq.html

[Q08] 创建普通索引
来源：http://hz.yj20258888.top/gtphkdcwgo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.fengsongda.top/gtzsduqqci.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtrseopatr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtkosgzwwr.html

[Q10] 插入单行
来源：http://hz.316326.xyz/gtcelzjmmr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.gotoacloud.top/gtmhavrhld.html

[Q11] 一次插入多行
来源：http://hz.xziqi.cn/gtmotpaerf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.daxiang520.top/gtitxriphb.html

[Q12] 插入后取自增 ID
来源：http://hz.iojbl.cn/gttleksnmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.shzxlz.cn/gtspczbvtc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guowangkeji.top/gtcpwidfza.html

[Q13] 忽略重复插入
来源：http://hz.pengpengdd.cyou/gtdqxridxs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.redwolf501.top/gtsgvohfuf.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnqzz.top/gtomopljgn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guannengcc.top/gtttxruhpf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.aibaodan.cn/gtmqiauvlz.html

[Q15] 查询全部
来源：http://hz.jiagoushi.top/gtraqqlcam.html

SELECT * FROM users;
来源：http://hz.zhongyouzk.top/gtgvlhsupt.html

[Q16] 查询指定列
来源：http://hz.dianchejie.cn/gtoghoesfr.html

SELECT id, name FROM users;
来源：http://hz.aibaodan.cn/gthdnxhqqf.html

[Q17] 条件查询
来源：http://hz.quarkkingdee.top/gtbnhcrrfl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.smart0.xyz/gtcboqamiw.html

[Q18] 模糊匹配
来源：http://hz.zhijiandao.cn/gtqfthgsvt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.tianlin.xyz/gtqzhootue.html

[Q19] 范围查询
来源：http://hz.jiagoushi.top/gtjxzhownz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sufxvd.cn/gtrilbhudi.html

[Q20] IN 列表
来源：http://hz.cucudq.cn/gtgtuwhggr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yongpay.top/gttrcgsbiz.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtrkouztdy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tian-w.cn/gtdrzhwcxe.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtetwehlgv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hysaishi.cn/gtovkybdio.html

[Q23] 分页
来源：http://hz.svipenyu.cn/gtcjoaiohq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ehwqpu.com/gtaijqmdse.html

[Q24] 去重
来源：http://hz.gzhubu.top/gtyxrplysz.html

SELECT DISTINCT city FROM users;
来源：http://hz.tian-w.cn/gtotdkspxh.html

[Q25] 只取前 N 条
来源：http://hz.9152youxi.cn/gtrdxvudhb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gtzwpxohzz.html

[Q26] 计数
来源：http://hz.xylfe.cn/gtaukxrgyc.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgfzy.top/gtzxhnutxv.html

[Q27] 条件计数
来源：http://hz.yuanzhike.top/gtmsxsmocv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yuxming.cn/gtwmwjhxnh.html

[Q28] 求和与平均
来源：http://hz.tianlin.xyz/gtfouszqzp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtrwkrnqod.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtxjufxgmq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gtpdrxblcm.html

[Q30] 分组统计
来源：http://hz.yanxiufei.cn/gtrqnjdknm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtbdtkcouu.html

[Q31] 分组后过滤
来源：http://hz.yuxming.cn/gtxhiqyozn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shuidangran.top/gtheyfdkrz.html

[Q32] 分组拼接字符串
来源：http://hz.xuetiantiany.cn/gtplvdhidt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtqgbawmot.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shuidangran.top/gtkvxvgtrb.html

[Q33] 多列分组
来源：http://hz.jqgfzy.top/gtdwuqujcy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nwbrower.top/gtappfnypz.html

[Q34] 每组取第一条
来源：http://hz.yj20258888.top/gthyeinfhq.html

SELECT * FROM (
来源：http://hz.zhijiandao.cn/gtbcjjsftu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cqqwz.cn/gthiloxwua.html

) t WHERE rn = 1;
来源：http://hz.iojbl.cn/gtvrulokru.html

[Q35] 内连接
来源：http://hz.meibo888.top/gtscqncruy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuxming.cn/gtxmikuslr.html

[Q36] 左连接
来源：http://hz.xylfe.cn/gtzlfpsgde.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.0kj1m.cn/gtixxhpbbn.html

[Q37] 右连接
来源：http://hz.dianchejie.cn/gtylhcncch.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.kuanghao11.cn/gtvxrdnclt.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtmzfyafdh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.vqdsnc.cn/gtsdfootzx.html

[Q39] 自连接（查上下级）
来源：http://hz.quarkkingdee.top/gteoemvugw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtxadtjvrj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtlgkdgkqe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shuidangran.top/gthhmetqqm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sufxvd.cn/gtemzhufhf.html

[Q41] 多表连接
来源：http://hz.hfpthk.cn/gtouovrwlh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuanzhike.top/gtnkvzpegb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydjk.org.cn/gtewsmbgne.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yueranfly.top/gtwesayksq.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtgjhpihap.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pycfn.com/gtuiwnjaek.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gthlkuwccd.html

[Q43] 标量子查询
来源：http://hz.birdmap.top/gtzkyehuuv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.redwolf501.top/gtyvwimbvm.html

[Q44] IN 子查询
来源：http://hz.52xcode.cn/gtcwtloqzp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtauwzuqfc.html

[Q45] EXISTS 判断存在
来源：http://hz.yonumen.top/gtfdtfdwxk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtjaqbflum.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.quarkkingdee.top/gtzicgnsfs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hysaishi.cn/gtdnfmckqg.html

[Q47] 与平均值比较
来源：http://hz.c1oappe.top/gtqendgxxk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ywan-chungtsiang.top/gtxrmpmjlj.html

[Q48] CTE 公用表表达式
来源：http://hz.jinyuanbaomall.cn/gtwboqfdot.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cucudq.cn/gtdrlmxizo.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gttwnowzgb.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtatzdtpgj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtshflbaln.html

[Q50] 批量更新
来源：http://hz.svipenyu.cn/gtidlhzcms.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gtavaoymar.html

[Q51] 用子查询更新
来源：http://hz.ybcxt.top/gtochxipvg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.52xcode.cn/gtdtxpcees.html

[Q52] 删除指定行
来源：http://hz.wangshuangyany.cn/gtqeyummuy.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cdnleiting.top/gtzgdurrmp.html

[Q53] 按条件删除
来源：http://hz.yvedp.cn/gthhfnpsku.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gtqfecgxfd.html

[Q54] 清空表
来源：http://hz.yongpay.top/gtalwoaitc.html

TRUNCATE TABLE logs;
来源：http://hz.kuanghao11.cn/gtqgvaoohs.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gtlkhcxyql.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tanke756.top/gtvrivnujg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yangfankeji.com/gtdjxrzvwu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gtawgoyfet.html

[Q57] 行号
来源：http://hz.316326.xyz/gtqonlfhio.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jiagoushi.top/gtqxvqbmqm.html

[Q58] 累计求和
来源：http://hz.ydzc1.top/gtlcfevgen.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxuanxn.top/gtplwhxjnp.html

[Q59] 分组内累计
来源：http://hz.fzhhl.top/gtddpsofrn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtondwnocw.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gttgjcdyjm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnqzz.top/gtprpsrbva.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtbuhzzldj.html

[Q61] 移动平均
来源：http://hz.shzxlz.cn/gtkkixmhpf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jyoumei.cn/gtyuxvbnux.html

[Q62] 分组占比
来源：http://hz.nanxinkj.top/gtpumnksha.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ehwqpu.com/gtcpwailly.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtspxoizjw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtrfmzuwvj.html

[Q64] 提交事务
来源：http://hz.pycfn.com/gtxgleupem.html

COMMIT;
来源：http://hz.zdqjudy.top/gtynxshunx.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtuhbfcxgw.html

ROLLBACK;
来源：http://hz.yangfankeji.com/gtltdmsqzx.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtzizdwbgn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj202588.top/gtowhbvcnb.html

[Q67] 设置隔离级别
来源：http://hz.gaohongyu789.top/gteuafnxgd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sxryk.cn/gtqgvoomev.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gtjenzvjyw.html

SAVEPOINT sp1;
来源：http://hz.zhaomingkeji.xyz/gtdqpwquye.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtzwxkhjxl.html

[Q69] 查看执行计划
来源：http://hz.kuanghao11.cn/gtajumjlge.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sufxvd.cn/gthtwmvrdm.html

[Q70] 更新统计信息
来源：http://hz.yvedp.cn/gtdrluudcp.html

ANALYZE TABLE users;
来源：http://hz.jinyuanbaomall.cn/gtzqgnssuh.html

[Q71] 查看建表语句
来源：http://hz.hysaishi.cn/gtclkvznow.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.9152youxi.cn/gtjaddzmby.html

[Q72] 查看索引
来源：http://hz.zhengqikj.top/gtkwajpmdo.html

SHOW INDEX FROM users;
来源：http://hz.yvedp.cn/gtypuhwqii.html

[Q73] 查看表状态
来源：http://hz.zhixingplan.top/gtpxhyszfu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sweek.top/gtbaxowkgb.html

[Q74] 强制使用索引
来源：http://hz.cqqwz.cn/gteowcysyk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxinkj.top/gtiycdqbfn.html

[Q75] 日期格式化
来源：http://hz.yanxiufei.cn/gtahktbqzr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hfpthk.cn/gtjsfrdbuz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhoulong.xyz/gtjjbjobug.html


<!-- 参考信息 -->