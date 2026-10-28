代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ehwqpu.com/gtnwensiqb.html

C#:   lock (gate) { shared++; }
来源：http://hz.sxryk.cn/gtwxgymyyi.html

[O04] 定义异步函数并等待
来源：http://hz.zhaomingkeji.xyz/gtkljgcmyx.html

Py:   async def f():⏎    await g()
来源：http://hz.nwbrower.top/gtdwzfxhts.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gtmwsmrxxj.html

JS:   async function f() { await g(); }
来源：http://hz.xuanzx.com/gtnwkbjhjx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.havefunace.top/gttimlwirb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ywan-chungtsiang.top/gtcuzeifbv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gaohongyu789.top/gtdocyvlsu.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gzhubu.top/gtmccfzmmg.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtutmehmrs.html

[O05] 并发执行并等待全部完成
来源：http://hz.jlsjyb.cn/gtqzajtjzy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cashguo.top/gtagzvzzjh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.meibo888.top/gtvaefaxdo.html

JS:   await Promise.all(tasks)
来源：http://hz.xinyue.icu/gtuljrxjrg.html

TS:   await Promise.all(tasks)
来源：http://hz.nanxinkj.top/gtlyvcmepx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.andypj.xyz/gtyegmybbu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ivvv.top/gtfvtxnqgf.html

Ruby: threads.map(&:join)
来源：http://hz.sweek.top/gtwubeuyit.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jiagoushi.top/gtzestfjwj.html

[O06] 使用进程池
来源：http://hz.zdqjudy.top/gteanybbxk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ybcxt.top/gtalynbnlw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tianlin.xyz/gtobojhwkm.html

JS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtcxaalakq.html

TS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtsssqgcrp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.0kj1m.cn/gtthuaygeu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zdqjudy.top/gttkiciqfg.html

Ruby: // fork 块
来源：http://hz.quarkkingdee.top/gtzwevpajp.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtkqkcuxpj.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgtmstlsu.html

P. 常用工具函数
来源：http://hz.guowangkeji.top/gtfnbgfxod.html

================================================================================
来源：http://hz.snrcjt.cn/gtoviqmquq.html

[P01] 生成 UUID
来源：http://hz.iojbl.cn/gtbslnjrko.html

Py:   str(uuid.uuid4())
来源：http://hz.andypj.xyz/gteuniojti.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pengpengdd.cyou/gtqiuwlhwy.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtgexmhbda.html

TS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtiffeggtc.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtddhgsqcj.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydzc1.top/gtqlacbpgn.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtcimqylfm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.316326.xyz/gtsziazjne.html

[P02] MD5 / SHA256 摘要
来源：http://hz.nanxuanxn.top/gtzehawrfo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.zhoulong.xyz/gthgifirad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.svipenyu.cn/gtfxmyvumx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.hnqzz.top/gtclzrsyhy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aibaodan.cn/gtaqecpqer.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.chenlongwang.top/gttmgfumyj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hysaishi.cn/gtqsrwuyde.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aibaodan.cn/gtetesqict.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.meibo888.top/gtswiozjfy.html

[P03] 生成短随机字符串
来源：http://hz.feifeiyinyue.top/gtrlkymtse.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cdnleiting.top/gtjtxwjocg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.316326.xyz/gtucqvxopw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtdyukgfti.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.fengsongda.top/gtpqmpdaot.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.zhaomingkeji.xyz/gtpjqfxiuo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuetiantiany.cn/gtnwsmyecv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jyoumei.cn/gtvjwixeej.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ybcxt.top/gthhdtyipd.html

[P04] 求长度
来源：http://hz.ivvv.top/gtftskatwj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sysykeji.top/gteavsrcic.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtwoxbwgum.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.quarkkingdee.top/gtfiengolb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gtkrqpvjjf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.c1oappe.top/gtimhpotmw.html

Go:   len(arr);  len(m)
来源：http://hz.iojbl.cn/gtbatzpwbm.html

