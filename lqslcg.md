代发 wailian999

[O02] 使用线程池
来源：http://hz.yuxming.cn/gtgfwfotol.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.mhx1999.top/gtxorntppf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xuanzx.com/gtqjxesrod.html

JS:   // worker_threads 线程池
来源：http://hz.xuanzx.com/gtwgajwcss.html

TS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtvsufhvtb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hongshengwenyu.top/gtyrcrdiwg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sysykeji.top/gtfdbqbjcm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jianghu66.top/gtpdjnxffi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.9152youxi.cn/gtvfxdbwql.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258.top/gtijdodjxc.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtpuwpkrbn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shanyushiyangkeji.top/gteyjvpcir.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gtglxfszgj.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gtayyvomut.html

Java: synchronized (this) { shared++; }
来源：http://hz.jyoumei.cn/gtsanjmejs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtwwnaacku.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangdashe.top/gtpuiwrukn.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhoulong.xyz/gtlvxprvqq.html

[O04] 定义异步函数并等待
来源：http://hz.dashuyun.cn/gtrmdeyzba.html

Py:   async def f():⏎    await g()
来源：http://hz.xziqi.cn/gtpouhdnyr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinqigufen.top/gthsvqddrm.html

JS:   async function f() { await g(); }
来源：http://hz.yonumen.top/gtktrwedwg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.vqdsnc.cn/gttiuvrbuk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ivvv.top/gtowghmkxo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.chenjidiqi.icu/gtngjsiyii.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gttbcnovoy.html

C#:   async Task F() { await G(); }
来源：http://hz.jiagoushi.top/gtapygleil.html

[O05] 并发执行并等待全部完成
来源：http://hz.pengpengdd.cyou/gtzjfpdnif.html

Py:   asyncio.gather(*tasks)
来源：http://hz.bjfxy.top/gtsjepvymd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dashuyun.cn/gtlmrmvjiu.html

JS:   await Promise.all(tasks)
来源：http://hz.yongpay.top/gtfjwsyyho.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtkuyydbfe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinghuilouyu.cn/gtzcvgiuxe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.chenzaomai.com/gtcxdyzyhb.html

Ruby: threads.map(&:join)
来源：http://hz.andypj.xyz/gtncciaaeo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daria6918.cn/gtzafvtefi.html

[O06] 使用进程池
来源：http://hz.chenlongwang.top/gteykueysm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daria6918.cn/gtdmnozmrq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.birdmap.top/gtcapsaoqh.html

JS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gtdtbyzvhi.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtpysuqmsz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jyoumei.cn/gtzdugqgae.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtfjtpfcls.html

Ruby: // fork 块
来源：http://hz.shanyushiyangtech.top/gtsovrtxgq.html

C#:   Parallel.For
来源：http://hz.shzxlz.cn/gtyvdocxfu.html

================================================================================
来源：http://hz.hysaishi.cn/gtjtgsqezr.html

P. 常用工具函数
来源：http://hz.ydzc1.top/gtbdpjnwsz.html

================================================================================
来源：http://hz.ppjwa.cn/gtoimyfqfo.html

[P01] 生成 UUID
来源：http://hz.nanxinkj.top/gtdcyccpcp.html

Py:   str(uuid.uuid4())
来源：http://hz.gogol.net.cn/gtzrpboezk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.bjfxy.top/gtlahykmtr.html

JS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtnlakcpqb.html

TS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtwtuvwjwn.html

Java: UUID.randomUUID().toString()
来源：http://hz.sxryk.cn/gtmlgqkous.html

Go:   // 用 github.com/google/uuid
来源：http://hz.c1oappe.top/gtxqanmlar.html

Ruby: SecureRandom.uuid
来源：http://hz.ywan-chungtsiang.top/gtfyqnxsyl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.bjfxy.top/gtrxuswiow.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sufxvd.cn/gtpvzoenxc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.smart0.xyz/gtssacapxz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zycfv.cn/gttkpiffcq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.haohaochexian.top/gtamqpwdwl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtyitjmktj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gtypodbmxc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.316326.xyz/gtfwexbqip.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hysaishi.cn/gtkcteroop.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gzhubu.top/gtxrfdxpau.html

