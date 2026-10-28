代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.0kj1m.cn/gtsoncabay.html

C#:   lock (gate) { shared++; }
来源：http://hz.yonumen.top/gtraqjrzcs.html

[O04] 定义异步函数并等待
来源：http://hz.nwbrower.top/gtbljbhlbd.html

Py:   async def f():⏎    await g()
来源：http://hz.dashuyun.cn/gtqbqrildh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.chenjidiqi.icu/gtjdxocljw.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gtnzrxvwzd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhengqikj.top/gttecgasjl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gtapwymzmu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.tian-w.cn/gtrpnkueju.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hfpthk.cn/gtawrbfsye.html

C#:   async Task F() { await G(); }
来源：http://hz.yanxiufei.cn/gtjonpktyd.html

[O05] 并发执行并等待全部完成
来源：http://hz.feifeiyinyue.top/gtkxvjxitx.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daxiang520.top/gtzlkehhsb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtporobaej.html

JS:   await Promise.all(tasks)
来源：http://hz.bjfxy.top/gttewegeje.html

TS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtapmajcjk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shzxlz.cn/gtspjtytnl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.316326.xyz/gtihltennf.html

Ruby: threads.map(&:join)
来源：http://hz.xinyue.icu/gteqzgljku.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gzhubu.top/gtwrwickru.html

[O06] 使用进程池
来源：http://hz.52xcode.cn/gtphhaukmx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.daxiang520.top/gtvuymhknp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sufxvd.cn/gtioapuwms.html

JS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtnbdefbly.html

TS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtbozgplps.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.feifeiyinyue.top/gtuetxkhzm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtlhpyxueb.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtiseebgaz.html

C#:   Parallel.For
来源：http://hz.zhengqikj.top/gtgavffnbd.html

================================================================================
来源：http://hz.gogol.net.cn/gtagipxkkp.html

P. 常用工具函数
来源：http://hz.xuetiantiany.cn/gtfldihmxa.html

================================================================================
来源：http://hz.haohaochexian.top/gtcfwxyzie.html

[P01] 生成 UUID
来源：http://hz.nanxuanxn.top/gtmbggnkzt.html

Py:   str(uuid.uuid4())
来源：http://hz.yvedp.cn/gthexramov.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hywenlv.cn/gthffotpfn.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtsnxrsgun.html

TS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtporbnemr.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhiwuduotai.top/gtekfuusxq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtqizxxirz.html

Ruby: SecureRandom.uuid
来源：http://hz.hongshengwenyu.top/gtmxhdikkq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jiagoushi.top/gtszgrbdou.html

[P02] MD5 / SHA256 摘要
来源：http://hz.cucudq.cn/gtnfioaraj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.0kj1m.cn/gtetzucysa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shangyingyoupin.top/gtwvtjyqhf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtbwaoesjf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gtebypfcko.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gteuimtwix.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhaomingkeji.xyz/gtoyrvyobl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenlongwang.top/gtcyqxsjmu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydjk.org.cn/gtprhmbnvt.html

[P03] 生成短随机字符串
来源：http://hz.52xcode.cn/gtxtddauks.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangdashe.top/gtzzgzbuoq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jiagoushi.top/gtsskypudk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtdqizlrry.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtwkpitwyx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.meibo888.top/gtlgbuukkl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.fengsongda.top/gteqgzrhmq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.shzxlz.cn/gteqxliikd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yongpay.top/gtfrdxmglg.html

[P04] 求长度
来源：http://hz.sweek.top/gtcldpxiuk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hfpthk.cn/gtxcdxzofn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtgtrjjwua.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hammf.cn/gteggcnxej.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.gotoacloud.top/gtpdyqrgaf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtytdijkqw.html

Go:   len(arr);  len(m)
来源：http://hz.9152youxi.cn/gtgccvcdei.html

Ruby: x.length;  x.size
来源：http://hz.dianchejie.cn/gtvimjsqli.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxinkj.top/gtrupculfn.html

[P05] 判断两个对象内容是否相等
来源：http://hz.chenlongwang.top/gthogdxare.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jinqigufen.top/gttimzifwd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gzhubu.top/gtzhhqwtzf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.havefunace.top/gtjmbmjnjf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinghuilouyu.cn/gtmopxihbg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.meibo888.top/gtnxmniokl.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yvedp.cn/gtvufkbodb.html

Ruby: a == b
来源：http://hz.sufxvd.cn/gtdravbcxa.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.aizwys.cn/gtsbhgsayd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yongpay.top/gtgjiopslc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shuidangran.top/gtkdfqgxqu.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtwqwrtxxk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.jinqigufen.top/gtecdzgdjg.html

TS:   if (x == null) {}
来源：http://hz.9152youxi.cn/gtgepotlov.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shuidangran.top/gtywyksuwt.html