Ruby: x.length;  x.size
来源：http://hz.zhijiandao.cn/gtnhdqztrj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hongshengwenyu.top/gtewledeay.html

[P05] 判断两个对象内容是否相等
来源：http://hz.dianchejie.cn/gtepkcjbze.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.quarkkingdee.top/gtddwkcjbx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.fengsongda.top/gtlktbpqza.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtxxznybls.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtagoepsqr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.bjfxy.top/gtzoweuuth.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jlsjyb.cn/gtyomxgfun.html

Ruby: a == b
来源：http://hz.zdqjudy.top/gtnkdrxsjp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhongyouzk.top/gtbxvhwfru.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jqgfzy.top/gtgyrhczwd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sxryk.cn/gtikywhnbl.html

PHP:  if (empty($x)) {}
来源：http://hz.jiagoushi.top/gtkwhtlvnv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.shuidangran.top/gtraxdmksy.html

TS:   if (x == null) {}
来源：http://hz.shuidangran.top/gttbtjlwhz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtswkuzcvg.html

Go:   if x == nil {}
来源：http://hz.shangyingyoupin.top/gtyhhupgmf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydjk.org.cn/gtusiwmvmf.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtkizkvlby.html

[P07] 防抖与节流
来源：http://hz.tanke756.top/gtsbabongc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.vqdsnc.cn/gtmcgxsrgc.html

PHP:  // 手写时间戳比较
来源：http://hz.316326.xyz/gtpxtoytwc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtjlfzoujd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gtcboakagv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.cqqwz.cn/gtxrbospgj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.c1oappe.top/gtusepycmh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.shuidangran.top/gtaxwdiujh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gzhubu.top/gtaraxvekt.html

[P08] 处理浮点精度问题
来源：http://hz.hongshengwenyu.top/gtwyvsqpqu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.fengsongda.top/gtwavwhhxn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.sweek.top/gttvkfsloe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sweek.top/gtfyvmnyoo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yuanzhike.top/gtfhzcpsdv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.feifeiyinyue.top/gtnghyknai.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.bjfxy.top/gtyxutgdrv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.0kj1m.cn/gtykmkkofg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhengqikj.top/gtmgofzmwn.html

================================================================================
来源：http://hz.xinyue.icu/gtmdwhncth.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jianghu66.top/gtsqpmeuoe.html

================================================================================
来源：http://hz.daria6918.cn/gtzojscdww.html

[Q01] 创建表
来源：http://hz.ydjk.org.cn/gtxjkcaapg.html

CREATE TABLE users (
来源：http://hz.dianchejie.cn/gtvhvdqepv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenlongwang.top/gtfpqrtbjk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xuanzx.com/gtehkjoaar.html

email VARCHAR(100) UNIQUE,
来源：http://hz.meibo888.top/gtdprxzweb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ehwqpu.com/gtbxrazohy.html

);
来源：http://hz.kuanghao11.cn/gtvhvqgavo.html

[Q02] 创建带外键的表
来源：http://hz.aizwys.cn/gtnukjthla.html

CREATE TABLE orders (
来源：http://hz.jinghuilouyu.cn/gtagddobrv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gttgkendkg.html

user_id INT NOT NULL,
来源：http://hz.c1oappe.top/gtyyxsueza.html

amount DECIMAL(10, 2),
来源：http://hz.gotoacloud.top/gtdwkdcujn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.feifeiyinyue.top/gtwdafxsij.html

);
来源：http://hz.316326.xyz/gtscdeslxo.html

[Q03] 增加列
来源：http://hz.xuanzx.com/gtohfyabaz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gtaqrhrpzt.html

[Q04] 修改列类型
来源：http://hz.chenlongwang.top/gtpedfmgim.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gogol.net.cn/gtrolgizod.html

[Q05] 重命名列
来源：http://hz.jiagoushi.top/gtimxwuiot.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhoulong.xyz/gtpyhepxui.html

