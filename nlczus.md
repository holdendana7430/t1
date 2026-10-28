代发 wailian999

[O02] 使用线程池
来源：http://hz.shanyushiyangtech.top/gtoaweqyhe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhiwuduotai.top/gttccuqhcp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtgyhuahyk.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gticfbffux.html

TS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtefkrlveo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hnxiangtu.top/gtpemxnfin.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jianghu66.top/gtrtmnnzco.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.havefunace.top/gtkmllohqv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.tanke756.top/gtggnghori.html

[O03] 加锁保护共享数据
来源：http://hz.dashuyun.cn/gtonznpffv.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtcnmaaeyd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hysaishi.cn/gtssininbr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jqgufenzy.top/gtrkpsyhuq.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtegmprnsk.html

Java: synchronized (this) { shared++; }
来源：http://hz.tian-w.cn/gtuzjstgqs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhongyouzk.top/gtbjscbcrt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tanke756.top/gtwvymgwme.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtpusijqpm.html

[O04] 定义异步函数并等待
来源：http://hz.hammf.cn/gtyounmhee.html

Py:   async def f():⏎    await g()
来源：http://hz.yongpay.top/gtahehvpqv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangtech.top/gtqpkipqrj.html

JS:   async function f() { await g(); }
来源：http://hz.sxryk.cn/gtsdbdtljx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhongyouzk.top/gtbpftgvlx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenjidiqi.icu/gtojbekojs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtfkcdbuni.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yj20258.top/gtmxyiuzok.html

C#:   async Task F() { await G(); }
来源：http://hz.guannengcc.top/gtuzucweva.html

[O05] 并发执行并等待全部完成
来源：http://hz.havefunace.top/gtgjwkzitc.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jinghuilouyu.cn/gthcoytqil.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtmpguzsjl.html

JS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtkdbjgfhh.html

TS:   await Promise.all(tasks)
来源：http://hz.gaohongyu789.top/gtskzhxqms.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.kuanghao11.cn/gtabbqofkv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gthulhtqhq.html

Ruby: threads.map(&:join)
来源：http://hz.zdqjudy.top/gtlliwnivp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.c1oappe.top/gtfcpshehy.html

[O06] 使用进程池
来源：http://hz.sweek.top/gtbjmfdhkh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gtvegtqoyd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangshuangyany.cn/gtruxucvks.html

JS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtcpaadiij.html

TS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gteflvtnzo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtoyyductu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gotoacloud.top/gtjrlxizjg.html

Ruby: // fork 块
来源：http://hz.hnxiangtu.top/gtzwrieets.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtbprprqqp.html

================================================================================
来源：http://hz.hnxiangtu.top/gtpuqygtrf.html

P. 常用工具函数
来源：http://hz.jyoumei.cn/gtiowdkqno.html

================================================================================
来源：http://hz.zhijiandao.cn/gttpxtolnn.html

[P01] 生成 UUID
来源：http://hz.52xcode.cn/gtmythfkjn.html

Py:   str(uuid.uuid4())
来源：http://hz.yuxming.cn/gtkbtcahnd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hnqzz.top/gtudculmkv.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtcwcppkgx.html

TS:   crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gteugdyepw.html

Java: UUID.randomUUID().toString()
来源：http://hz.yangfankeji.com/gttdyzltdl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shzxlz.cn/gtyupfkcwe.html

Ruby: SecureRandom.uuid
来源：http://hz.c1oappe.top/gttnkyzxxl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.birdmap.top/gtpoiqynba.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtwarbpuee.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zycfv.cn/gtadfrxgmm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xziqi.cn/gtzycsljtl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.316326.xyz/gtkdwblpwx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jqgfzy.top/gtujihefrw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jlsjyb.cn/gtxluoufuy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.havefunace.top/gtrmlaoame.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.zhengqikj.top/gtscgtwibe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guowangkeji.top/gtjrrsznay.html

[P03] 生成短随机字符串
来源：http://hz.shanyushiyangtech.top/gthmjwihyl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tanke756.top/gtxldmptvo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jinyuanbaomall.cn/gtujsuznyg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtnuwjrkjk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gzhubu.top/gtnxjnxypq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.9152youxi.cn/gtnbfirydv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhongyouzk.top/gtwnhxlobu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yj20258.top/gticziaiar.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.bjfxy.top/gtkhcjfnek.html

[P04] 求长度
来源：http://hz.aizwys.cn/gtwujhmcym.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtqubjhnos.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtiytozoux.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gtjdqizanm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.9152youxi.cn/gtpolbzxdj.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtqjfcezky.html

Go:   len(arr);  len(m)
来源：http://hz.aibaodan.cn/gtwzxlxllu.html

