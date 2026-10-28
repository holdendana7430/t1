代发 wailian999

TS:   // worker_threads 线程池
来源：http://hz.sufxvd.cn/gtlqdokovy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtvvdyndih.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gthivtbkdi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pycfn.com/gtmgfuhvap.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtpabbjpyj.html

[O03] 加锁保护共享数据
来源：http://hz.xuanzx.com/gtgyyxrkfe.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtvlwijilh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.vqdsnc.cn/gtkegvgcoz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ybcxt.top/gtgpxjwnub.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtgyutjajh.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gtpdezvyhj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuanzhike.top/gtlyhbqcdr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pycfn.com/gtshxzeyho.html

C#:   lock (gate) { shared++; }
来源：http://hz.havefunace.top/gtpdusufif.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gteuhzdjsu.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigfzy.top/gtwtxlxflu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangtech.top/gtkcapkzbd.html

JS:   async function f() { await g(); }
来源：http://hz.guannengcc.top/gtdfzdpnrm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xinyue.icu/gtzuolnltq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zycfv.cn/gtuanlvdaw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.svipenyu.cn/gtreweanjc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hywenlv.cn/gtpgupjdre.html

C#:   async Task F() { await G(); }
来源：http://hz.pengpengdd.cyou/gtvurseflc.html

[O05] 并发执行并等待全部完成
来源：http://hz.chenlongwang.top/gttsvpfhaa.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtbepxycnf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinghuilouyu.cn/gtrltcihgn.html

JS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtiwypxgev.html

TS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gtbvlvktwk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fengsongda.top/gtfezpfova.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shzxlz.cn/gtuepsakpy.html

Ruby: threads.map(&:join)
来源：http://hz.c1oappe.top/gtesosahph.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cucudq.cn/gtmemtkiql.html

[O06] 使用进程池
来源：http://hz.shanyushiyangkeji.top/gtgorslwuu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hfpthk.cn/gtdzwzbxph.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gtxyqouojc.html

JS:   // child_process / cluster 模块
来源：http://hz.tianlin.xyz/gtwykgoafg.html

TS:   // child_process / cluster 模块
来源：http://hz.zhixingplan.top/gtkwczeejy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nwbrower.top/gtwdjoxaor.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gteqiqdgjc.html

Ruby: // fork 块
来源：http://hz.sysykeji.top/gtzghnhmaq.html

C#:   Parallel.For
来源：http://hz.guannengcc.top/gtmuhbxzdi.html

================================================================================
来源：http://hz.xylfe.cn/gtoixgnyhx.html

P. 常用工具函数
来源：http://hz.316326.xyz/gtpwjstdem.html

================================================================================
来源：http://hz.jqgfzy.top/gtjwmyhbaw.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gtxbvkdrxw.html

Py:   str(uuid.uuid4())
来源：http://hz.zhongyouzk.top/gtlnwflevr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.quarkkingdee.top/gtixegdtsd.html

JS:   crypto.randomUUID()
来源：http://hz.nanxinkj.top/gtitzdtxvv.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtihhxoefu.html

Java: UUID.randomUUID().toString()
来源：http://hz.zdqjudy.top/gtuceldyjt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangdashe.top/gtdnrfkkzk.html

Ruby: SecureRandom.uuid
来源：http://hz.xylfe.cn/gtefsxdxno.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.svipenyu.cn/gtwtliisfa.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuetiantiany.cn/gtjdzcqaxw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tian-w.cn/gtaajeikbu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gtgbidvitm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xylfe.cn/gtffhipndv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuxming.cn/gtrqeutkmw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ywan-chungtsiang.top/gtljdmbycw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tanke756.top/gtdflxfakk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.316326.xyz/gtrhamvtmx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cashguo.top/gtwtmbrpjk.html

[P03] 生成短随机字符串
来源：http://hz.iojbl.cn/gtzeqephwp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinghuilouyu.cn/gteztowvcr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.316326.xyz/gtfqkrxaai.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtfkaxijwq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtjzmtqjgq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigufen.top/gtultwsrtb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ybcxt.top/gtdlgrdjwk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.fzhhl.top/gtyrhpbsjw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shanyushiyangtech.top/gtpdshcgaq.html

[P04] 求长度
来源：http://hz.yonumen.top/gtxjneqmdn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.yonumen.top/gtzavwxjay.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtmzzjbrpw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtghbbucju.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.zhijiandao.cn/gtareqskiy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yvedp.cn/gtljsprufw.html

Go:   len(arr);  len(m)
来源：http://hz.kuanghao11.cn/gtrxjcvnxh.html

