代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ivvv.top/gtdzkcxrry.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hfpthk.cn/gtloezgent.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hammf.cn/gtgquggidh.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gtnsyybwrb.html

Java: new Thread(() -> f()).start()
来源：http://hz.cucudq.cn/gtclqsvcyv.html

Go:   go f()
来源：http://hz.ppjwa.cn/gteccwxpkh.html

Ruby: Thread.new { f }
来源：http://hz.birdmap.top/gtxluzjasf.html

C#:   Task.Run(() => F());
来源：http://hz.zycfv.cn/gtgxbcfvet.html

[O02] 使用线程池
来源：http://hz.cheryme.top/gtectawvmr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.316326.xyz/gtzjusafde.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gtktmysceb.html

JS:   // worker_threads 线程池
来源：http://hz.mhx1999.top/gttashfinx.html

TS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtyuyqfhsb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenjidiqi.icu/gtzflfnygk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ehwqpu.com/gtvoufxrbw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenjidiqi.icu/gtdcqigjos.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gtyqgkaycl.html

[O03] 加锁保护共享数据
来源：http://hz.jinqigufen.top/gtefqecrmo.html

Py:   with lock: shared += 1
来源：http://hz.fengsongda.top/gtszshzvyw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tianlin.xyz/gtshhbopbv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtuxyqdvcf.html

TS:   // 同 JS
来源：http://hz.aizwys.cn/gtazrnrowd.html

Java: synchronized (this) { shared++; }
来源：http://hz.sweek.top/gtrbzqyzzf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shzxlz.cn/gtcargkuts.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenlongwang.top/gthkggodyc.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhoulong.xyz/gtjlkpyitf.html

[O04] 定义异步函数并等待
来源：http://hz.andypj.xyz/gtewcowgbt.html

Py:   async def f():⏎    await g()
来源：http://hz.jinyuanbaomall.cn/gtzlpymold.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangshuangyany.cn/gttektsedb.html

JS:   async function f() { await g(); }
来源：http://hz.52xcode.cn/gthmjpjixu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxinkj.top/gtpllzcpwf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jqgfzy.top/gtwieqzqbn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gtblybdrrg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jyoumei.cn/gtzdzgvjiu.html

C#:   async Task F() { await G(); }
来源：http://hz.ywan-chungtsiang.top/gtkkzkwdic.html

[O05] 并发执行并等待全部完成
来源：http://hz.shzxlz.cn/gtvnkxirha.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shuidangran.top/gtdurpotsd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jianghu66.top/gtygbozvky.html

JS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gtupwlxppf.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtjdimwhmg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.sxryk.cn/gtdhjczlaf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cdnleiting.top/gtsvxuzdjw.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gtdvcedxls.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhijiandao.cn/gtgiysgkao.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtpgeqxaop.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj202588.top/gtgfplgupk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhixingplan.top/gtpsuujreh.html

JS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtckyiqfqw.html

TS:   // child_process / cluster 模块
来源：http://hz.wangshuangyany.cn/gtefivcptm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sxryk.cn/gtzeodkfle.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258888.top/gtfpiqucee.html

Ruby: // fork 块
来源：http://hz.gogol.net.cn/gtmpqbnkop.html

C#:   Parallel.For
来源：http://hz.xuetiantiany.cn/gtbhkwgowq.html

================================================================================
来源：http://hz.jqgfzy.top/gtzmisimnc.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtlxmxxdhs.html

================================================================================
来源：http://hz.cucudq.cn/gtxjsjwisd.html

[P01] 生成 UUID
来源：http://hz.sysykeji.top/gtdgxghlvl.html

Py:   str(uuid.uuid4())
来源：http://hz.xuetiantiany.cn/gtwzhxnizm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtjlrbkmrv.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtbptenhsp.html

TS:   crypto.randomUUID()
来源：http://hz.9152youxi.cn/gtjbvnrhxj.html

Java: UUID.randomUUID().toString()
来源：http://hz.0kj1m.cn/gtekxpfzgb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuxming.cn/gtkehwambd.html

Ruby: SecureRandom.uuid
来源：http://hz.yueranfly.top/gtuswsngej.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sxryk.cn/gtabspffqv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jyoumei.cn/gtmqqjmmgm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.shanyushiyangkeji.top/gtgcufiarm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258888.top/gtwlxvvozu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yanxiufei.cn/gtvguyqbnr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sufxvd.cn/gtixhdowxk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aibaodan.cn/gtwxggesdr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuanzx.com/gtjimegqsr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtwqzwmrew.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.chenjidiqi.icu/gttxpqdpce.html

