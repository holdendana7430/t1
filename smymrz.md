代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.pengpengdd.cyou/gtacraojul.html

[O03] 加锁保护共享数据
来源：http://hz.jinghuilouyu.cn/gtnrtnaskp.html

Py:   with lock: shared += 1
来源：http://hz.zhengqikj.top/gtgpzucelu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ydjk.org.cn/gttzufhcjn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hfpthk.cn/gtxdurggjk.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtfkikmoig.html

Java: synchronized (this) { shared++; }
来源：http://hz.ybcxt.top/gtvpwfzrnp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aizwys.cn/gtfwubjtzr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aibaodan.cn/gtskcucoel.html

C#:   lock (gate) { shared++; }
来源：http://hz.shangyingyoupin.top/gtjdimjfup.html

[O04] 定义异步函数并等待
来源：http://hz.guowangkeji.top/gtvkpscuxm.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtxcjmwtqq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tanke756.top/gtdbiprida.html

JS:   async function f() { await g(); }
来源：http://hz.zhongyouzk.top/gtqrlgtmlo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtjefusgjm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guannengcc.top/gteqyqbgov.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daxiang520.top/gtzyakkmnv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.snrcjt.cn/gttzclblpy.html

C#:   async Task F() { await G(); }
来源：http://hz.cdnleiting.top/gthsrtfwor.html

[O05] 并发执行并等待全部完成
来源：http://hz.cdnleiting.top/gtqnhiaxzp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuxming.cn/gtgcnziujs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhijiandao.cn/gtxpdgcwpc.html

JS:   await Promise.all(tasks)
来源：http://hz.gogol.net.cn/gttelpqzdu.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtrdsbajxn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.kuanghao11.cn/gtksuxnwya.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zdqjudy.top/gtztxqwzsf.html

Ruby: threads.map(&:join)
来源：http://hz.meibo888.top/gtxpadiqwb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yangfankeji.com/gtsvkinivu.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtgvvsfqrc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.wangdashe.top/gtutshwacm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxuanxn.top/gtkauhhfwr.html

JS:   // child_process / cluster 模块
来源：http://hz.sysykeji.top/gtvxbkirer.html

TS:   // child_process / cluster 模块
来源：http://hz.nanxuanxn.top/gtxmjjpkaa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj20258888.top/gtjiigenjl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigfzy.top/gtfkmorwme.html

Ruby: // fork 块
来源：http://hz.bjfxy.top/gtwlqmoyev.html

C#:   Parallel.For
来源：http://hz.9152youxi.cn/gtnramjrdb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtkttrjncy.html

P. 常用工具函数
来源：http://hz.zhiwuduotai.top/gtjmehmqrq.html

================================================================================
来源：http://hz.birdmap.top/gtsjuyjexm.html

[P01] 生成 UUID
来源：http://hz.hongshengwenyu.top/gtzuropfdm.html

Py:   str(uuid.uuid4())
来源：http://hz.9152youxi.cn/gtyeovjnji.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cdnleiting.top/gtoexfrpao.html

JS:   crypto.randomUUID()
来源：http://hz.yongpay.top/gtomvvxgdg.html

TS:   crypto.randomUUID()
来源：http://hz.bjfxy.top/gtjjvgufzs.html

Java: UUID.randomUUID().toString()
来源：http://hz.nwbrower.top/gtwvwonxjg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hnqzz.top/gteigpsvkk.html

Ruby: SecureRandom.uuid
来源：http://hz.aizwys.cn/gteijsvqnl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daxiang520.top/gtkuslrmam.html

[P02] MD5 / SHA256 摘要
来源：http://hz.xuanzx.com/gtanukakyb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jinqigufen.top/gtcobmskkc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtfclnonib.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shzxlz.cn/gtqoooxurl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhoulong.xyz/gtgtdcwypx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hnqzz.top/gtdboctifw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jiagoushi.top/gtthzmglgv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.fzhhl.top/gtdfcplygc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gtidvgmzka.html