Ruby: x.length;  x.size
来源：http://hz.52xcode.cn/gtllqaxmjw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhixingplan.top/gtzrstiqvo.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jqgufenzy.top/gtoosqkkgb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.hysaishi.cn/gtxwpexqzk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.dianchejie.cn/gtzmhtzqbs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.svipenyu.cn/gtiubnxxcn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gogol.net.cn/gtulurgrow.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.vqdsnc.cn/gtdykelawb.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.andypj.xyz/gtaikbujkm.html

Ruby: a == b
来源：http://hz.feifeiyinyue.top/gtjooibijq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangtech.top/gtufuiousi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.ppjwa.cn/gtrkbihnpi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jyoumei.cn/gtmnrgxavf.html

PHP:  if (empty($x)) {}
来源：http://hz.guannengcc.top/gtjtymlyfw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guannengcc.top/gtbrlomcdl.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gtzlvzbndz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtzcvjejjp.html

Go:   if x == nil {}
来源：http://hz.zhengqikj.top/gtpuqzbmhi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.mhx1999.top/gtjgqqygws.html

C#:   if (x is null) {}
来源：http://hz.aizwys.cn/gtvhzlvsdr.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangtech.top/gtpqwpmmlu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.andypj.xyz/gtbxuqoczk.html

PHP:  // 手写时间戳比较
来源：http://hz.shzxlz.cn/gtcfsfrfun.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtlkjpiiua.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtembvmktx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.kuanghao11.cn/gtcygxccjr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.aizwys.cn/gttcwvgals.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jiagoushi.top/gtyuxcnura.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jqgfzy.top/gtdisgmnaz.html

[P08] 处理浮点精度问题
来源：http://hz.daria6918.cn/gtvzucfcsu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.chenjidiqi.icu/gtpfsjxjsl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shuidangran.top/gtcmaosxvx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yonumen.top/gtqyljzbkg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gotoacloud.top/gtjhlvpesr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yueranfly.top/gtpbratbwy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jiagoushi.top/gtnisihlzs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cqqwz.cn/gttrermvin.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.jinghuilouyu.cn/gtlufdnyse.html

================================================================================
来源：http://hz.pycfn.com/gteoridnob.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yangfankeji.com/gtipdtdgei.html

================================================================================
来源：http://hz.zhijiandao.cn/gttorrlqkf.html

[Q01] 创建表
来源：http://hz.daria6918.cn/gtmwgplmjz.html

CREATE TABLE users (
来源：http://hz.ivvv.top/gtostlzphi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zdqjudy.top/gtqnpnorcg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shanyushiyangtech.top/gtmajosaxh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cucudq.cn/gtixvsrlfn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yj202588.top/gtkqcrtlky.html

);
来源：http://hz.xuetiantiany.cn/gtfpjbsevn.html

[Q02] 创建带外键的表
来源：http://hz.gogol.net.cn/gtmaeptucm.html

CREATE TABLE orders (
来源：http://hz.zhiwuduotai.top/gttscnjxpm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shanyushiyangtech.top/gtbuhkvezh.html

user_id INT NOT NULL,
来源：http://hz.0kj1m.cn/gttgvklnbt.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtiuqsaicz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.haohaochexian.top/gtffcgamhg.html

);
来源：http://hz.guannengcc.top/gtehaugfrn.html

[Q03] 增加列
来源：http://hz.gotoacloud.top/gtjunpikmr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.nanxuanxn.top/gtlvfewxob.html

[Q04] 修改列类型
来源：http://hz.zhengqikj.top/gtjhjlrsjk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xylfe.cn/gteqpeuppp.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtpbjqvgnm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxinkj.top/gtfoyuqbsm.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gtdelvleet.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xuetiantiany.cn/gtyimwbjlq.html

[Q07] 删除表
来源：http://hz.fzhhl.top/gtrshdkutn.html

DROP TABLE IF EXISTS orders;
来源：http://hz.hnxiangtu.top/gtvejlijcb.html

[Q08] 创建普通索引
来源：http://hz.birdmap.top/gtjpnnqpky.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtkmifgqbk.html

[Q09] 创建唯一索引
来源：http://hz.aibaodan.cn/gtpdjdmndy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.vqdsnc.cn/gtvufbwjiw.html

[Q10] 插入单行
来源：http://hz.yuanzhike.top/gtchiqygmr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.sysykeji.top/gtizhdfdct.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gttwtnetxq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigufen.top/gtzjxsowsm.html

[Q12] 插入后取自增 ID
来源：http://hz.jinqigufen.top/gtsdiwhxqd.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xziqi.cn/gtfwaevrrm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nwbrower.top/gtsdsgypjp.html

[Q13] 忽略重复插入
来源：http://hz.ydzc1.top/gtkgetaetv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtdbtmhskt.html