Go:   if x == nil {}
来源：http://hz.zhixingplan.top/gtjpikigjn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gzhubu.top/gtaalivmky.html

C#:   if (x is null) {}
来源：http://hz.shzxlz.cn/gtijylxmgz.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtshvqrvdk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jianghu66.top/gtqkcadlht.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtdizwkrxz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.pycfn.com/gtbvljvycp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.andypj.xyz/gtpnipicrx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jlsjyb.cn/gtfsdccbta.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xinyue.icu/gtydlvupjt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hywenlv.cn/gtriqxipqa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.wangshuangyany.cn/gttfnlsutk.html

[P08] 处理浮点精度问题
来源：http://hz.gzhubu.top/gtwmmdrphm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ywan-chungtsiang.top/gtsbxigkyt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.chenjidiqi.icu/gteoogpoof.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.haohaochexian.top/gtmpwierha.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jlsjyb.cn/gtdrntbayh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tanke756.top/gtplfkhjqz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.cucudq.cn/gtntzxwiit.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xuetiantiany.cn/gtqdwitbra.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.smart0.xyz/gtpjumcpde.html

================================================================================
来源：http://hz.ydzc1.top/gtqfhbapiz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhijiandao.cn/gttrhmpeuf.html

================================================================================
来源：http://hz.zhongyouzk.top/gtoxxgokjf.html

[Q01] 创建表
来源：http://hz.tianlin.xyz/gtcethpozt.html

CREATE TABLE users (
来源：http://hz.jinqigufen.top/gtnzobgtgb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.tianlin.xyz/gtxhezdcpd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.daria6918.cn/gtrllmeyhh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinghuilouyu.cn/gtdxbnqgra.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigfzy.top/gtcqjwkqoi.html

);
来源：http://hz.havefunace.top/gtvthmgeki.html

[Q02] 创建带外键的表
来源：http://hz.aibaodan.cn/gtjcphsumz.html

CREATE TABLE orders (
来源：http://hz.jinqigufen.top/gtcslntdif.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtxacrafvb.html

user_id INT NOT NULL,
来源：http://hz.chenzaomai.com/gtnonvuccc.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtlpxdcttw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.daria6918.cn/gtygkgryzl.html

);
来源：http://hz.sufxvd.cn/gtpjbypkds.html

[Q03] 增加列
来源：http://hz.feifeiyinyue.top/gtdjgqgvoz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.ppjwa.cn/gtavgfueze.html

[Q04] 修改列类型
来源：http://hz.jinyuanbaomall.cn/gtudvhdnin.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.kuanghao11.cn/gtnqvmumoo.html

[Q05] 重命名列
来源：http://hz.iojbl.cn/gtvxgjutin.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.pycfn.com/gttrwjffch.html

[Q06] 删除列
来源：http://hz.sweek.top/gttxhwmnam.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.c1oappe.top/gtsmbdohis.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtgxsoazaw.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tianlin.xyz/gtsbxwupds.html

[Q08] 创建普通索引
来源：http://hz.jqgfzy.top/gtvsvufzmo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtprlrbpfz.html

[Q09] 创建唯一索引
来源：http://hz.shzxlz.cn/gtdnrsjqji.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.fzhhl.top/gtqnjiplqr.html

[Q10] 插入单行
来源：http://hz.tanke756.top/gtbyrjzgkc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hysaishi.cn/gtrxqwppgz.html

[Q11] 一次插入多行
来源：http://hz.xziqi.cn/gtfyffxkvu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.sxryk.cn/gtkiejztzn.html

[Q12] 插入后取自增 ID
来源：http://hz.gzhubu.top/gtjionijhi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nwbrower.top/gtauvgkwua.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.0kj1m.cn/gtqlecnths.html

[Q13] 忽略重复插入
来源：http://hz.jianghu66.top/gtrfrlpzus.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.c1oappe.top/gtbbkywhoi.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtpavshxtb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.feifeiyinyue.top/gtonqhbnss.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cashguo.top/gtfkolgrec.html

[Q15] 查询全部
来源：http://hz.hnqzz.top/gtpqytmlcp.html

SELECT * FROM users;
来源：http://hz.wangdashe.top/gtfrlpfdjq.html

[Q16] 查询指定列
来源：http://hz.zhengqikj.top/gtojtlqeky.html

SELECT id, name FROM users;
来源：http://hz.cdnleiting.top/gtssnluwan.html

[Q17] 条件查询
来源：http://hz.jqgfzy.top/gtmijidcfj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zycfv.cn/gtephkwdkq.html

[Q18] 模糊匹配
来源：http://hz.yongpay.top/gtwyjnhklh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.pengpengdd.cyou/gtxvifaeer.html

[Q19] 范围查询
来源：http://hz.chenjidiqi.icu/gtqlfoxmqg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sysykeji.top/gtjswcyvkg.html