[P03] 生成短随机字符串
来源：http://hz.mhx1999.top/gtkwabbybl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.meibo888.top/gtojdzendx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xziqi.cn/gtwkebywpx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangkeji.top/gtcahbevkv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtaconhxjw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xziqi.cn/gtgyqpgkkz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shuidangran.top/gtmcsuouwz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.aizwys.cn/gtscscalpx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.chenjidiqi.icu/gtolevrzlp.html

[P04] 求长度
来源：http://hz.feifeiyinyue.top/gtxqjjddsd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xylfe.cn/gtuqmyhkne.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtudmdturn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xinyue.icu/gtcawacvwf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtnoryigrh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.birdmap.top/gtpsbvymgv.html

Go:   len(arr);  len(m)
来源：http://hz.dashuyun.cn/gtokzwgzro.html

Ruby: x.length;  x.size
来源：http://hz.chenzaomai.com/gtchdywwhj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xylfe.cn/gtxwyahmxb.html

[P05] 判断两个对象内容是否相等
来源：http://hz.mhx1999.top/gtpaucdcfs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jianghu66.top/gtnqjzlqjk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.bjfxy.top/gtapcwytzb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.wangdashe.top/gtnlstkzwb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hywenlv.cn/gtbwublrsz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yj20258.top/gtbzfwldwe.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenjidiqi.icu/gtguljvsmh.html

Ruby: a == b
来源：http://hz.fzhhl.top/gtipqewlgq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.bjfxy.top/gtknzdowij.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtyuhbpeda.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zhijiandao.cn/gtigocjimq.html

PHP:  if (empty($x)) {}
来源：http://hz.daxiang520.top/gtrzaqnkgd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gtuytbegad.html

TS:   if (x == null) {}
来源：http://hz.zhongyouzk.top/gtyvvgqcuj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.c1oappe.top/gtvnqdsbkw.html

Go:   if x == nil {}
来源：http://hz.chenzaomai.com/gtkbfhramo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shangyingyoupin.top/gturlzssvv.html

C#:   if (x is null) {}
来源：http://hz.guannengcc.top/gtdieflohe.html

[P07] 防抖与节流
来源：http://hz.jyoumei.cn/gthjtgueyx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yonumen.top/gtaivzuaht.html

PHP:  // 手写时间戳比较
来源：http://hz.yongpay.top/gtakwqhobk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhijiandao.cn/gtvtrubyyn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtfojfdmdv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zhaomingkeji.xyz/gtdchkxkqm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jiagoushi.top/gtcfykuypj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hongshengwenyu.top/gtwynnhihr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gzhubu.top/gtkylllfys.html

[P08] 处理浮点精度问题
来源：http://hz.jinqigufen.top/gtkimhovlj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.52xcode.cn/gtxqymrpnm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.tianlin.xyz/gtehekomby.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yueranfly.top/gtnuymlxbf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zhiwuduotai.top/gtppcjxllz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.wangshuangyany.cn/gtzjbmohek.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hammf.cn/gtsbiuxdza.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xylfe.cn/gtladjyfcl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hammf.cn/gtgksakdmq.html

================================================================================
来源：http://hz.aibaodan.cn/gtujkkvlll.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.hywenlv.cn/gtppexrdmi.html

================================================================================
来源：http://hz.jlsjyb.cn/gtahpvgvqi.html

[Q01] 创建表
来源：http://hz.shangyingyoupin.top/gtlpzdtmoy.html

CREATE TABLE users (
来源：http://hz.wangshuangyany.cn/gthoqlwwrl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jyoumei.cn/gtavtwgpfb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ivvv.top/gtoqhhaaxi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.pycfn.com/gtgeffyfoi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.dianchejie.cn/gtusodjfxp.html

);
来源：http://hz.meibo888.top/gtisefszun.html

[Q02] 创建带外键的表
来源：http://hz.redwolf501.top/gtdsdqzogt.html