[Q06] 删除列
来源：http://hz.yj202588.top/gtkygqtsdx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.snrcjt.cn/gtlyivytxo.html

[Q07] 删除表
来源：http://hz.jinqigufen.top/gtcbkurfio.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cdnleiting.top/gtdmbwctjl.html

[Q08] 创建普通索引
来源：http://hz.meibo888.top/gtfccqgsau.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtqsqhfrah.html

[Q09] 创建唯一索引
来源：http://hz.gotoacloud.top/gtpyravzpx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinqigufen.top/gttgxygvqg.html

[Q10] 插入单行
来源：http://hz.gaohongyu789.top/gtxrlcdzgz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jinghuilouyu.cn/gtdzgyzrpq.html

[Q11] 一次插入多行
来源：http://hz.redwolf501.top/gtxudtbyxy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhongyouzk.top/gtmcvuzecs.html

[Q12] 插入后取自增 ID
来源：http://hz.zdqjudy.top/gtvxymfxcq.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.0kj1m.cn/gtlhzgpibu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jqgfzy.top/gtbbgdnvbm.html

[Q13] 忽略重复插入
来源：http://hz.xuetiantiany.cn/gtioekmtpu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ehwqpu.com/gthxtinlhi.html

[Q14] 存在则更新（upsert）
来源：http://hz.c1oappe.top/gtivbccvgu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nanxuanxn.top/gtktpvawzx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nwbrower.top/gtcmlkbjec.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtkmwbubii.html

SELECT * FROM users;
来源：http://hz.yj20258888.top/gthbsqpcrz.html

[Q16] 查询指定列
来源：http://hz.ywan-chungtsiang.top/gtdigsclkz.html

SELECT id, name FROM users;
来源：http://hz.shuidangran.top/gtibgacsos.html

[Q17] 条件查询
来源：http://hz.kuanghao11.cn/gtiwxboyiq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.andypj.xyz/gtrilbwfzo.html

[Q18] 模糊匹配
来源：http://hz.aizwys.cn/gtqgpgomnc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhoulong.xyz/gtgbbeuyrv.html

[Q19] 范围查询
来源：http://hz.zycfv.cn/gtzewvxhil.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shangyingyoupin.top/gtyikuykkh.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gtrlomnigq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gogol.net.cn/gtylzwdecq.html

[Q21] 空值判断
来源：http://hz.shuidangran.top/gtjtjeljne.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gtjcdyoofk.html

[Q22] 排序
来源：http://hz.hysaishi.cn/gtksrbmbaz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydjk.org.cn/gtvmagwhec.html

[Q23] 分页
来源：http://hz.fzhhl.top/gtlbwinmdr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxuanxn.top/gtdjajetgo.html

[Q24] 去重
来源：http://hz.nwbrower.top/gtfzdxwjnm.html

SELECT DISTINCT city FROM users;
来源：http://hz.fengsongda.top/gtuumngpkm.html

[Q25] 只取前 N 条
来源：http://hz.shangyingyoupin.top/gtltlnfnye.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gtnbscgjux.html

[Q26] 计数
来源：http://hz.wangshuangyany.cn/gtxknbwfrm.html

SELECT COUNT(*) FROM users;
来源：http://hz.fzhhl.top/gtavotckaj.html

[Q27] 条件计数
来源：http://hz.yueranfly.top/gtsbrfvruy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ydjk.org.cn/gtnwnyhxgl.html

[Q28] 求和与平均
来源：http://hz.tian-w.cn/gtdwfmzrer.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jyoumei.cn/gtbyvacenk.html

[Q29] 最大最小值
来源：http://hz.yangfankeji.com/gtudlgnilq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gtbvskzmgp.html

[Q30] 分组统计
来源：http://hz.hnxiangtu.top/gtzbbtmkgb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtpyprpqcy.html

[Q31] 分组后过滤
来源：http://hz.316326.xyz/gtwyiqamtz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gtginavgri.html