[P03] 生成短随机字符串
来源：http://hz.vqdsnc.cn/gtyuzhzizv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.hammf.cn/gtqbwmdsia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sysykeji.top/gtiaibtryv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gtkmvjetwz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtbrcavgwy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jlsjyb.cn/gteqtusovh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhoulong.xyz/gtedkfsqnp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yueranfly.top/gtrhfctfvj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tian-w.cn/gtepnemedt.html

[P04] 求长度
来源：http://hz.hnqzz.top/gtghmlgdvk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.daxiang520.top/gtpgaqqgzx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtbhywstoi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yangfankeji.com/gtaowsipve.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.kuanghao11.cn/gtwynsonam.html

Java: list.size();  map.size();  s.length()
来源：http://hz.gzhubu.top/gtptplcics.html

Go:   len(arr);  len(m)
来源：http://hz.vqdsnc.cn/gtymsqyrqn.html

Ruby: x.length;  x.size
来源：http://hz.zdqjudy.top/gtgnrpubaq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.wangdashe.top/gtlstpstgf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenzaomai.com/gthrumgrao.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.fzhhl.top/gtqvlrqqbm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hammf.cn/gtuwrenycs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cucudq.cn/gtjimrrzjt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zycfv.cn/gtmtvcvdor.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.hammf.cn/gtdzedfvit.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhongyouzk.top/gtbxwljyyd.html

Ruby: a == b
来源：http://hz.pengpengdd.cyou/gtyqluwzve.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhaomingkeji.xyz/gtaopefojm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yanxiufei.cn/gtclolugtw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhongyouzk.top/gtxdigkcwk.html

