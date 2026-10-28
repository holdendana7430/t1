代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.guowangkeji.top/gtiuwrmfew.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtzxstnjbu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.feifeiyinyue.top/gtnvfowfog.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtmrmiqjqj.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigufen.top/gtjpcndmvh.html

Go:   go f()
来源：http://hz.xuetiantiany.cn/gtabhkmohu.html

Ruby: Thread.new { f }
来源：http://hz.fzhhl.top/gtszcxrbww.html

C#:   Task.Run(() => F());
来源：http://hz.yonumen.top/gthxiamoii.html

[O02] 使用线程池
来源：http://hz.cqqwz.cn/gtrdaarjah.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhongyouzk.top/gtnowqdboi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jianghu66.top/gttrntdymk.html

JS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtmnhyhkqi.html

TS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gtwapeffpf.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.52xcode.cn/gtdqdextuf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yueranfly.top/gtobtntzyt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cashguo.top/gtumlotpfr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtireuoibp.html

[O03] 加锁保护共享数据
来源：http://hz.cdnleiting.top/gterbwapup.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtfihgxpne.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtpnigyuez.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fzhhl.top/gtnnkgnzyd.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtewdeukfo.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxinkj.top/gtqqxiciif.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtsubeapjz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sxryk.cn/gtsmcfsuhs.html

C#:   lock (gate) { shared++; }
来源：http://hz.jlsjyb.cn/gtvpzicvow.html

[O04] 定义异步函数并等待
来源：http://hz.52xcode.cn/gteskqyzeq.html

Py:   async def f():⏎    await g()
来源：http://hz.fengsongda.top/gtrgaragyd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.bjfxy.top/gtagrgsqzs.html

JS:   async function f() { await g(); }
来源：http://hz.hfpthk.cn/gtgyunqakg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gtfratydso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.smart0.xyz/gthixstzvg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.iojbl.cn/gtgzpfhwky.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gtqdshtsqi.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gthhsttuow.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinyuanbaomall.cn/gtdyakdiuu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shuidangran.top/gtqiqsczuf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtkbwmrhkv.html

JS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtcrnphjky.html

TS:   await Promise.all(tasks)
来源：http://hz.havefunace.top/gtpuzpajhs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.kuanghao11.cn/gtvoibdzqq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dashuyun.cn/gtrkudetbm.html

Ruby: threads.map(&:join)
来源：http://hz.cqqwz.cn/gtuwqzhkup.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.c1oappe.top/gteiauszhp.html

[O06] 使用进程池
来源：http://hz.zdqjudy.top/gtwtfqppay.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gtidkmyksn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtvsxbavgj.html

JS:   // child_process / cluster 模块
来源：http://hz.yuxming.cn/gtczgqufal.html

TS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtbernofsx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yonumen.top/gtediktdgz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.daxiang520.top/gteyjcpwir.html

Ruby: // fork 块
来源：http://hz.wangdashe.top/gtldxrbdxu.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtvwyfqynp.html

================================================================================
来源：http://hz.jqgfzy.top/gtuqtixyat.html

P. 常用工具函数
来源：http://hz.sxryk.cn/gtahggvfjq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfkfrjzns.html

[P01] 生成 UUID
来源：http://hz.wangdashe.top/gtbfbgooaj.html

Py:   str(uuid.uuid4())
来源：http://hz.yj20258.top/gtqudikmcl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ybcxt.top/gtmbhrsifb.html

JS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtlyedwtcj.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtueqtempz.html

Java: UUID.randomUUID().toString()
来源：http://hz.9152youxi.cn/gtqalpsfdb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhoulong.xyz/gtmzjiubrd.html

Ruby: SecureRandom.uuid
来源：http://hz.yueranfly.top/gtqgednztn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.9152youxi.cn/gtwhgeawsd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guowangkeji.top/gtlzabhbrg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtxfnryfcx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gtdddcwqvr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.guannengcc.top/gtersmrdti.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenzaomai.com/gtpppkarnb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtvpmourot.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhengqikj.top/gtmepcrtvb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.nanxinkj.top/gtmjuotjfr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhiwuduotai.top/gtnscjxzox.html

[P03] 生成短随机字符串
来源：http://hz.cqqwz.cn/gtzqaapwjt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinqigufen.top/gtbxohgsvg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhijiandao.cn/gtbwynkfyd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtgxckrgpq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aizwys.cn/gtfxrnpfbz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xingfuxueyuan.xyz/gtdfgcccdh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.meibo888.top/gtyeausivu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuanzx.com/gtcgkxhovy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.daria6918.cn/gtxwxxsemt.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gtdzxslirl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guowangkeji.top/gtrralzgro.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtpxdthvwi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtwnwpymsv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pycfn.com/gtkzatmcaq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.ydjk.org.cn/gtgfcwssfk.html