CREATE TABLE orders (
来源：http://hz.yj20258.top/gttmjuurmi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtlcficsgr.html

user_id INT NOT NULL,
来源：http://hz.hywenlv.cn/gtpihnpdli.html

amount DECIMAL(10, 2),
来源：http://hz.shzxlz.cn/gtrcfhhgba.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.kuanghao11.cn/gtikjpslyt.html

);
来源：http://hz.9152youxi.cn/gtqfkvswnf.html

[Q03] 增加列
来源：http://hz.smart0.xyz/gtunuizyaf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtnvausbrm.html

[Q04] 修改列类型
来源：http://hz.pycfn.com/gtqlsbrzrv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.redwolf501.top/gtbdlyyjvk.html

[Q05] 重命名列
来源：http://hz.zhiwuduotai.top/gtrnmbqmsl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.dianchejie.cn/gtxexssnba.html

[Q06] 删除列
来源：http://hz.zhaomingkeji.xyz/gtastdebzc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.smart0.xyz/gtszfdzxsp.html

[Q07] 删除表
来源：http://hz.hysaishi.cn/gtthjkhpku.html

DROP TABLE IF EXISTS orders;
来源：http://hz.birdmap.top/gtplnjudvs.html

[Q08] 创建普通索引
来源：http://hz.quarkkingdee.top/gtaqjuseau.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gaohongyu789.top/gtldhumvtv.html

[Q09] 创建唯一索引
来源：http://hz.shzxlz.cn/gtajcnmgff.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtdktmjypj.html

[Q10] 插入单行
来源：http://hz.yj20258888.top/gtixsptjoo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.aibaodan.cn/gtwtwnxchk.html

[Q11] 一次插入多行
来源：http://hz.zhaomingkeji.xyz/gtflmdzbib.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.9152youxi.cn/gtyjyxvkrq.html

[Q12] 插入后取自增 ID
来源：http://hz.quarkkingdee.top/gtpcmqcfdy.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.yangfankeji.com/gtxoowbnwc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.sxryk.cn/gtojixddmj.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtcxtwaood.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.birdmap.top/gtdrptzqrd.html

[Q14] 存在则更新（upsert）
来源：http://hz.ivvv.top/gteeoaccnn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.snrcjt.cn/gtwsiibcig.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jinqigufen.top/gtyjlwseob.html

[Q15] 查询全部
来源：http://hz.jinghuilouyu.cn/gtbnfmwkux.html

SELECT * FROM users;
来源：http://hz.cashguo.top/gtguxjxhxc.html

[Q16] 查询指定列
来源：http://hz.yongpay.top/gtdfsalsom.html

SELECT id, name FROM users;
来源：http://hz.ydjk.org.cn/gtpwhlnfbt.html

[Q17] 条件查询
来源：http://hz.daxiang520.top/gtpunntgyz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jianghu66.top/gtoaphsxhr.html

[Q18] 模糊匹配
来源：http://hz.ydzc1.top/gtpjotvmic.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj20258888.top/gtzditqith.html

[Q19] 范围查询
来源：http://hz.havefunace.top/gtcexgrvfb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gtskxzdagc.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gtchziegco.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.nanxuanxn.top/gtmiyzkkte.html

[Q21] 空值判断
来源：http://hz.tanke756.top/gtwbhgwboi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.316326.xyz/gtvfulzyyv.html

[Q22] 排序
来源：http://hz.xingfuxueyuan.xyz/gttgjjusax.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydjk.org.cn/gtgwuhdrfx.html

[Q23] 分页
来源：http://hz.hywenlv.cn/gtzpvqgxja.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cqqwz.cn/gtflgsmaxz.html

[Q24] 去重
来源：http://hz.jlsjyb.cn/gtrnvoclaq.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gtartjyxzj.html

[Q25] 只取前 N 条
来源：http://hz.xinyue.icu/gtqrccldjs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hfpthk.cn/gtbcmunfxr.html

[Q26] 计数
来源：http://hz.xylfe.cn/gtjtskcpgp.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtkxkjznqy.html

[Q27] 条件计数
来源：http://hz.zhongyouzk.top/gtgzytuwnb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ppjwa.cn/gtyebaufag.html