PHP:  if (empty($x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtuemhferz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.mhx1999.top/gtdkxisjqx.html

TS:   if (x == null) {}
来源：http://hz.ybcxt.top/gtfdcpolsg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtpnensfmn.html

Go:   if x == nil {}
来源：http://hz.hywenlv.cn/gtlrchwaci.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.havefunace.top/gtaoogcvss.html

C#:   if (x is null) {}
来源：http://hz.316326.xyz/gtkwvdwobd.html

[P07] 防抖与节流
来源：http://hz.nanxuanxn.top/gtvdlnimke.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhongyouzk.top/gtwuxnhohs.html

PHP:  // 手写时间戳比较
来源：http://hz.cucudq.cn/gtyocgygtq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gthtlodshq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtmfshbjqp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hysaishi.cn/gtxyjmubbo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.dashuyun.cn/gtmxdstxgx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ehwqpu.com/gtjhvbmskg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ivvv.top/gtxetvlkvv.html

[P08] 处理浮点精度问题
来源：http://hz.tianlin.xyz/gtmkqbyodu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhijiandao.cn/gtuytbdjyz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daxiang520.top/gtkomgqwuy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.chenlongwang.top/gtniptefhm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.fengsongda.top/gtpxyhxmhp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zycfv.cn/gtaxcvdgej.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.zhiwuduotai.top/gtpnywzfpw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yanxiufei.cn/gtuiiefhwo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gtylshxpnu.html

================================================================================
来源：http://hz.ybcxt.top/gtpxqgattn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ehwqpu.com/gtzdmqoeiu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgeqsrnbn.html

[Q01] 创建表
来源：http://hz.hnxiangtu.top/gtperpqtml.html

CREATE TABLE users (
来源：http://hz.cucudq.cn/gtlkdvlfem.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhongyouzk.top/gtiunzzxta.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtuznlgqcc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aibaodan.cn/gtimzdhurx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sweek.top/gtegnckgmb.html

);
来源：http://hz.nanxinkj.top/gtkqzmrnnc.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtwagyefnk.html

CREATE TABLE orders (
来源：http://hz.yuanzhike.top/gtkozqzqwa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtosshvpra.html

user_id INT NOT NULL,
来源：http://hz.cheryme.top/gtpbbwaqiw.html

amount DECIMAL(10, 2),
来源：http://hz.birdmap.top/gtrqtulged.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.hnxiangtu.top/gtbbrkfdad.html

);
来源：http://hz.cashguo.top/gtjxjbvniy.html

[Q03] 增加列
来源：http://hz.guannengcc.top/gtwvhhxkkm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.havefunace.top/gtwhwpfhbk.html

[Q04] 修改列类型
来源：http://hz.gogol.net.cn/gtkmyossqf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.iojbl.cn/gttvbkfinf.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtixrykigl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.0kj1m.cn/gtuustujen.html

[Q06] 删除列
来源：http://hz.aizwys.cn/gtnhwzqwyf.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.kuanghao11.cn/gthrnnabqk.html

[Q07] 删除表
来源：http://hz.ydjk.org.cn/gtnyrttivl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yuanzhike.top/gthysowqsi.html

[Q08] 创建普通索引
来源：http://hz.pycfn.com/gtnitizzxv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nwbrower.top/gthkbjydte.html

[Q09] 创建唯一索引
来源：http://hz.vqdsnc.cn/gtnbfghvsp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhaomingkeji.xyz/gtbuwxrjaf.html

[Q10] 插入单行
来源：http://hz.ydjk.org.cn/gtpuaueaab.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yuanzhike.top/gtfvqklxcp.html

[Q11] 一次插入多行
来源：http://hz.gaohongyu789.top/gtrjnavsdk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangdashe.top/gtpxbnulgl.html

[Q12] 插入后取自增 ID
来源：http://hz.316326.xyz/gtjvsvwfos.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cheryme.top/gtghzjzgor.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shzxlz.cn/gtbrvlmrfr.html

[Q13] 忽略重复插入
来源：http://hz.fzhhl.top/gtmihkjegd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.316326.xyz/gtixkzwqdp.html

[Q14] 存在则更新（upsert）
来源：http://hz.kuanghao11.cn/gtbqcpbeiw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.fzhhl.top/gtwugczmkn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ehwqpu.com/gtdniynuku.html

[Q15] 查询全部
来源：http://hz.zhixingplan.top/gtrgimcmij.html

SELECT * FROM users;
来源：http://hz.gogol.net.cn/gthvhcnzjo.html

[Q16] 查询指定列
来源：http://hz.jinqigfzy.top/gtphenxifh.html

SELECT id, name FROM users;
来源：http://hz.hnqzz.top/gtdkrsgtro.html

[Q17] 条件查询
来源：http://hz.ywan-chungtsiang.top/gtrxfmzjvw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yangfankeji.com/gtrcpwhowu.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtrylxkjiu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shzxlz.cn/gtackiovks.html

[Q19] 范围查询
来源：http://hz.fzhhl.top/gtsjbcptmn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhongyouzk.top/gthurocluh.html

[Q20] IN 列表
来源：http://hz.wangdashe.top/gtwxvujxtz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.bjfxy.top/gtpfidmxen.html

[Q21] 空值判断
来源：http://hz.meibo888.top/gtgtqabtte.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gaohongyu789.top/gtvkwhauum.html

[Q22] 排序
来源：http://hz.dashuyun.cn/gtdhzgqtih.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.aibaodan.cn/gtwadvtatz.html

[Q23] 分页
来源：http://hz.xuanzx.com/gtibibhkqh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigfzy.top/gtyoeohlkp.html

[Q24] 去重
来源：http://hz.yueranfly.top/gtcggehwhl.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gtcvznwnui.html

[Q25] 只取前 N 条
来源：http://hz.hysaishi.cn/gtkugjjrel.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.feifeiyinyue.top/gtmnmqhwyw.html

[Q26] 计数
来源：http://hz.ydjk.org.cn/gtqmrjboka.html

SELECT COUNT(*) FROM users;
来源：http://hz.316326.xyz/gtamaqffdv.html

[Q27] 条件计数
来源：http://hz.zhixingplan.top/gtfktyioyx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.redwolf501.top/gtadfvimee.html

[Q28] 求和与平均
来源：http://hz.guannengcc.top/gtgyrpwfra.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhoulong.xyz/gtlouqjvzs.html

[Q29] 最大最小值
来源：http://hz.nanxinkj.top/gtykfmgjnj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gtbcmwwgjf.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtgqpzoyii.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtalutrygc.html

[Q31] 分组后过滤
来源：http://hz.jqgfzy.top/gtseimwasf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gogol.net.cn/gtopvscfua.html

[Q32] 分组拼接字符串
来源：http://hz.zhijiandao.cn/gtleolawxa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtcugdwjss.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yvedp.cn/gtgupnwwra.html

[Q33] 多列分组
来源：http://hz.zhaomingkeji.xyz/gthzpzxnxa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtgytbxsvt.html

[Q34] 每组取第一条
来源：http://hz.tanke756.top/gtjzxcsgcp.html

SELECT * FROM (
来源：http://hz.havefunace.top/gtsgvgdnlf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtzhxuzooz.html

) t WHERE rn = 1;
来源：http://hz.xinyue.icu/gtmoymnwxz.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gttfdnkozw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ywan-chungtsiang.top/gtuxmqfayw.html

[Q36] 左连接
来源：http://hz.dashuyun.cn/gtwxfvsluz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtubotmqaf.html

[Q37] 右连接
来源：http://hz.jqgfzy.top/gtkoiqyugo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yongpay.top/gteicsfjeu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gaohongyu789.top/gtsbpuqtyr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhaomingkeji.xyz/gtfltzcadd.html

[Q39] 自连接（查上下级）
来源：http://hz.9152youxi.cn/gtvyzizddp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigfzy.top/gtttplvxqz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.pengpengdd.cyou/gtrfnnwzem.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fzhhl.top/gtlsqsgfgk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.aizwys.cn/gthsxldrsf.html

[Q41] 多表连接
来源：http://hz.shangyingyoupin.top/gtfdnzeqla.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hammf.cn/gtphnndqzi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nwbrower.top/gtgnghkqbz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sufxvd.cn/gtogqutzan.html

[Q42] 连接条件附加过滤
来源：http://hz.hnqzz.top/gtkkldywek.html

SELECT u.name, o.amount FROM users u
来源：http://hz.quarkkingdee.top/gtrtaarzoo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhijiandao.cn/gtpvfrcmjx.html

[Q43] 标量子查询
来源：http://hz.svipenyu.cn/gtshtefvqm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xziqi.cn/gtksnkueib.html

[Q44] IN 子查询
来源：http://hz.hnqzz.top/gtrxrkourz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zycfv.cn/gtvosmzbki.html

[Q45] EXISTS 判断存在
来源：http://hz.xylfe.cn/gtvujvmrec.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtmiahompt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenzaomai.com/gtqteftwee.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gtyyzzhvio.html

[Q47] 与平均值比较
来源：http://hz.wangshuangyany.cn/gtgmtdpudv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.daria6918.cn/gtndbqghmj.html

[Q48] CTE 公用表表达式
来源：http://hz.zdqjudy.top/gtayfvhoqt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gtlyzmqwhp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj202588.top/gtvwpiwzdu.html

[Q49] 更新单行
来源：http://hz.jqgfzy.top/gtmabkqaxe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pycfn.com/gtkmifmord.html

[Q50] 批量更新
来源：http://hz.cheryme.top/gtiajssbzw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gttwgoeouv.html

[Q51] 用子查询更新
来源：http://hz.hysaishi.cn/gthgvsiife.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yangfankeji.com/gtzgrbafqq.html

[Q52] 删除指定行
来源：http://hz.hnxiangtu.top/gtpxzrpaip.html

DELETE FROM users WHERE id = 10;
来源：http://hz.c1oappe.top/gthppulzzy.html

[Q53] 按条件删除
来源：http://hz.zdqjudy.top/gtjoealaeh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.mhx1999.top/gtqmokfkpm.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtgrgdmqhf.html

TRUNCATE TABLE logs;
来源：http://hz.aibaodan.cn/gtktqlnxup.html

[Q55] 排名（并列占位）
来源：http://hz.chenjidiqi.icu/gtusqezxcq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangshuangyany.cn/gtttljvcjw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuanzx.com/gtcezjxiie.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zycfv.cn/gtuxqwjzal.html

[Q57] 行号
来源：http://hz.hnqzz.top/gtyidbcyta.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.316326.xyz/gtciyamrmf.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gtfuuyfyyv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.kuanghao11.cn/gtzbssyhmt.html

[Q59] 分组内累计
来源：http://hz.cucudq.cn/gtiuuyndfh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gtrdkevygz.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtdvqwfewc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.quarkkingdee.top/gtnmuwuwym.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hywenlv.cn/gtzhitbngj.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtxeehjopk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gttctdpjgh.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtzzaopuru.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtoivcophl.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gtsvgcwdot.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.andypj.xyz/gtyrharnzo.html

[Q64] 提交事务
来源：http://hz.daria6918.cn/gtejfribqn.html

COMMIT;
来源：http://hz.vqdsnc.cn/gtarerhucb.html

[Q65] 回滚事务
来源：http://hz.yangfankeji.com/gtzimtfgdo.html

ROLLBACK;
来源：http://hz.nanxuanxn.top/gtehsuouma.html

[Q66] 行锁查询
来源：http://hz.ivvv.top/gtvzlfaqdd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xziqi.cn/gtznchbqhd.html

[Q67] 设置隔离级别
来源：http://hz.yvedp.cn/gtflnldxst.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ppjwa.cn/gtvykyuiyt.html

[Q68] 保存点
来源：http://hz.yuxming.cn/gtxgbtnunn.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gtsuuamvti.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtiwnehlnm.html

[Q69] 查看执行计划
来源：http://hz.ehwqpu.com/gttwitbbiw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gtuyzrufgh.html

[Q70] 更新统计信息
来源：http://hz.xingfuxueyuan.xyz/gtidftgkjz.html

ANALYZE TABLE users;
来源：http://hz.vqdsnc.cn/gttapjogmv.html

[Q71] 查看建表语句
来源：http://hz.vqdsnc.cn/gtyfqfxfsf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cdnleiting.top/gtlyczbeii.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gtoouoxuvq.html

SHOW INDEX FROM users;
来源：http://hz.smart0.xyz/gtaywpzwwn.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtdcyudaxi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtvenkbejx.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gttibrdner.html


<!-- 参考信息 -->