[Q20] IN 列表
来源：http://hz.ybcxt.top/gtuwctxgun.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtwcgxjdmx.html

[Q21] 空值判断
来源：http://hz.chenzaomai.com/gtsugbmzwo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shzxlz.cn/gttkcjbepy.html

[Q22] 排序
来源：http://hz.nanxuanxn.top/gtjqaydkeb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenjidiqi.icu/gtewnximkz.html

[Q23] 分页
来源：http://hz.havefunace.top/gttrfiwiji.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gotoacloud.top/gtzbsrezfv.html

[Q24] 去重
来源：http://hz.xingfuxueyuan.xyz/gtlrwirsol.html

SELECT DISTINCT city FROM users;
来源：http://hz.andypj.xyz/gtiyjqjbre.html

[Q25] 只取前 N 条
来源：http://hz.zdqjudy.top/gtnalmxpzn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hnqzz.top/gtgaxfbptj.html

[Q26] 计数
来源：http://hz.yj20258888.top/gtcvphenmz.html

SELECT COUNT(*) FROM users;
来源：http://hz.hywenlv.cn/gtuawwippx.html

[Q27] 条件计数
来源：http://hz.yuanzhike.top/gtpnsaovid.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.0kj1m.cn/gtcxlefsel.html

[Q28] 求和与平均
来源：http://hz.zhijiandao.cn/gtouxrodtx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.meibo888.top/gthpdjjvff.html

[Q29] 最大最小值
来源：http://hz.chenlongwang.top/gtckeeozvi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ybcxt.top/gtrugmojdx.html

[Q30] 分组统计
来源：http://hz.sysykeji.top/gtizbobfgp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtjglvgerr.html

[Q31] 分组后过滤
来源：http://hz.pengpengdd.cyou/gtssriehyf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.birdmap.top/gtpxnkvgqx.html

[Q32] 分组拼接字符串
来源：http://hz.jinqigufen.top/gtsfzqlvmw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgufenzy.top/gtnrntxwqz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtexvenkkp.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtewiyptle.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.9152youxi.cn/gtjmhvemxb.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtjpvklgmd.html

SELECT * FROM (
来源：http://hz.cdnleiting.top/gtfptcixir.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gtafbnfxeo.html

) t WHERE rn = 1;
来源：http://hz.jinqigufen.top/gtujwdauek.html

[Q35] 内连接
来源：http://hz.guannengcc.top/gtrbshfyrv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtlaxjdpxg.html

[Q36] 左连接
来源：http://hz.zycfv.cn/gtupjiitvx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhengqikj.top/gtiaadjyte.html

[Q37] 右连接
来源：http://hz.yongpay.top/gtgtmbcjbe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.mhx1999.top/gtrtjudbxb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tian-w.cn/gtrikslpvu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtzspfshye.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtsxertavf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuanzx.com/gtmrezcqcd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cashguo.top/gtjgekalqk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtupgirmtr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xingfuxueyuan.xyz/gtzwufbntg.html

[Q41] 多表连接
来源：http://hz.zdqjudy.top/gtogghhzjn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.havefunace.top/gtxdwppdsz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.snrcjt.cn/gtvkzbbyfn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.vqdsnc.cn/gtlvqkkqjt.html

[Q42] 连接条件附加过滤
来源：http://hz.dashuyun.cn/gtwelslnqv.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xziqi.cn/gtzxsgffvd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yonumen.top/gthtisvfbe.html

[Q43] 标量子查询
来源：http://hz.jinyuanbaomall.cn/gtgnfjxclw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.svipenyu.cn/gtaaivcrqy.html

[Q44] IN 子查询
来源：http://hz.zhixingplan.top/gtksgqverv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.wangshuangyany.cn/gttdkzgvcy.html

[Q45] EXISTS 判断存在
来源：http://hz.hnxiangtu.top/gtpthcwous.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.aizwys.cn/gtegzlvxnr.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigufen.top/gtiqbzcywh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gtihscqkgh.html

[Q47] 与平均值比较
来源：http://hz.52xcode.cn/gtrfayzuxu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.pycfn.com/gthyxmvivp.html

[Q48] CTE 公用表表达式
来源：http://hz.gaohongyu789.top/gtjpttxsmd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guannengcc.top/gtkjursgim.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.dianchejie.cn/gtlozwscpi.html

[Q49] 更新单行
来源：http://hz.jianghu66.top/gtwponwdjh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj202588.top/gtnyydzjrz.html

[Q50] 批量更新
来源：http://hz.ydjk.org.cn/gtiucntwkc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.daria6918.cn/gttzfxqkwf.html

[Q51] 用子查询更新
来源：http://hz.jinghuilouyu.cn/gtrspmbyni.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.wangdashe.top/gtwldsjcgt.html