[Q14] 存在则更新（upsert）
来源：http://hz.xziqi.cn/gtnjkvmdpz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.guannengcc.top/gtefmiysea.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gogol.net.cn/gtzibdmfqi.html

[Q15] 查询全部
来源：http://hz.andypj.xyz/gtudqqaydq.html

SELECT * FROM users;
来源：http://hz.yonumen.top/gtmcqfxikc.html

[Q16] 查询指定列
来源：http://hz.ywan-chungtsiang.top/gtkjxdztji.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gtfsslbohp.html

[Q17] 条件查询
来源：http://hz.0kj1m.cn/gtiqrkxzul.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.birdmap.top/gtqliqbynn.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtwyffrpae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenlongwang.top/gtrheoxydt.html

[Q19] 范围查询
来源：http://hz.cucudq.cn/gtrmhhsmys.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.snrcjt.cn/gtnkohtfgp.html

[Q20] IN 列表
来源：http://hz.ywan-chungtsiang.top/gtpfdybzbs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj202588.top/gtzpnlynck.html

[Q21] 空值判断
来源：http://hz.xuanzx.com/gtqkemcfzt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenlongwang.top/gtwbsocwxm.html

[Q22] 排序
来源：http://hz.yvedp.cn/gtlrundzoy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aibaodan.cn/gtpeqnulrq.html

[Q23] 分页
来源：http://hz.cheryme.top/gtizcgmeas.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ywan-chungtsiang.top/gtbcilrigj.html

[Q24] 去重
来源：http://hz.yj20258888.top/gtngrkwzqi.html

SELECT DISTINCT city FROM users;
来源：http://hz.mhx1999.top/gtzwhkgytp.html

[Q25] 只取前 N 条
来源：http://hz.shangyingyoupin.top/gtpwovgtjy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.svipenyu.cn/gtkkupfqlp.html

[Q26] 计数
来源：http://hz.guowangkeji.top/gtgevyzdnu.html

SELECT COUNT(*) FROM users;
来源：http://hz.meibo888.top/gtxyryltuq.html

[Q27] 条件计数
来源：http://hz.xziqi.cn/gthonbqtdy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.haohaochexian.top/gtepwsogqk.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtdawvrhwb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xinyue.icu/gtqhceubye.html

[Q29] 最大最小值
来源：http://hz.redwolf501.top/gtnnookfsx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xziqi.cn/gtshhljjmw.html

[Q30] 分组统计
来源：http://hz.guannengcc.top/gtyngfyfeq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtnisezwuq.html

[Q31] 分组后过滤
来源：http://hz.hammf.cn/gtpahvdlcr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yongpay.top/gtwbhdaxzf.html

[Q32] 分组拼接字符串
来源：http://hz.tanke756.top/gtwjxwoyex.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtyizvckze.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.gotoacloud.top/gtruqwapeg.html

[Q33] 多列分组
来源：http://hz.bjfxy.top/gtvjabghrt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xinyue.icu/gtnbsigafn.html

[Q34] 每组取第一条
来源：http://hz.feifeiyinyue.top/gtherrmfko.html