Ruby: x.length;  x.size
来源：http://hz.zhoulong.xyz/gtxplybkzj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jqgufenzy.top/gtdoyduldo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xuetiantiany.cn/gtelbgxjba.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hywenlv.cn/gtqvrseshc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxinkj.top/gtiafmgacz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtgsryjhrq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ybcxt.top/gtukifrxxp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fengsongda.top/gtvwblbmyv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinqigfzy.top/gtevqayjvi.html

Ruby: a == b
来源：http://hz.daria6918.cn/gtlywbyxfl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.ppjwa.cn/gtgpwqipev.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fengsongda.top/gthjtztjgd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sweek.top/gtpsomtqne.html

PHP:  if (empty($x)) {}
来源：http://hz.xziqi.cn/gtlmyqtnem.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sxryk.cn/gtikkbwlse.html

TS:   if (x == null) {}
来源：http://hz.wangdashe.top/gtxbrjojlz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtolywagtm.html

Go:   if x == nil {}
来源：http://hz.wangdashe.top/gtdsuigipc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxinkj.top/gtnikylcko.html

C#:   if (x is null) {}
来源：http://hz.jianghu66.top/gtnfvxjosu.html

[P07] 防抖与节流
来源：http://hz.dashuyun.cn/gtdzufgaqj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yvedp.cn/gtymxsripw.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtzjgkeasz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtmqmcfpri.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gtjypzwgkw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shanyushiyangtech.top/gtoqoqnsjs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.dashuyun.cn/gtmysdiizs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.xuanzx.com/gteshzfhkk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xingfuxueyuan.xyz/gtcfgmhmve.html

[P08] 处理浮点精度问题
来源：http://hz.c1oappe.top/gtrisbwciu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.smart0.xyz/gtvxkqqddp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.xylfe.cn/gtqoyemxhu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yj20258.top/gtymmnclmh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.shzxlz.cn/gtycexbomi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.redwolf501.top/gtctjzlwue.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yj20258.top/gtwphqsmew.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.guannengcc.top/gtidxpynrp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinqigufen.top/gtklebotfu.html

================================================================================
来源：http://hz.xinyue.icu/gtufywtbzq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shuidangran.top/gtogijgclr.html

================================================================================
来源：http://hz.xziqi.cn/gtfcuglshk.html

[Q01] 创建表
来源：http://hz.xziqi.cn/gtapcbomyn.html

CREATE TABLE users (
来源：http://hz.yonumen.top/gtarwmrpgc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gotoacloud.top/gtqowdrwcg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtzfqhzkrk.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pengpengdd.cyou/gtzlrcghob.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.tanke756.top/gtvkgxyofx.html

);
来源：http://hz.feifeiyinyue.top/gtalcsawld.html

[Q02] 创建带外键的表
来源：http://hz.cqqwz.cn/gtiddlgump.html

CREATE TABLE orders (
来源：http://hz.tian-w.cn/gtukmmnppp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gtnmkdahfn.html

user_id INT NOT NULL,
来源：http://hz.zhixingplan.top/gtqzsbfowc.html

amount DECIMAL(10, 2),
来源：http://hz.cashguo.top/gtbxlmaipw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj202588.top/gtsbirvgsx.html

);
来源：http://hz.nwbrower.top/gtfmvrmjwt.html

[Q03] 增加列
来源：http://hz.tianlin.xyz/gtyqldrvly.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cucudq.cn/gtsgrjaocl.html

[Q04] 修改列类型
来源：http://hz.ydjk.org.cn/gtteidcmqs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtvfhvenme.html

[Q05] 重命名列
来源：http://hz.cdnleiting.top/gtxblspgxq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cheryme.top/gtdfqfpuhf.html

[Q06] 删除列
来源：http://hz.fzhhl.top/gttviynshx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.pengpengdd.cyou/gtrlrjtthk.html

[Q07] 删除表
来源：http://hz.shangyingyoupin.top/gtqynpusnd.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jinqigfzy.top/gtpgpxdhsm.html

[Q08] 创建普通索引
来源：http://hz.zhixingplan.top/gtvjcaqrvf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hongshengwenyu.top/gtaumqyeid.html

[Q09] 创建唯一索引
来源：http://hz.zhiwuduotai.top/gtqxhwyixn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cdnleiting.top/gtpptntjna.html

[Q10] 插入单行
来源：http://hz.meibo888.top/gttguvdxww.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cucudq.cn/gtsuuzmpqy.html

[Q11] 一次插入多行
来源：http://hz.zhixingplan.top/gtirvwekkq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtybfzypae.html

[Q12] 插入后取自增 ID
来源：http://hz.zycfv.cn/gtlzwjuysa.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.andypj.xyz/gtjcqkkbqg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hnxiangtu.top/gtynywrovo.html