Go:   len(arr);  len(m)
来源：http://hz.ybcxt.top/gtkqmvqnkg.html

Ruby: x.length;  x.size
来源：http://hz.sysykeji.top/gtcnzhopzh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tianlin.xyz/gtiaiuxxha.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zhiwuduotai.top/gtlvoevhdw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.ywan-chungtsiang.top/gtlpdxewvx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.sxryk.cn/gtidtsnrqa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.316326.xyz/gtlbberolp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xinyue.icu/gtupuopvqh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.feifeiyinyue.top/gtqnlxlkiy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhoulong.xyz/gtzqqbzewt.html

Ruby: a == b
来源：http://hz.wangshuangyany.cn/gtmhegcowd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.snrcjt.cn/gtdhadyolk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jlsjyb.cn/gtpcscvvir.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.fengsongda.top/gtlzjjecji.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gtoehnxwaj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinyuanbaomall.cn/gteuescqch.html

TS:   if (x == null) {}
来源：http://hz.hongshengwenyu.top/gtzfpgkjww.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.xuanzx.com/gtulnpymhy.html

Go:   if x == nil {}
来源：http://hz.xylfe.cn/gtsmykergm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.sufxvd.cn/gtxfzehkwd.html

C#:   if (x is null) {}
来源：http://hz.shuidangran.top/gtpryxcupa.html

[P07] 防抖与节流
来源：http://hz.jinqigfzy.top/gtcfwuhzbg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gaohongyu789.top/gtymksoqvl.html

PHP:  // 手写时间戳比较
来源：http://hz.sxryk.cn/gtdfrdrnax.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.redwolf501.top/gtmlwzdula.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhiwuduotai.top/gtsczwqvsl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ydzc1.top/gtwfcolrnm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yvedp.cn/gtyvbgkwtd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sweek.top/gtpcmvaerz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.52xcode.cn/gtrvnryljr.html

[P08] 处理浮点精度问题
来源：http://hz.hammf.cn/gtvluypidk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.andypj.xyz/gtukjjyncc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.fzhhl.top/gtiylwyabi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxuanxn.top/gtanhyvmey.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xuetiantiany.cn/gtszwocdpk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shzxlz.cn/gtqyvlvgwj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yangfankeji.com/gtqyodzroj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.smart0.xyz/gttfzyzdns.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.cucudq.cn/gtiszcozkh.html

================================================================================
来源：http://hz.tian-w.cn/gtbjnraepg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cashguo.top/gtkzuyopoj.html

================================================================================
来源：http://hz.yj202588.top/gtovxrqfuo.html

[Q01] 创建表
来源：http://hz.zdqjudy.top/gtdrfuxbwd.html

CREATE TABLE users (
来源：http://hz.cdnleiting.top/gtsgrwdwam.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yongpay.top/gtropzzfks.html

name VARCHAR(50) NOT NULL,
来源：http://hz.chenlongwang.top/gtcuxaudhf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhongyouzk.top/gtdcwfilou.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj20258.top/gtihgdoifl.html

);
来源：http://hz.9152youxi.cn/gtykjqmamd.html

[Q02] 创建带外键的表
来源：http://hz.sysykeji.top/gthcccaqkg.html

CREATE TABLE orders (
来源：http://hz.jinqigufen.top/gtxvfplrvc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtcyyhvpxh.html

user_id INT NOT NULL,
来源：http://hz.guowangkeji.top/gtehfdovmq.html

amount DECIMAL(10, 2),
来源：http://hz.nanxinkj.top/gtwznscfpp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xuetiantiany.cn/gtwektfitd.html

);
来源：http://hz.jqgufenzy.top/gtimgbsdya.html

[Q03] 增加列
来源：http://hz.bjfxy.top/gtjwzdjmol.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yvedp.cn/gtzooxmzti.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtgrrwolwy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.daria6918.cn/gtowzlafje.html

[Q05] 重命名列
来源：http://hz.0kj1m.cn/gtkhbrjgvj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.fzhhl.top/gtndnkhujl.html

[Q06] 删除列
来源：http://hz.shanyushiyangtech.top/gtxruqxvon.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zdqjudy.top/gtxqqluikk.html

[Q07] 删除表
来源：http://hz.guannengcc.top/gtyiwgbdlg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sweek.top/gtxdakmrhw.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtfhouloqb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtoclzvjci.html

[Q09] 创建唯一索引
来源：http://hz.daxiang520.top/gtzsdkvpdp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.snrcjt.cn/gttptrquaw.html

[Q10] 插入单行
来源：http://hz.aibaodan.cn/gtzjnuuzam.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shzxlz.cn/gtobwxdnzr.html