[Q32] 分组拼接字符串
来源：http://hz.316326.xyz/gtoeifkico.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtrrcjnlvm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sxryk.cn/gtcjqhbrfc.html

[Q33] 多列分组
来源：http://hz.shanyushiyangkeji.top/gtnqukjezo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jqgfzy.top/gtedtvlznj.html

[Q34] 每组取第一条
来源：http://hz.ydzc1.top/gtotkyczkc.html

SELECT * FROM (
来源：http://hz.pengpengdd.cyou/gtrgiaixfj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.redwolf501.top/gtlcrvjvia.html

) t WHERE rn = 1;
来源：http://hz.chenjidiqi.icu/gtqyyshyrq.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtkfiopwyf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gthocnbjbg.html

[Q36] 左连接
来源：http://hz.feifeiyinyue.top/gtbmydwiea.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gaohongyu789.top/gtyqsmvpzq.html

[Q37] 右连接
来源：http://hz.yueranfly.top/gtihcskrwd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ydjk.org.cn/gtuhjdioko.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuetiantiany.cn/gtqjbryqbp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zdqjudy.top/gtrolvyzly.html

[Q39] 自连接（查上下级）
来源：http://hz.zhijiandao.cn/gtxndwwkwt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.vqdsnc.cn/gthosmonko.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.9152youxi.cn/gtnylnstzn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhaomingkeji.xyz/gtezbwlodm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.vqdsnc.cn/gtrzdwepsd.html

[Q41] 多表连接
来源：http://hz.shuidangran.top/gtpfsdvtth.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtwsuxgvws.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yangfankeji.com/gtyjlmfobj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigfzy.top/gtzltjbrtj.html

[Q42] 连接条件附加过滤
来源：http://hz.ehwqpu.com/gtiavkylux.html

SELECT u.name, o.amount FROM users u
来源：http://hz.c1oappe.top/gtyabszwvz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtklgopppm.html

[Q43] 标量子查询
来源：http://hz.jlsjyb.cn/gtcuorpntp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.dianchejie.cn/gtcxwglhni.html

[Q44] IN 子查询
来源：http://hz.quarkkingdee.top/gtvugrtfcc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ydzc1.top/gteskgteru.html

[Q45] EXISTS 判断存在
来源：http://hz.havefunace.top/gtclmnmbuq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtnsxdkcgu.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinyuanbaomall.cn/gtfudazmcz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuxming.cn/gtcktuberk.html

[Q47] 与平均值比较
来源：http://hz.jinghuilouyu.cn/gtijgwhwbr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cdnleiting.top/gtwuydkqxk.html

[Q48] CTE 公用表表达式
来源：http://hz.aibaodan.cn/gtxmwjyuxa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.feifeiyinyue.top/gtxgidydme.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtxsivigvm.html

[Q49] 更新单行
来源：http://hz.svipenyu.cn/gtqvyhezlh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.daxiang520.top/gtbodmzphs.html

[Q50] 批量更新
来源：http://hz.hfpthk.cn/gtxvpvqhif.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yuxming.cn/gtxwlmaxqa.html

[Q51] 用子查询更新
来源：http://hz.sweek.top/gtmkuskocj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhijiandao.cn/gtfckvyfih.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtlhjntjqf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.cdnleiting.top/gtqlpiayjp.html

[Q53] 按条件删除
来源：http://hz.vqdsnc.cn/gtjexcjysn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.smart0.xyz/gtktdgfdeg.html

[Q54] 清空表
来源：http://hz.gzhubu.top/gtghwaqqhp.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gtdohnhugw.html

[Q55] 排名（并列占位）
来源：http://hz.zdqjudy.top/gtbavjbhas.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tian-w.cn/gtihtduenm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gzhubu.top/gtnjilozno.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shanyushiyangkeji.top/gtztstqndh.html

[Q57] 行号
来源：http://hz.vqdsnc.cn/gtjhdmogfi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.havefunace.top/gtapfhrahz.html