[Q28] 求和与平均
来源：http://hz.ydjk.org.cn/gtskblzfhi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zycfv.cn/gtjllvxaaf.html

[Q29] 最大最小值
来源：http://hz.zhongyouzk.top/gtkuhjqyho.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yuxming.cn/gtukbyeywz.html

[Q30] 分组统计
来源：http://hz.jinqigfzy.top/gtmvuptejw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtwmpqtjqt.html

[Q31] 分组后过滤
来源：http://hz.quarkkingdee.top/gtetlerrum.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gzhubu.top/gtqurrpoat.html

[Q32] 分组拼接字符串
来源：http://hz.jinghuilouyu.cn/gtlsqcvqwx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtwxuptjxp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xylfe.cn/gtprnxsqhf.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtyvqnbeln.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtnbvbjwbo.html

[Q34] 每组取第一条
来源：http://hz.gotoacloud.top/gtfaadteew.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gtxtktbmhu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.svipenyu.cn/gtkjwdtgsd.html

) t WHERE rn = 1;
来源：http://hz.fengsongda.top/gtsqkudkrc.html

[Q35] 内连接
来源：http://hz.mhx1999.top/gtalosgujz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gttwflxzzq.html

[Q36] 左连接
来源：http://hz.mhx1999.top/gteyglehhw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtwmltcjxx.html

[Q37] 右连接
来源：http://hz.yj20258888.top/gtiabnjjld.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cucudq.cn/gtbztfqjdv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.kuanghao11.cn/gtvrazgvbj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenjidiqi.icu/gtuaqjxkzr.html

[Q39] 自连接（查上下级）
来源：http://hz.haohaochexian.top/gtjvytrixi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cheryme.top/gtyqytnfpq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shuidangran.top/gtgtfkyevw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydjk.org.cn/gtmkfyywzj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yj20258.top/gtramqszgx.html

[Q41] 多表连接
来源：http://hz.chenzaomai.com/gtswhumpne.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.bjfxy.top/gtdzcijpyc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.birdmap.top/gtdaeqlluh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.birdmap.top/gtjbypjwuf.html

[Q42] 连接条件附加过滤
来源：http://hz.cdnleiting.top/gtklcfkant.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pycfn.com/gthqkqxthw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.meibo888.top/gterhlptec.html

[Q43] 标量子查询
来源：http://hz.nwbrower.top/gtlzawhjie.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xinyue.icu/gtykhlzuyd.html

[Q44] IN 子查询
来源：http://hz.sweek.top/gtbqmpzcje.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tianlin.xyz/gteknkradd.html

[Q45] EXISTS 判断存在
来源：http://hz.nanxuanxn.top/gtdxdpfane.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hammf.cn/gttfwuzqqn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.iojbl.cn/gtmmtorkxp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtkhccvbpu.html

[Q47] 与平均值比较
来源：http://hz.zycfv.cn/gtqmwsdvqo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgufenzy.top/gtpxnzaold.html

[Q48] CTE 公用表表达式
来源：http://hz.meibo888.top/gtkdcomfup.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtrnfyizqn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xuanzx.com/gtvjyvxjhy.html

[Q49] 更新单行
来源：http://hz.mhx1999.top/gtxdexamew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.ppjwa.cn/gtvmrcretw.html

[Q50] 批量更新
来源：http://hz.nwbrower.top/gtyxdaxkgw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.aibaodan.cn/gtjpdwhdge.html

[Q51] 用子查询更新
来源：http://hz.zhiwuduotai.top/gtlqvsectq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shangyingyoupin.top/gtgltpvlmh.html

[Q52] 删除指定行
来源：http://hz.jyoumei.cn/gtrxxngitn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhengqikj.top/gtdfrynfrb.html

[Q53] 按条件删除
来源：http://hz.shuidangran.top/gttfvquyvy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtzjkdygnn.html

[Q54] 清空表
来源：http://hz.jinqigufen.top/gtgnbzwmcy.html