[Q11] 一次插入多行
来源：http://hz.zhiwuduotai.top/gtzcvwdrwa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtjvevdkml.html

[Q12] 插入后取自增 ID
来源：http://hz.52xcode.cn/gtxfobmlto.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yuanzhike.top/gthjeagqwq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuetiantiany.cn/gtytqyvaxv.html

[Q13] 忽略重复插入
来源：http://hz.jqgfzy.top/gtzhwoekym.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.cashguo.top/gtrhusluzg.html

[Q14] 存在则更新（upsert）
来源：http://hz.birdmap.top/gtplowzqse.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhixingplan.top/gtsyoagrws.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.iojbl.cn/gtodhowzqp.html

[Q15] 查询全部
来源：http://hz.birdmap.top/gtgryqnpye.html

SELECT * FROM users;
来源：http://hz.kuanghao11.cn/gtrqwccgvw.html

[Q16] 查询指定列
来源：http://hz.hammf.cn/gtasdnizcw.html

SELECT id, name FROM users;
来源：http://hz.nwbrower.top/gtxitkistl.html

[Q17] 条件查询
来源：http://hz.wangshuangyany.cn/gtpitdkbsc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.guowangkeji.top/gtzuomxksd.html

[Q18] 模糊匹配
来源：http://hz.nanxinkj.top/gtwlvlmldk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gtdyocoxjo.html

[Q19] 范围查询
来源：http://hz.zhoulong.xyz/gtcfjpynji.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dashuyun.cn/gtawrmvdoe.html

[Q20] IN 列表
来源：http://hz.xylfe.cn/gtrcnqllzf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.pengpengdd.cyou/gttukwlmwi.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtwqdzdwws.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jyoumei.cn/gtjqjrlcow.html

[Q22] 排序
来源：http://hz.jiagoushi.top/gtnbtheyhp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenlongwang.top/gtvelngxbz.html

[Q23] 分页
来源：http://hz.hongshengwenyu.top/gtkvzqdyne.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuanzhike.top/gtouyxscsg.html

[Q24] 去重
来源：http://hz.havefunace.top/gtynxtssur.html

SELECT DISTINCT city FROM users;
来源：http://hz.fzhhl.top/gtjzzqjbxk.html

[Q25] 只取前 N 条
来源：http://hz.sufxvd.cn/gtqrgfdmgs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gtnqelifgf.html

[Q26] 计数
来源：http://hz.shangyingyoupin.top/gtbwyeskjq.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj20258888.top/gteujasddg.html

[Q27] 条件计数
来源：http://hz.fzhhl.top/gtkahhyqey.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zycfv.cn/gtcgynsyby.html

[Q28] 求和与平均
来源：http://hz.xuetiantiany.cn/gtrgnhzfvm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shuidangran.top/gtzbmpmixw.html

[Q29] 最大最小值
来源：http://hz.bjfxy.top/gtoyaygbmw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ppjwa.cn/gtvxzjgrzo.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtdmxidhpe.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.havefunace.top/gtotzbftlp.html

[Q31] 分组后过滤
来源：http://hz.zhoulong.xyz/gtcwrrcuco.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guowangkeji.top/gtjuvdjkbi.html

[Q32] 分组拼接字符串
来源：http://hz.yangfankeji.com/gtzapgchdp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtmzqpbitb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cheryme.top/gtyhmhvlrt.html

[Q33] 多列分组
来源：http://hz.ydzc1.top/gtzwolgufd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtgozyqpaj.html

[Q34] 每组取第一条
来源：http://hz.yonumen.top/gtbkuphhuc.html