[P03] 生成短随机字符串
来源：http://hz.havefunace.top/gtmzijkebg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yangfankeji.com/gtktbyjjhs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.chenlongwang.top/gthrakslts.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gtsiqisqnb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtnomnlrpv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.chenzaomai.com/gtxvoehocr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xinyue.icu/gttrzmapcv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jqgfzy.top/gtfnksbtzp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.meibo888.top/gtojcatvwk.html

[P04] 求长度
来源：http://hz.tianlin.xyz/gtsjntbqub.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cdnleiting.top/gtyycmstge.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shzxlz.cn/gtofjmcbnv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.52xcode.cn/gtjhxqyvjw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtcgeuhxoa.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gzhubu.top/gtvuxqygkr.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtrraxeukg.html

Ruby: x.length;  x.size
来源：http://hz.cdnleiting.top/gtgsjhhymj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xziqi.cn/gtvorulkic.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtvytoqydi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.birdmap.top/gtnbwuyluy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.birdmap.top/gtrgatbkof.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.nwbrower.top/gtcusjaaxp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.pengpengdd.cyou/gtgubladmg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258.top/gtwinzpmqi.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.shanyushiyangkeji.top/gtlccswpqr.html

Ruby: a == b
来源：http://hz.pengpengdd.cyou/gtwdhstpnp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.haohaochexian.top/gtswokysuu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgufenzy.top/gtbnnsjhsq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.hongshengwenyu.top/gtgbqnzfrz.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtmbeovvkk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.meibo888.top/gtvijncvfh.html

TS:   if (x == null) {}
来源：http://hz.jqgufenzy.top/gtyerwmdss.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shzxlz.cn/gtnbrjrxzf.html

Go:   if x == nil {}
来源：http://hz.yuanzhike.top/gtqqomslcw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.nanxuanxn.top/gtfvzkbtjr.html

C#:   if (x is null) {}
来源：http://hz.jlsjyb.cn/gtzfbroovr.html

[P07] 防抖与节流
来源：http://hz.xingfuxueyuan.xyz/gttznblruf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yongpay.top/gtfqnqkvlz.html

PHP:  // 手写时间戳比较
来源：http://hz.jlsjyb.cn/gtxnnjbyrn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.316326.xyz/gtcqxfejaw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtiykxqski.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhoulong.xyz/gtdunzrtym.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hammf.cn/gtbosdpqll.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.quarkkingdee.top/gteodmlgja.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.tanke756.top/gtkcykjyyz.html

[P08] 处理浮点精度问题
来源：http://hz.xuanzx.com/gtdjecuzqr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yj20258.top/gtyumfnsol.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.meibo888.top/gtzwzvockx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtxteczstd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.andypj.xyz/gteqhmigvd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.chenlongwang.top/gtpmwmpfnx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.snrcjt.cn/gtjswqhnth.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cashguo.top/gtbwlbvjeu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ybcxt.top/gtfqrqrnbc.html

================================================================================
来源：http://hz.cashguo.top/gtiffjkhcy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.dianchejie.cn/gtihcmeuaf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwvrjnbdc.html

[Q01] 创建表
来源：http://hz.feifeiyinyue.top/gtcubkjrsi.html

CREATE TABLE users (
来源：http://hz.feifeiyinyue.top/gtwleqikew.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtnlqptgwt.html

name VARCHAR(50) NOT NULL,
来源：http://hz.sufxvd.cn/gtilvokxxa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hfpthk.cn/gtnqaqowpr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hnxiangtu.top/gtfazirspi.html

);
来源：http://hz.cucudq.cn/gtqmsfioiq.html

[Q02] 创建带外键的表
来源：http://hz.gaohongyu789.top/gtbdatcpbs.html