[Q13] 忽略重复插入
来源：http://hz.yj20258.top/gtpwwcoreb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shangyingyoupin.top/gtvjpubkll.html

[Q14] 存在则更新（upsert）
来源：http://hz.yonumen.top/gtpsptvgmv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtckrdpvnr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.wangshuangyany.cn/gtigkecyoz.html

[Q15] 查询全部
来源：http://hz.zhongyouzk.top/gtrjnydidt.html

SELECT * FROM users;
来源：http://hz.aizwys.cn/gtljdvuoca.html

[Q16] 查询指定列
来源：http://hz.cashguo.top/gtfphmopwg.html

SELECT id, name FROM users;
来源：http://hz.yj20258.top/gtxiylzscn.html

[Q17] 条件查询
来源：http://hz.xziqi.cn/gtdqbnhzsc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.cashguo.top/gtpozdqksq.html

[Q18] 模糊匹配
来源：http://hz.316326.xyz/gtwjuofcmu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.9152youxi.cn/gtgalrdclq.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtyfvyjctx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daxiang520.top/gthdxrkdjq.html

[Q20] IN 列表
来源：http://hz.shanyushiyangkeji.top/gtxtirvwuq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.svipenyu.cn/gtgggjzicc.html

[Q21] 空值判断
来源：http://hz.shanyushiyangkeji.top/gtbqlrhuiw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yj20258888.top/gtszuobima.html

[Q22] 排序
来源：http://hz.yonumen.top/gtppachvmo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tianlin.xyz/gtrmerbedp.html

[Q23] 分页
来源：http://hz.sysykeji.top/gtttpjknbz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.kuanghao11.cn/gtrotrxkbt.html

[Q24] 去重
来源：http://hz.yueranfly.top/gtkfxhwyri.html

SELECT DISTINCT city FROM users;
来源：http://hz.xuanzx.com/gtesbrxtbk.html

[Q25] 只取前 N 条
来源：http://hz.guannengcc.top/gtbpxxaibe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258.top/gthjhsnhhl.html

[Q26] 计数
来源：http://hz.xuanzx.com/gtwfhbzkut.html

SELECT COUNT(*) FROM users;
来源：http://hz.haohaochexian.top/gtrkldkfqu.html

[Q27] 条件计数
来源：http://hz.xylfe.cn/gtxocuvqed.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cashguo.top/gtnksygmkl.html

[Q28] 求和与平均
来源：http://hz.yj20258.top/gtqhztwapg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtugjsdcns.html

[Q29] 最大最小值
来源：http://hz.zhiwuduotai.top/gtjbwzymqf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtiwqtmudk.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtmppsqhzj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtmlqpgzrs.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gtiytitcbj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ybcxt.top/gtdzpnfdqf.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtumlpctkj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtoenksgar.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hywenlv.cn/gtsomzaitn.html

[Q33] 多列分组
来源：http://hz.ywan-chungtsiang.top/gtzqjgesci.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hysaishi.cn/gtzduubztv.html

[Q34] 每组取第一条
来源：http://hz.xziqi.cn/gtjebctajx.html

SELECT * FROM (
来源：http://hz.zhiwuduotai.top/gtobesdbyt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sufxvd.cn/gtnxmrftif.html

) t WHERE rn = 1;
来源：http://hz.redwolf501.top/gtxgszjmms.html

[Q35] 内连接
来源：http://hz.cheryme.top/gtunyayhjw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gtucmupkkk.html

[Q36] 左连接
来源：http://hz.yj20258888.top/gtkexgnhcu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jyoumei.cn/gtpmggimoq.html

[Q37] 右连接
来源：http://hz.yonumen.top/gtypaldkyp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gtxtrtanby.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ehwqpu.com/gtdpmjbeen.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xinyue.icu/gtuhlfavdo.html

[Q39] 自连接（查上下级）
来源：http://hz.nwbrower.top/gtdkhmcokk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xinyue.icu/gtzsewfsrl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhixingplan.top/gtszngnyya.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.c1oappe.top/gtyekzsocs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.tanke756.top/gtlvsnxvxb.html

[Q41] 多表连接
来源：http://hz.svipenyu.cn/gtcvpjuqsb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.fzhhl.top/gtnveykbkc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtexwrycps.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtkuslajiz.html

[Q42] 连接条件附加过滤
来源：http://hz.jinyuanbaomall.cn/gtdyzkouso.html

SELECT u.name, o.amount FROM users u
来源：http://hz.redwolf501.top/gtcuawbakm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yongpay.top/gtoqpfwuzx.html

[Q43] 标量子查询
来源：http://hz.quarkkingdee.top/gttxrwkofm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hywenlv.cn/gttxlyhtsp.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtnsjxxhsp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.havefunace.top/gtyzwgqblk.html