[Q52] 删除指定行
来源：http://hz.snrcjt.cn/gtphvbexvr.html

DELETE FROM users WHERE id = 10;
来源：http://hz.meibo888.top/gttrwslvtl.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtqodnibjl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenjidiqi.icu/gtofmbuhhc.html

[Q54] 清空表
来源：http://hz.vqdsnc.cn/gtiaxbyzce.html

TRUNCATE TABLE logs;
来源：http://hz.hammf.cn/gtxhstunsq.html

[Q55] 排名（并列占位）
来源：http://hz.cqqwz.cn/gtrnxofbcx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtdzrtxvhi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hnqzz.top/gtynkhuqcs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yonumen.top/gtuagelzux.html

[Q57] 行号
来源：http://hz.jyoumei.cn/gtehzpzjcv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtoyekbuco.html

[Q58] 累计求和
来源：http://hz.yj202588.top/gtcftcnhfh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hysaishi.cn/gtsgpzcktf.html

[Q59] 分组内累计
来源：http://hz.shanyushiyangtech.top/gtpfbhicxe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.c1oappe.top/gtiagvutqa.html

[Q60] 取上一行 / 下一行
来源：http://hz.kuanghao11.cn/gtsplzsxmy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hongshengwenyu.top/gtdrghntmp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtyynpqlsj.html

[Q61] 移动平均
来源：http://hz.yvedp.cn/gtwewjhmcq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hysaishi.cn/gthzzsmejg.html

[Q62] 分组占比
来源：http://hz.guannengcc.top/gtzjnijxti.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gttwbqzjts.html

[Q63] 开启事务
来源：http://hz.zdqjudy.top/gttmjvvagq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cashguo.top/gtbxfndlfq.html

[Q64] 提交事务
来源：http://hz.chenzaomai.com/gtgpadvgmm.html

COMMIT;
来源：http://hz.ydzc1.top/gtavbhjyay.html

[Q65] 回滚事务
来源：http://hz.ehwqpu.com/gtgbzqfebf.html

ROLLBACK;
来源：http://hz.yj20258.top/gtfbhqywvp.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtunhyuvlf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hammf.cn/gtiwniggli.html

[Q67] 设置隔离级别
来源：http://hz.jlsjyb.cn/gtjlssqsae.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ybcxt.top/gtlvikohuy.html

[Q68] 保存点
来源：http://hz.wangshuangyany.cn/gtoxhmmadk.html

SAVEPOINT sp1;
来源：http://hz.yangfankeji.com/gtdxlgmpme.html

ROLLBACK TO sp1;
来源：http://hz.cashguo.top/gtjwcojxvj.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gtsjapsoel.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yuxming.cn/gtdrigrmav.html

[Q70] 更新统计信息
来源：http://hz.jianghu66.top/gtsiuloicz.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtpvmfmxha.html

[Q71] 查看建表语句
来源：http://hz.jlsjyb.cn/gtkyeozjmk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ehwqpu.com/gtuyuspsdq.html

[Q72] 查看索引
来源：http://hz.chenlongwang.top/gtzlqcpvzo.html

SHOW INDEX FROM users;
来源：http://hz.yongpay.top/gtvbbhsyuh.html

[Q73] 查看表状态
来源：http://hz.cucudq.cn/gtbrgncjoh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yonumen.top/gtvbgtdghz.html

[Q74] 强制使用索引
来源：http://hz.gotoacloud.top/gtnpyxlegy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xinyue.icu/gtmflklpit.html

[Q75] 日期格式化
来源：http://hz.xuetiantiany.cn/gthrklfidd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shuidangran.top/gtpqhulvco.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtcvitfifs.html

[Q76] 按天统计
来源：http://hz.zdqjudy.top/gtpcjidvmw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.9152youxi.cn/gtniysnpdd.html

[Q77] 时间加减
来源：http://hz.cucudq.cn/gtbbuqavzz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hammf.cn/gthpnozwpq.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtuwasihxi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tanke756.top/gtdzoyzldh.html

[Q79] 字符串拼接
来源：http://hz.guowangkeji.top/gtlrygosra.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtgfehwfni.html

[Q80] 字符串截取
来源：http://hz.ydzc1.top/gtnzthpgde.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yongpay.top/gtwaplurrm.html

[Q81] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtpcywjpjs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj20258888.top/gtgrmwongq.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtenwaqwtt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtvokcbmil.html

[Q83] 大小写转换
来源：http://hz.chenzaomai.com/gtdoippung.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xinyue.icu/gtwstbwtwu.html

[Q84] 去除首尾空格
来源：http://hz.daxiang520.top/gtsgkxpjrb.html

SELECT TRIM(name) FROM users;
来源：http://hz.havefunace.top/gtcujrabda.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtiivwnsgh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zdqjudy.top/gtdoxudvmh.html


<!-- 参考信息 -->