CREATE TABLE orders (
来源：http://hz.meibo888.top/gtcuobwsze.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gttngiowpd.html

user_id INT NOT NULL,
来源：http://hz.xylfe.cn/gtuomlahmi.html

amount DECIMAL(10, 2),
来源：http://hz.jlsjyb.cn/gtuluumswx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj20258.top/gtfrvfzvmb.html

);
来源：http://hz.dianchejie.cn/gtwxozefpm.html

[Q03] 增加列
来源：http://hz.gaohongyu789.top/gtnrllqssh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nanxuanxn.top/gtrshbbpwf.html

[Q04] 修改列类型
来源：http://hz.cucudq.cn/gtakpofzqg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.bjfxy.top/gtdwonptod.html

[Q05] 重命名列
来源：http://hz.zhixingplan.top/gtscuyztnd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.snrcjt.cn/gtcrofmfyf.html

[Q06] 删除列
来源：http://hz.316326.xyz/gtjepzwkgj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yonumen.top/gtxwljnavt.html

[Q07] 删除表
来源：http://hz.shanyushiyangkeji.top/gtdqzbqypf.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jqgfzy.top/gthywikgjb.html

[Q08] 创建普通索引
来源：http://hz.jyoumei.cn/gtrwikxeur.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtxpzbzygc.html

[Q09] 创建唯一索引
来源：http://hz.feifeiyinyue.top/gtopcpxuqp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.shanyushiyangtech.top/gtgqmjufmg.html

[Q10] 插入单行
来源：http://hz.gotoacloud.top/gtzfsmzbyp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ydjk.org.cn/gtnqzcdxyb.html

[Q11] 一次插入多行
来源：http://hz.dianchejie.cn/gtrpvpnmye.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xylfe.cn/gtkqljplcv.html

[Q12] 插入后取自增 ID
来源：http://hz.hfpthk.cn/gtigxwtply.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sweek.top/gtncwrpsfv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenzaomai.com/gtybzweiue.html

[Q13] 忽略重复插入
来源：http://hz.andypj.xyz/gtslsoafqp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinghuilouyu.cn/gtisokvlmy.html

[Q14] 存在则更新（upsert）
来源：http://hz.nwbrower.top/gtjirpcvyu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.iojbl.cn/gtkbkrfegg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangkeji.top/gtacdklrbl.html

[Q15] 查询全部
来源：http://hz.yj20258.top/gtbdngqtbc.html

SELECT * FROM users;
来源：http://hz.zhijiandao.cn/gtsjbkwxrv.html

[Q16] 查询指定列
来源：http://hz.daria6918.cn/gtukrrdhsr.html

SELECT id, name FROM users;
来源：http://hz.cheryme.top/gtmwsonwfy.html

[Q17] 条件查询
来源：http://hz.zhoulong.xyz/gtwoeuodpr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhoulong.xyz/gtixghlept.html

[Q18] 模糊匹配
来源：http://hz.chenzaomai.com/gtstcygrsl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xingfuxueyuan.xyz/gteyrwxqrv.html

[Q19] 范围查询
来源：http://hz.ydjk.org.cn/gtmzeexaef.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtxyfrakcb.html

[Q20] IN 列表
来源：http://hz.chenjidiqi.icu/gtagssjikd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cucudq.cn/gtpubpuiak.html

[Q21] 空值判断
来源：http://hz.nanxinkj.top/gtattyojbh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.wangdashe.top/gtookwkvph.html

[Q22] 排序
来源：http://hz.ywan-chungtsiang.top/gtjkiuryfj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ppjwa.cn/gtjralceki.html

[Q23] 分页
来源：http://hz.birdmap.top/gtptkjbqye.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtycjrlgbz.html

[Q24] 去重
来源：http://hz.316326.xyz/gtoucisruj.html

SELECT DISTINCT city FROM users;
来源：http://hz.xuetiantiany.cn/gtrvdvdsbv.html