SELECT * FROM (
来源：http://hz.cdnleiting.top/gtpwiddqec.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.hammf.cn/gtgpxbwoma.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtjxhmkbhl.html

[Q35] 内连接
来源：http://hz.daxiang520.top/gtkcpywruf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtqneyiyiu.html

[Q36] 左连接
来源：http://hz.guannengcc.top/gtxvaobfym.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuetiantiany.cn/gtxhbpvyym.html

[Q37] 右连接
来源：http://hz.jinyuanbaomall.cn/gtcfdxhyfe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gtmfhhhqqn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ppjwa.cn/gtpexglssh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.smart0.xyz/gtijrfflaa.html

[Q39] 自连接（查上下级）
来源：http://hz.hnxiangtu.top/gtwhlfwzty.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtcwfzpxyb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nanxinkj.top/gtrxzhyjwd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuetiantiany.cn/gtehobnsye.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yanxiufei.cn/gtewnbvlem.html

[Q41] 多表连接
来源：http://hz.ybcxt.top/gtbhyldrba.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.9152youxi.cn/gtrszjzzjo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.quarkkingdee.top/gtfxsrnhvg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.havefunace.top/gtqvllhncq.html

[Q42] 连接条件附加过滤
来源：http://hz.feifeiyinyue.top/gtgqrzdczo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yueranfly.top/gtnbgnlzwq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtmnbygocl.html

[Q43] 标量子查询
来源：http://hz.mhx1999.top/gthyajhbsx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shanyushiyangtech.top/gtdoevxuwz.html

[Q44] IN 子查询
来源：http://hz.cashguo.top/gtlusjpdhw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gzhubu.top/gtzibjdfjs.html

[Q45] EXISTS 判断存在
来源：http://hz.hnqzz.top/gtpeqtnjpd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenjidiqi.icu/gtwjjuudyp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gtlzfkuqfr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cqqwz.cn/gtpkwjjqqp.html

[Q47] 与平均值比较
来源：http://hz.ivvv.top/gtsdmsfoqz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yonumen.top/gthtizkapp.html

[Q48] CTE 公用表表达式
来源：http://hz.52xcode.cn/gtzgfcksag.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gtwqqnvssi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yongpay.top/gtjowvebgt.html

[Q49] 更新单行
来源：http://hz.sweek.top/gtokcrprzy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtupfmmlob.html

[Q50] 批量更新
来源：http://hz.guowangkeji.top/gtlohchgmd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258.top/gtpcgpvevb.html

[Q51] 用子查询更新
来源：http://hz.zhengqikj.top/gtiixctahr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.feifeiyinyue.top/gtyombxsgv.html

[Q52] 删除指定行
来源：http://hz.ywan-chungtsiang.top/gtsznnitlk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shangyingyoupin.top/gtpwwucdnc.html

[Q53] 按条件删除
来源：http://hz.jinqigfzy.top/gtmozhfbxd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.c1oappe.top/gtpdrglfoy.html

[Q54] 清空表
来源：http://hz.gogol.net.cn/gtlootfral.html

TRUNCATE TABLE logs;
来源：http://hz.ppjwa.cn/gtvtgpscvt.html

[Q55] 排名（并列占位）
来源：http://hz.feifeiyinyue.top/gtqifgpctv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ybcxt.top/gthokupflq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.aibaodan.cn/gtlunxrigy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jlsjyb.cn/gtnoemqetc.html

[Q57] 行号
来源：http://hz.xylfe.cn/gtnviabyex.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yangfankeji.com/gtbjxrbvza.html

[Q58] 累计求和
来源：http://hz.aibaodan.cn/gtxsndukex.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ehwqpu.com/gtmzplqlmm.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtnpazvzki.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.quarkkingdee.top/gtsvzfbiby.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtogbrtshh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daxiang520.top/gtbnrhrvhp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aibaodan.cn/gtnmraxtjr.html

[Q61] 移动平均
来源：http://hz.c1oappe.top/gtvxfocfdb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuanzx.com/gtrfpbhkyq.html

[Q62] 分组占比
来源：http://hz.svipenyu.cn/gtkcvchoxr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtqhhcsnhx.html

[Q63] 开启事务
来源：http://hz.jyoumei.cn/gtfmideajn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shanyushiyangtech.top/gtxcgkkvqk.html

[Q64] 提交事务
来源：http://hz.wangdashe.top/gtqvkvjafg.html

COMMIT;
来源：http://hz.mhx1999.top/gtewhpdjvs.html

[Q65] 回滚事务
来源：http://hz.hnxiangtu.top/gtflxdkqmb.html

ROLLBACK;
来源：http://hz.yuxming.cn/gtcuuchpeh.html

[Q66] 行锁查询
来源：http://hz.jqgufenzy.top/gthagaqbrr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aibaodan.cn/gtjjvqhqrs.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtiggtpvwh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuanzx.com/gtschuidom.html

[Q68] 保存点
来源：http://hz.cqqwz.cn/gtmzqskcks.html

SAVEPOINT sp1;
来源：http://hz.haohaochexian.top/gtdgppuzrn.html

ROLLBACK TO sp1;
来源：http://hz.cheryme.top/gtyjfjfktr.html

[Q69] 查看执行计划
来源：http://hz.gzhubu.top/gtodxinkho.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sysykeji.top/gtgballift.html

[Q70] 更新统计信息
来源：http://hz.feifeiyinyue.top/gtrjjqroin.html

ANALYZE TABLE users;
来源：http://hz.xylfe.cn/gthuhfxtoy.html

[Q71] 查看建表语句
来源：http://hz.nwbrower.top/gtqdtehgsj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aibaodan.cn/gtseqhsggh.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gthciamnkk.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtgmtjfenz.html

[Q73] 查看表状态
来源：http://hz.ivvv.top/gtaypmfinx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gotoacloud.top/gtpasqyacs.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtipswbvho.html


<!-- 参考信息 -->