SELECT * FROM (
来源：http://hz.yvedp.cn/gtcvlgmxxr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinqigfzy.top/gtdbnvmwdm.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtsinkdwjg.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtzcmflhvu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxinkj.top/gtraeqkqgg.html

[Q36] 左连接
来源：http://hz.guannengcc.top/gtnifzrjti.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gtlnboovbx.html

[Q37] 右连接
来源：http://hz.hnxiangtu.top/gtagjocedh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yvedp.cn/gtfveiuwit.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.svipenyu.cn/gtnjftabbr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cheryme.top/gtyjglwufz.html

[Q39] 自连接（查上下级）
来源：http://hz.gaohongyu789.top/gtrapwhqpe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cucudq.cn/gtpkoqllou.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gtvreyeyjm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtfrzbfldx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtvnrbiuzn.html

[Q41] 多表连接
来源：http://hz.ybcxt.top/gtwbkqaryd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinqigfzy.top/gtymioperq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhoulong.xyz/gteydrgtfk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangtech.top/gtzerrgxxc.html

[Q42] 连接条件附加过滤
来源：http://hz.ywan-chungtsiang.top/gtynkctxbx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.havefunace.top/gtxzlkivte.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtznwnnnfh.html

[Q43] 标量子查询
来源：http://hz.xinyue.icu/gtabuiswhp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gtjbpibbqr.html

[Q44] IN 子查询
来源：http://hz.ivvv.top/gtfftnwoec.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ivvv.top/gtcsulozsz.html

[Q45] EXISTS 判断存在
来源：http://hz.yongpay.top/gtsloksdde.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtjgitcwvm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xziqi.cn/gtmzqaxyke.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.andypj.xyz/gtymmyndkl.html

[Q47] 与平均值比较
来源：http://hz.jlsjyb.cn/gtocvxwwap.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuetiantiany.cn/gtzqinxjfd.html

[Q48] CTE 公用表表达式
来源：http://hz.jlsjyb.cn/gtinsywyzk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigufen.top/gtwkudtlao.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.feifeiyinyue.top/gtkgfdqsju.html

[Q49] 更新单行
来源：http://hz.cdnleiting.top/gtibfjgjad.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ydzc1.top/gtyxrihgac.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtxolvfwdh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtezzipmlo.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtffjyyozk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgufenzy.top/gtsyzghzhi.html

[Q52] 删除指定行
来源：http://hz.jqgfzy.top/gttcefgdoa.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtarfjrslf.html

[Q53] 按条件删除
来源：http://hz.cashguo.top/gtrckvjeoo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.wangdashe.top/gtebduvgtw.html

[Q54] 清空表
来源：http://hz.tian-w.cn/gtrbdatqri.html

TRUNCATE TABLE logs;
来源：http://hz.pycfn.com/gtkebplqme.html

[Q55] 排名（并列占位）
来源：http://hz.jlsjyb.cn/gtdclengpk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgufenzy.top/gttfwrhqzz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gotoacloud.top/gtnmioydbg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuanzhike.top/gtbzmxbrud.html

[Q57] 行号
来源：http://hz.jianghu66.top/gtncalwiiu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtypcwcfqw.html

[Q58] 累计求和
来源：http://hz.birdmap.top/gttpordbgm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtuywqjbje.html

[Q59] 分组内累计
来源：http://hz.jqgfzy.top/gtiiflvzwf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.kuanghao11.cn/gtfhygsptf.html

[Q60] 取上一行 / 下一行
来源：http://hz.tanke756.top/gtszwzohuo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gtontnukei.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jianghu66.top/gtsdosvvxj.html

[Q61] 移动平均
来源：http://hz.cqqwz.cn/gtmitgcofu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gtbxzhlfog.html

[Q62] 分组占比
来源：http://hz.shangyingyoupin.top/gtvfnztdzr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuanzhike.top/gtstzzdseo.html

[Q63] 开启事务
来源：http://hz.sweek.top/gtctzoewqo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yanxiufei.cn/gtbwdvbnga.html

[Q64] 提交事务
来源：http://hz.gogol.net.cn/gtrcqnfdwk.html

COMMIT;
来源：http://hz.hammf.cn/gtvfaqxmij.html

[Q65] 回滚事务
来源：http://hz.shuidangran.top/gtkcboyeml.html

ROLLBACK;
来源：http://hz.tian-w.cn/gthuecudpj.html

[Q66] 行锁查询
来源：http://hz.zhengqikj.top/gtqgnuxixy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hywenlv.cn/gtikxlslau.html

[Q67] 设置隔离级别
来源：http://hz.pycfn.com/gtqmokrqfg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xziqi.cn/gtnyneocud.html

[Q68] 保存点
来源：http://hz.sufxvd.cn/gtsmgqowsu.html

SAVEPOINT sp1;
来源：http://hz.hnxiangtu.top/gtbupmqqwv.html

ROLLBACK TO sp1;
来源：http://hz.iojbl.cn/gtrwrruqlp.html

[Q69] 查看执行计划
来源：http://hz.zhiwuduotai.top/gtfqpvrquj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nwbrower.top/gthmiawkri.html

[Q70] 更新统计信息
来源：http://hz.snrcjt.cn/gtgvguwiiv.html

ANALYZE TABLE users;
来源：http://hz.yj202588.top/gtwtpqiich.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gtjfwrybok.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtezerbusw.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtzurzzdph.html

SHOW INDEX FROM users;
来源：http://hz.jinqigfzy.top/gtqkqkcshb.html

[Q73] 查看表状态
来源：http://hz.316326.xyz/gtuiyltxmd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ywan-chungtsiang.top/gtmzgvilqv.html

[Q74] 强制使用索引
来源：http://hz.yueranfly.top/gtqmxaiimx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtmpmhhaad.html

[Q75] 日期格式化
来源：http://hz.zhengqikj.top/gtuansacub.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.dashuyun.cn/gtcgpdqtpz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gogol.net.cn/gtsaybyblc.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtppigknyb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xziqi.cn/gtayvixznb.html

[Q77] 时间加减
来源：http://hz.wangdashe.top/gtshbpoygv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydjk.org.cn/gtfucdhrlt.html

[Q78] 当前时间
来源：http://hz.xinyue.icu/gtohrmzgxb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guannengcc.top/gtoqsocaxl.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gthbpgaoiy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.aizwys.cn/gtbucfsrlw.html


<!-- 参考信息 -->