[Q25] 只取前 N 条
来源：http://hz.ydjk.org.cn/gtmmhphjsc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhaomingkeji.xyz/gtrvqqsegx.html

[Q26] 计数
来源：http://hz.tianlin.xyz/gtgmqbxxvt.html

SELECT COUNT(*) FROM users;
来源：http://hz.andypj.xyz/gthzekbora.html

[Q27] 条件计数
来源：http://hz.jianghu66.top/gtoabbogfm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenzaomai.com/gtrdiebrby.html

[Q28] 求和与平均
来源：http://hz.xuanzx.com/gtqkiwcaly.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.smart0.xyz/gtddozhykw.html

[Q29] 最大最小值
来源：http://hz.hongshengwenyu.top/gtbsfdjsof.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtggsuqrao.html

[Q30] 分组统计
来源：http://hz.andypj.xyz/gtayrrijdj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yangfankeji.com/gtmvxzrczz.html

[Q31] 分组后过滤
来源：http://hz.zhijiandao.cn/gthjqoohsz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigufen.top/gtudxuxevw.html

[Q32] 分组拼接字符串
来源：http://hz.andypj.xyz/gtobtpatbd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtfnlsrdnm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gtvzyhtytw.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtslbyspbq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yanxiufei.cn/gtvrecsprn.html

[Q34] 每组取第一条
来源：http://hz.zhongyouzk.top/gtzjshxphf.html

SELECT * FROM (
来源：http://hz.aibaodan.cn/gtydsclhwz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.vqdsnc.cn/gtkrykmjvy.html

) t WHERE rn = 1;
来源：http://hz.0kj1m.cn/gtttoawvkn.html

[Q35] 内连接
来源：http://hz.snrcjt.cn/gtokcaqrbx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtlcjbzkxy.html

[Q36] 左连接
来源：http://hz.svipenyu.cn/gtydydaovu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.pengpengdd.cyou/gtpmjftszm.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtyuyvhbdh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yanxiufei.cn/gtstnqgcjp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nwbrower.top/gtnwwsdwlq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.316326.xyz/gtnsbgfqwy.html

[Q39] 自连接（查上下级）
来源：http://hz.gotoacloud.top/gtclzcpzoa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.birdmap.top/gtlojfabmu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cucudq.cn/gtvdsknfvi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.snrcjt.cn/gtczrvxxid.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.sweek.top/gtgekcrpch.html

[Q41] 多表连接
来源：http://hz.gogol.net.cn/gtamqspnne.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtghfujehb.html

JOIN users u ON u.id = o.user_id
来源：http://hz.meibo888.top/gtzbucivdt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydzc1.top/gtbgwhfssv.html

[Q42] 连接条件附加过滤
来源：http://hz.zycfv.cn/gtigjvglnn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.meibo888.top/gtdipmiirv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zdqjudy.top/gtohjcuqrn.html

[Q43] 标量子查询
来源：http://hz.yj202588.top/gtvzszrrhd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xylfe.cn/gtaeroelet.html

[Q44] IN 子查询
来源：http://hz.nanxinkj.top/gtxbgzfsbn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangtech.top/gtuagxpece.html

[Q45] EXISTS 判断存在
来源：http://hz.quarkkingdee.top/gtbctqnmvv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gteckaizuc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtudtxwozy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtpkzctmxp.html

[Q47] 与平均值比较
来源：http://hz.jqgfzy.top/gtqqquyque.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhoulong.xyz/gtyzdaefha.html

[Q48] CTE 公用表表达式
来源：http://hz.jqgfzy.top/gtnulaqwow.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jqgfzy.top/gtzplbxfni.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtvwjcgtym.html

[Q49] 更新单行
来源：http://hz.gzhubu.top/gtmbzgyjtv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtmqylnycx.html

[Q50] 批量更新
来源：http://hz.meibo888.top/gtevjsmgbm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yangfankeji.com/gtkciivnie.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gtflpwdogq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenlongwang.top/gtdjbzomwd.html