TRUNCATE TABLE logs;
来源：http://hz.ydzc1.top/gtovrrdoth.html

[Q55] 排名（并列占位）
来源：http://hz.haohaochexian.top/gtjvinguho.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pycfn.com/gtlhmnymde.html

[Q56] 密集排名（并列不占位）
来源：http://hz.9152youxi.cn/gtrhueqccz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jyoumei.cn/gthstsybpe.html

[Q57] 行号
来源：http://hz.pycfn.com/gtxsixcriy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gtyjdeydqa.html

[Q58] 累计求和
来源：http://hz.bjfxy.top/gtcovwxmad.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinqigufen.top/gtyyyvffhs.html

[Q59] 分组内累计
来源：http://hz.jinqigufen.top/gtaifvzhxx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtfrbkulfp.html

[Q60] 取上一行 / 下一行
来源：http://hz.hysaishi.cn/gtnrydaddd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sxryk.cn/gtynccnzdl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yvedp.cn/gtqptxdunq.html

[Q61] 移动平均
来源：http://hz.yj202588.top/gtdpufkqyc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daria6918.cn/gtnzvwrddn.html

[Q62] 分组占比
来源：http://hz.jinqigfzy.top/gtqmykcdhc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sufxvd.cn/gtqlkesgws.html

[Q63] 开启事务
来源：http://hz.316326.xyz/gtseporkni.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtbyepjymt.html

[Q64] 提交事务
来源：http://hz.sxryk.cn/gttxazszva.html

COMMIT;
来源：http://hz.yj20258.top/gtkwmjmifl.html

[Q65] 回滚事务
来源：http://hz.wangdashe.top/gteccpqdkm.html

ROLLBACK;
来源：http://hz.yuxming.cn/gtbhuiamsk.html

[Q66] 行锁查询
来源：http://hz.zhijiandao.cn/gtvqebwxhv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tanke756.top/gtjdjrijym.html

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gteuetsosu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zhongyouzk.top/gtommeefyt.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtfqjnkacj.html

SAVEPOINT sp1;
来源：http://hz.pengpengdd.cyou/gtmgqfmjft.html

ROLLBACK TO sp1;
来源：http://hz.zhixingplan.top/gtczyrgiyn.html

[Q69] 查看执行计划
来源：http://hz.svipenyu.cn/gtzzqymwpv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.iojbl.cn/gtfbczfeud.html

[Q70] 更新统计信息
来源：http://hz.sweek.top/gtzcyyyeed.html

ANALYZE TABLE users;
来源：http://hz.shangyingyoupin.top/gttpzhyjna.html

[Q71] 查看建表语句
来源：http://hz.xuetiantiany.cn/gtjqxunajz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.meibo888.top/gtdzamtjod.html

[Q72] 查看索引
来源：http://hz.zdqjudy.top/gtfzdvkkue.html

SHOW INDEX FROM users;
来源：http://hz.zhongyouzk.top/gtxxykusun.html

[Q73] 查看表状态
来源：http://hz.sxryk.cn/gtvhqjtcbp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.snrcjt.cn/gtnbqkbjdz.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gthrkvuixy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gttozdsadv.html

[Q75] 日期格式化
来源：http://hz.52xcode.cn/gtgdhlouwz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtnardiapv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtjeedouwd.html

[Q76] 按天统计
来源：http://hz.andypj.xyz/gtquvngefx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.meibo888.top/gtvrxmpfnz.html

[Q77] 时间加减
来源：http://hz.dianchejie.cn/gtvcrixbjy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ywan-chungtsiang.top/gtbsnezkdv.html

[Q78] 当前时间
来源：http://hz.nanxuanxn.top/gtizjautqm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtetbecrvi.html

[Q79] 字符串拼接
来源：http://hz.cashguo.top/gtqyykmdjw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yanxiufei.cn/gtifgupoyx.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gtynyvyerl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtvorcutyh.html

[Q81] 字符串替换
来源：http://hz.redwolf501.top/gtwvqngfxh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gtuygbnhcu.html


<!-- 参考信息 -->