[Q45] EXISTS 判断存在
来源：http://hz.sweek.top/gtcwiojnoh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtwfjzcvwj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ybcxt.top/gtvwpgkqtf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtlonswnrc.html

[Q47] 与平均值比较
来源：http://hz.zhongyouzk.top/gtyrdqhtps.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sysykeji.top/gtgsdpuyvb.html

[Q48] CTE 公用表表达式
来源：http://hz.mhx1999.top/gtdbsxjwta.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtcdfvhjzx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtqetotfoc.html

[Q49] 更新单行
来源：http://hz.redwolf501.top/gtjgknkbfp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daria6918.cn/gtmouojumm.html

[Q50] 批量更新
来源：http://hz.aizwys.cn/gtbfhgynsa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.0kj1m.cn/gtvodcvfpn.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gtlcvgxjes.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hammf.cn/gtrbjvmhlg.html

[Q52] 删除指定行
来源：http://hz.tianlin.xyz/gtopxivlhu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtrmmrojlb.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gtiqfzdxix.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinghuilouyu.cn/gtuwrwpkcn.html

[Q54] 清空表
来源：http://hz.ybcxt.top/gthvnluqke.html

TRUNCATE TABLE logs;
来源：http://hz.xuetiantiany.cn/gtnojlnruh.html

[Q55] 排名（并列占位）
来源：http://hz.xingfuxueyuan.xyz/gtdrqkbdga.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinghuilouyu.cn/gtvffamzbw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.52xcode.cn/gthfykmmhf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pengpengdd.cyou/gtufvojmjg.html

[Q57] 行号
来源：http://hz.cheryme.top/gtddodctdc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtuncxtuhe.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtkhmmhlrb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tian-w.cn/gtdgvaenkr.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtbihzbpvv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.meibo888.top/gtklxuunva.html

[Q60] 取上一行 / 下一行
来源：http://hz.tianlin.xyz/gtzzjpoqry.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yuanzhike.top/gtafmtwtgw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yvedp.cn/gtgtwjexrv.html

[Q61] 移动平均
来源：http://hz.chenlongwang.top/gtcwwmdpbs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gotoacloud.top/gtfgnflvuo.html

[Q62] 分组占比
来源：http://hz.yj20258888.top/gtghxertsp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zycfv.cn/gtmrkrciks.html

[Q63] 开启事务
来源：http://hz.hywenlv.cn/gtmgpgfyal.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fengsongda.top/gtmucifljg.html

[Q64] 提交事务
来源：http://hz.0kj1m.cn/gttqkkltjm.html

COMMIT;
来源：http://hz.ivvv.top/gtydzxmzsy.html

[Q65] 回滚事务
来源：http://hz.chenzaomai.com/gtxaesnmpo.html

ROLLBACK;
来源：http://hz.feifeiyinyue.top/gtczeesywe.html

[Q66] 行锁查询
来源：http://hz.quarkkingdee.top/gtwbzzgtna.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.svipenyu.cn/gtzmswnvoc.html

[Q67] 设置隔离级别
来源：http://hz.nanxuanxn.top/gtywnbonxf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tianlin.xyz/gtjwwwyarm.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtqklindyp.html

SAVEPOINT sp1;
来源：http://hz.meibo888.top/gtwpxqcxzv.html

ROLLBACK TO sp1;
来源：http://hz.jinqigfzy.top/gteuqggzcv.html

[Q69] 查看执行计划
来源：http://hz.pengpengdd.cyou/gtlbktjidv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenzaomai.com/gtjyoekkuu.html

[Q70] 更新统计信息
来源：http://hz.wangdashe.top/gthlmyuipn.html

ANALYZE TABLE users;
来源：http://hz.yuanzhike.top/gthyiifyyd.html

[Q71] 查看建表语句
来源：http://hz.ivvv.top/gtqgngmnyz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtbqurpxdv.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtiggczbus.html

SHOW INDEX FROM users;
来源：http://hz.tanke756.top/gtuqrwkkla.html

[Q73] 查看表状态
来源：http://hz.chenjidiqi.icu/gthswtxdym.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtkactruux.html

[Q74] 强制使用索引
来源：http://hz.sysykeji.top/gtganncndy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.316326.xyz/gtkfdmznqn.html

[Q75] 日期格式化
来源：http://hz.jinqigfzy.top/gtiyunrfxk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aizwys.cn/gtdfagyaol.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinghuilouyu.cn/gtbyfkbels.html

[Q76] 按天统计
来源：http://hz.xingfuxueyuan.xyz/gtrzdkhtgy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydjk.org.cn/gtineklvkl.html

[Q77] 时间加减
来源：http://hz.xingfuxueyuan.xyz/gttavfwdqk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuxming.cn/gtiabvisby.html


<!-- 参考信息 -->