[Q52] 删除指定行
来源：http://hz.zycfv.cn/gtjorosvxa.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hfpthk.cn/gtganoctfb.html

[Q53] 按条件删除
来源：http://hz.hammf.cn/gtqfylnjvc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtxinjtjex.html

[Q54] 清空表
来源：http://hz.iojbl.cn/gtkbbcipwn.html

TRUNCATE TABLE logs;
来源：http://hz.snrcjt.cn/gtkhjqsnmu.html

[Q55] 排名（并列占位）
来源：http://hz.vqdsnc.cn/gtmsaqtsky.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtlcamfbhw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.svipenyu.cn/gtljubldjy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinqigufen.top/gtcelqozjs.html

[Q57] 行号
来源：http://hz.smart0.xyz/gtrcksfmfy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.wangshuangyany.cn/gtlheiofzi.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtmbjzgfsn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtkfpgvpkl.html

[Q59] 分组内累计
来源：http://hz.52xcode.cn/gtsvcbkljh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gttkojjqol.html

[Q60] 取上一行 / 下一行
来源：http://hz.daxiang520.top/gtfodunjgg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ppjwa.cn/gteazjulys.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gtweezbcue.html

[Q61] 移动平均
来源：http://hz.aibaodan.cn/gtloxiutwe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.birdmap.top/gtzzwpmxrb.html

[Q62] 分组占比
来源：http://hz.shzxlz.cn/gtvonphpaq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtbikrmwcw.html

[Q63] 开启事务
来源：http://hz.jiagoushi.top/gtpvbqjumn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtvczuppsn.html

[Q64] 提交事务
来源：http://hz.nanxuanxn.top/gtgdeieoqs.html

COMMIT;
来源：http://hz.ivvv.top/gtxvhuaqcw.html

[Q65] 回滚事务
来源：http://hz.xziqi.cn/gtdlgpmliv.html

ROLLBACK;
来源：http://hz.tian-w.cn/gtcomhdrnd.html

[Q66] 行锁查询
来源：http://hz.redwolf501.top/gtxsykcfhf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yonumen.top/gtayyqptrd.html

[Q67] 设置隔离级别
来源：http://hz.gzhubu.top/gtudwzbjwv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hywenlv.cn/gtjtzzblze.html

[Q68] 保存点
来源：http://hz.fengsongda.top/gtzhayicci.html

SAVEPOINT sp1;
来源：http://hz.nanxinkj.top/gtxvuuxnyy.html

ROLLBACK TO sp1;
来源：http://hz.hammf.cn/gttyoymeew.html

[Q69] 查看执行计划
来源：http://hz.kuanghao11.cn/gtzvggurow.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtytwtzcmo.html

[Q70] 更新统计信息
来源：http://hz.cqqwz.cn/gtekdntqdx.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gtqbrtjijg.html

[Q71] 查看建表语句
来源：http://hz.zhiwuduotai.top/gtigdwphqg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tanke756.top/gtgvvaqcju.html

[Q72] 查看索引
来源：http://hz.yvedp.cn/gtnteywtoo.html

SHOW INDEX FROM users;
来源：http://hz.redwolf501.top/gtwtskiffe.html

[Q73] 查看表状态
来源：http://hz.ybcxt.top/gtmmmysrjo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cqqwz.cn/gtcauciuka.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtffnsljua.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pycfn.com/gtnndqebcj.html

[Q75] 日期格式化
来源：http://hz.ydzc1.top/gtxpcoprgx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sweek.top/gtdbphepie.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuanzhike.top/gtykkajrkr.html

[Q76] 按天统计
来源：http://hz.jiagoushi.top/gtholqvrgb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhijiandao.cn/gtqcjulbuk.html

[Q77] 时间加减
来源：http://hz.dianchejie.cn/gteblipcdl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.kuanghao11.cn/gtznybshci.html


<!-- 参考信息 -->