[Q58] 累计求和
来源：http://hz.hnxiangtu.top/gtzgwxxvbi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.dashuyun.cn/gtqhwrldhp.html

[Q59] 分组内累计
来源：http://hz.dianchejie.cn/gtjqzqjyyd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shangyingyoupin.top/gtarcqpsfa.html

[Q60] 取上一行 / 下一行
来源：http://hz.gzhubu.top/gtxxohtfdb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.pengpengdd.cyou/gtuzsejhbw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtaagmoite.html

[Q61] 移动平均
来源：http://hz.sufxvd.cn/gtveggsfsg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gtwzhwchop.html

[Q62] 分组占比
来源：http://hz.jinghuilouyu.cn/gtixifqlzb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtsndnhyfs.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gtcrkaiktn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhengqikj.top/gtshznjmgz.html

[Q64] 提交事务
来源：http://hz.jyoumei.cn/gtcujvkuwg.html

COMMIT;
来源：http://hz.hfpthk.cn/gtjtqxbsbo.html

[Q65] 回滚事务
来源：http://hz.xuanzx.com/gtlvzjblcl.html

ROLLBACK;
来源：http://hz.sweek.top/gtnuxfnsti.html

[Q66] 行锁查询
来源：http://hz.xuetiantiany.cn/gtzyaslxyj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pengpengdd.cyou/gtejgjnttv.html

[Q67] 设置隔离级别
来源：http://hz.quarkkingdee.top/gtcfpcdmza.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtexwvocsg.html

[Q68] 保存点
来源：http://hz.birdmap.top/gtambrkdbr.html

SAVEPOINT sp1;
来源：http://hz.mhx1999.top/gtlphvvoej.html

ROLLBACK TO sp1;
来源：http://hz.yj20258.top/gtrbmsvgfp.html

[Q69] 查看执行计划
来源：http://hz.nanxuanxn.top/gtjwibbgxa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinyuanbaomall.cn/gtchwcfpnw.html

[Q70] 更新统计信息
来源：http://hz.jinqigfzy.top/gtktaspcxb.html

ANALYZE TABLE users;
来源：http://hz.shuidangran.top/gtyjvbuiad.html

[Q71] 查看建表语句
来源：http://hz.pengpengdd.cyou/gtzmcovqdn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.aibaodan.cn/gtdzfnspah.html

[Q72] 查看索引
来源：http://hz.shanyushiyangkeji.top/gtsiqpsyij.html

SHOW INDEX FROM users;
来源：http://hz.zhaomingkeji.xyz/gtgpndppfd.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtkihpirlz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ppjwa.cn/gtrhdffrqi.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gtltdruogb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.quarkkingdee.top/gthafbjaql.html

[Q75] 日期格式化
来源：http://hz.zhiwuduotai.top/gthbprdscv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.feifeiyinyue.top/gtqiknsqlv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtuxxflybd.html

[Q76] 按天统计
来源：http://hz.tian-w.cn/gtefyrlrxm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtparetamz.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtkvpmmxcn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtvkzsstzj.html

[Q78] 当前时间
来源：http://hz.fzhhl.top/gtueqwlzuy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jyoumei.cn/gtskkptagk.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtznhioybv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuanzhike.top/gtotogwmyo.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gtqqthkumf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gotoacloud.top/gtmtjctpzx.html

[Q81] 字符串替换
来源：http://hz.zhiwuduotai.top/gtbohakfco.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ivvv.top/gtmloxztqa.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gthdmlabrh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dashuyun.cn/gtejaoxgze.html

[Q83] 大小写转换
来源：http://hz.zhijiandao.cn/gtccoalxbe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nwbrower.top/gtuvzzxrpy.html

[Q84] 去除首尾空格
来源：http://hz.daria6918.cn/gtdiviwahz.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtpnhwytjf.html

[Q85] 数值取整
来源：http://hz.kuanghao11.cn/gthmbmkdnn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gtltrsgsfn.html


<!-- 参考信息 -->