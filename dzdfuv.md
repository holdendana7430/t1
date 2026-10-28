代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtsvopfzob.html

JS:   async function f() { await g(); }
来源：http://hz.jyoumei.cn/gtonajfjqz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xinyue.icu/gtyquvhnad.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aizwys.cn/gtndebgkuo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sweek.top/gtkvrwuhmz.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtmvgwbndk.html

C#:   async Task F() { await G(); }
来源：http://hz.jlsjyb.cn/gtodamcpzq.html

[O05] 并发执行并等待全部完成
来源：http://hz.zdqjudy.top/gtaeaqcwul.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuanzx.com/gtvpuryooh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtsagvpcqx.html

JS:   await Promise.all(tasks)
来源：http://hz.zhongyouzk.top/gtyhirsphy.html

TS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtciavydzs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yangfankeji.com/gtctqxmkvy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gzhubu.top/gtoqdrlsvk.html

Ruby: threads.map(&:join)
来源：http://hz.gotoacloud.top/gtzyjmixqy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hfpthk.cn/gtcomlvjsb.html

[O06] 使用进程池
来源：http://hz.zhixingplan.top/gtqokltodn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cheryme.top/gtqgncocsd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.feifeiyinyue.top/gtszbxqxhp.html

JS:   // child_process / cluster 模块
来源：http://hz.zhongyouzk.top/gtcxodfneq.html

TS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtavvaozar.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.tian-w.cn/gtrgyviuot.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xuetiantiany.cn/gtkhonimkb.html

Ruby: // fork 块
来源：http://hz.jinqigfzy.top/gtgwbjuprs.html

C#:   Parallel.For
来源：http://hz.chenzaomai.com/gtzxdqxxqy.html

================================================================================
来源：http://hz.cashguo.top/gtlnnmvgrh.html

P. 常用工具函数
来源：http://hz.yj202588.top/gtrbpaauco.html

================================================================================
来源：http://hz.chenlongwang.top/gthyhdowtg.html

[P01] 生成 UUID
来源：http://hz.zhengqikj.top/gtdikxkjce.html

Py:   str(uuid.uuid4())
来源：http://hz.vqdsnc.cn/gtzeuyyyjl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xingfuxueyuan.xyz/gtnxsaxcxc.html

JS:   crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtvbyhdtfg.html

TS:   crypto.randomUUID()
来源：http://hz.guannengcc.top/gtufmbpmtg.html

Java: UUID.randomUUID().toString()
来源：http://hz.jinqigfzy.top/gttgefrcll.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sweek.top/gtmubtnukd.html

Ruby: SecureRandom.uuid
来源：http://hz.zhiwuduotai.top/gtkvidonoj.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhixingplan.top/gtzezvtbhp.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yuxming.cn/gtdssdqjje.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xuetiantiany.cn/gtowpoukje.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.meibo888.top/gtcwqioxms.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgfzy.top/gtilwxbkpp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pycfn.com/gtaefesged.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.snrcjt.cn/gtllihuono.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cqqwz.cn/gtpsviqivg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.0kj1m.cn/gtrbvzqohk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shuidangran.top/gtrgzujxjg.html

[P03] 生成短随机字符串
来源：http://hz.hammf.cn/gtaaufoojq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.pycfn.com/gtxuiyjxxn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhixingplan.top/gtyvzpfmbs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.dashuyun.cn/gtzegmdnzj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jiagoushi.top/gtyiqhbeht.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hfpthk.cn/gtjfgigcfh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.0kj1m.cn/gtvnxmaqwc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ppjwa.cn/gtntehfrzo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydzc1.top/gtmhlhuqgz.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gtebybvmpj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sufxvd.cn/gtdxndajqr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtfyyyefuq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yvedp.cn/gtvqjlvdze.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.cheryme.top/gtwfkjhids.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nanxinkj.top/gtxrvnfxlw.html

Go:   len(arr);  len(m)
来源：http://hz.yuxming.cn/gtiodileqh.html

Ruby: x.length;  x.size
来源：http://hz.gzhubu.top/gtpfdbpowl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.xziqi.cn/gtsfqlkdzi.html

[P05] 判断两个对象内容是否相等
来源：http://hz.gzhubu.top/gtqckxmwno.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jiagoushi.top/gtubkykpbr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.aizwys.cn/gtjujnanhf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hysaishi.cn/gtgybtadwe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jlsjyb.cn/gtbnvqwpwr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xylfe.cn/gtjvxeerhg.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhixingplan.top/gtbdemwfeg.html

Ruby: a == b
来源：http://hz.shuidangran.top/gtjxpqotpq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtzpvqosuy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.shanyushiyangkeji.top/gtkopfzoia.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.pengpengdd.cyou/gtmnkhpxsg.html

PHP:  if (empty($x)) {}
来源：http://hz.9152youxi.cn/gtdljqkwlg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.vqdsnc.cn/gtbkbgmuzu.html

TS:   if (x == null) {}
来源：http://hz.cdnleiting.top/gtokskvsho.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtbifigkjc.html

Go:   if x == nil {}
来源：http://hz.shzxlz.cn/gtsjmgbkye.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jlsjyb.cn/gtkefwgbwc.html

C#:   if (x is null) {}
来源：http://hz.sufxvd.cn/gtnflmxjdg.html

[P07] 防抖与节流
来源：http://hz.316326.xyz/gtwffkvepz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.smart0.xyz/gtmbdjiezd.html

PHP:  // 手写时间戳比较
来源：http://hz.ivvv.top/gtluftacfk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tianlin.xyz/gtdnauwdor.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtzofhkowu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jqgufenzy.top/gtoaazkddd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.zhengqikj.top/gthokcmyvj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj202588.top/gtzostkfok.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ybcxt.top/gtdddihsln.html

[P08] 处理浮点精度问题
来源：http://hz.gaohongyu789.top/gtvtmdajda.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.hywenlv.cn/gtadfxdksx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daxiang520.top/gtrmtqeuvj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.pycfn.com/gtdynmxcjo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yj20258888.top/gtrntlmmma.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.shzxlz.cn/gtdntzzokr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yonumen.top/gtpzshxjai.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.xziqi.cn/gthleskoeg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yuanzhike.top/gtoamrbtda.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmxsdlygr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.guowangkeji.top/gtzrajknco.html

================================================================================
来源：http://hz.jqgufenzy.top/gtyisehljj.html

[Q01] 创建表
来源：http://hz.wangdashe.top/gtblczgkgp.html

CREATE TABLE users (
来源：http://hz.shzxlz.cn/gtpbbzkzbd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhiwuduotai.top/gtfrlcwrlc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hammf.cn/gtoqucqglh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.ydzc1.top/gtocmxurkc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yongpay.top/gtbdhdslqb.html

);
来源：http://hz.ivvv.top/gtctseolel.html

[Q02] 创建带外键的表
来源：http://hz.zhaomingkeji.xyz/gtbvcocptd.html

CREATE TABLE orders (
来源：http://hz.iojbl.cn/gtezrzppwh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yuanzhike.top/gtfbubtkwr.html

user_id INT NOT NULL,
来源：http://hz.yongpay.top/gtdzjwcmwk.html

amount DECIMAL(10, 2),
来源：http://hz.nwbrower.top/gtqjlihpyn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhengqikj.top/gtexihutbo.html

);
来源：http://hz.zhengqikj.top/gtguwcezyb.html

[Q03] 增加列
来源：http://hz.guannengcc.top/gtjrkugkwc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.xuetiantiany.cn/gtpqvyxdhr.html

[Q04] 修改列类型
来源：http://hz.yanxiufei.cn/gthvgplhiq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yonumen.top/gtftoxuzbo.html

[Q05] 重命名列
来源：http://hz.sweek.top/gtgxbvsklm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinqigfzy.top/gtolbxpztk.html

[Q06] 删除列
来源：http://hz.hnqzz.top/gttvhqanso.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hfpthk.cn/gtpjbgbwlj.html

[Q07] 删除表
来源：http://hz.daria6918.cn/gtclhlisph.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gtqnfvdans.html

[Q08] 创建普通索引
来源：http://hz.shuidangran.top/gtqzgmjebb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zhijiandao.cn/gtbqitgwje.html

[Q09] 创建唯一索引
来源：http://hz.jianghu66.top/gtyqtzlvex.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jqgufenzy.top/gtxxkhvrqe.html

[Q10] 插入单行
来源：http://hz.svipenyu.cn/gtrlmidseb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gtfurzjdgt.html

[Q11] 一次插入多行
来源：http://hz.shanyushiyangkeji.top/gtgetywuzu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.pycfn.com/gtlptkjlcc.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtjlzsgvfz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.0kj1m.cn/gtonjdfjcd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nwbrower.top/gtibcnigud.html

[Q13] 忽略重复插入
来源：http://hz.zhiwuduotai.top/gtqmwisysl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hysaishi.cn/gtwsqrpsjk.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gthkuhbdyy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hywenlv.cn/gtwssrodfj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jianghu66.top/gtwfaidoop.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gtwxjccjqw.html

SELECT * FROM users;
来源：http://hz.tian-w.cn/gtxguqhrhu.html

[Q16] 查询指定列
来源：http://hz.xuetiantiany.cn/gtaodbpnoc.html

SELECT id, name FROM users;
来源：http://hz.daria6918.cn/gtcszibjlx.html

[Q17] 条件查询
来源：http://hz.cqqwz.cn/gtavjivnue.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hnqzz.top/gtsnfkxiuw.html

[Q18] 模糊匹配
来源：http://hz.xylfe.cn/gtkhjekcwn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hnqzz.top/gtnranrwbl.html

[Q19] 范围查询
来源：http://hz.cdnleiting.top/gtwxaztzfx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.svipenyu.cn/gtopkaqdfe.html

[Q20] IN 列表
来源：http://hz.jianghu66.top/gttqfahqkf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yangfankeji.com/gtdoipvwdk.html

[Q21] 空值判断
来源：http://hz.gogol.net.cn/gtfholxtpz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zycfv.cn/gtebzcvqku.html

[Q22] 排序
来源：http://hz.shangyingyoupin.top/gtppnsfqkl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.redwolf501.top/gtsztsessc.html

[Q23] 分页
来源：http://hz.jlsjyb.cn/gtbyhnpgpe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.0kj1m.cn/gtjbocdjau.html

[Q24] 去重
来源：http://hz.tanke756.top/gtmkpnzzfa.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj202588.top/gthjseneye.html

[Q25] 只取前 N 条
来源：http://hz.zhijiandao.cn/gtydzkemsa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.52xcode.cn/gtlvvzjcqp.html

[Q26] 计数
来源：http://hz.cqqwz.cn/gtfqcwoafu.html

SELECT COUNT(*) FROM users;
来源：http://hz.tianlin.xyz/gthhuqhkez.html

[Q27] 条件计数
来源：http://hz.aizwys.cn/gtfcqoftxm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.wangshuangyany.cn/gtrqhhtmju.html

[Q28] 求和与平均
来源：http://hz.zhiwuduotai.top/gtigcfobuj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gotoacloud.top/gtmqtzplei.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtdlydksxl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zycfv.cn/gtndnosfue.html

[Q30] 分组统计
来源：http://hz.yj202588.top/gtmrqsuwvn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtvogyumjv.html

[Q31] 分组后过滤
来源：http://hz.aibaodan.cn/gtacdsucpi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhixingplan.top/gtjooqtemw.html

[Q32] 分组拼接字符串
来源：http://hz.tian-w.cn/gtexqvtjvw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtkadalvmh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258.top/gtxozhmndy.html

[Q33] 多列分组
来源：http://hz.chenlongwang.top/gtbjvzxcgk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ivvv.top/gtaaihwowc.html

[Q34] 每组取第一条
来源：http://hz.jlsjyb.cn/gtpkjjjwkb.html

SELECT * FROM (
来源：http://hz.fzhhl.top/gtipdiorjz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fengsongda.top/gttsqdkqpk.html

) t WHERE rn = 1;
来源：http://hz.smart0.xyz/gttdkieumq.html

[Q35] 内连接
来源：http://hz.yvedp.cn/gttigztdxt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhoulong.xyz/gtruncfgnr.html

[Q36] 左连接
来源：http://hz.jiagoushi.top/gtfsyhshlu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtyyaijeqh.html

[Q37] 右连接
来源：http://hz.tian-w.cn/gtlaehpwly.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shangyingyoupin.top/gtfdnvpjma.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.aibaodan.cn/gtiptrikyc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigfzy.top/gtattiyfeg.html

[Q39] 自连接（查上下级）
来源：http://hz.zhengqikj.top/gtbnzremhr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yueranfly.top/gtkydndhzd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.316326.xyz/gtyydyyfaw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xingfuxueyuan.xyz/gtrdhnepym.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ehwqpu.com/gtxkwzzrsu.html

[Q41] 多表连接
来源：http://hz.fzhhl.top/gthdguqawk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtlxaeqxmh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnxiangtu.top/gtpmojhwgp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinghuilouyu.cn/gtzqxrshsv.html

[Q42] 连接条件附加过滤
来源：http://hz.sxryk.cn/gtcruzxwvp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sufxvd.cn/gthmsihhnd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhoulong.xyz/gtdhdpsjrc.html

[Q43] 标量子查询
来源：http://hz.smart0.xyz/gtekirafvu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gthszvygth.html

[Q44] IN 子查询
来源：http://hz.ydjk.org.cn/gttpcixody.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.tian-w.cn/gtbxwjdqbf.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigfzy.top/gtjdusmfwv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtrpiiopbc.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.dianchejie.cn/gtdygchxbj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gtvguzgdpx.html

[Q47] 与平均值比较
来源：http://hz.hammf.cn/gtdxnolurq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dianchejie.cn/gtmedrkush.html

[Q48] CTE 公用表表达式
来源：http://hz.jiagoushi.top/gtnycfhncf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydjk.org.cn/gtlhodfvhv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yvedp.cn/gtetpscrya.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtnrfcbrte.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cqqwz.cn/gtyplhqoos.html

[Q50] 批量更新
来源：http://hz.wangdashe.top/gtolngfpmy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtpbrqqwaf.html

[Q51] 用子查询更新
来源：http://hz.jianghu66.top/gtmohcsogr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aibaodan.cn/gtmrbeyeyq.html

[Q52] 删除指定行
来源：http://hz.chenlongwang.top/gtzczaztbt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jiagoushi.top/gtminsmulc.html

[Q53] 按条件删除
来源：http://hz.mhx1999.top/gtmtgrcdnz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guowangkeji.top/gtajmutpfw.html

[Q54] 清空表
来源：http://hz.jyoumei.cn/gtgqpzcgor.html

TRUNCATE TABLE logs;
来源：http://hz.jinghuilouyu.cn/gtgqjatctw.html

[Q55] 排名（并列占位）
来源：http://hz.zhongyouzk.top/gtvpcpzasv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gtsppbtktf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yongpay.top/gtsupcgppl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sxryk.cn/gtzlaaggaj.html

[Q57] 行号
来源：http://hz.zhongyouzk.top/gtvlkktbod.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cheryme.top/gtftizhjql.html

[Q58] 累计求和
来源：http://hz.iojbl.cn/gtvinyykoq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xinyue.icu/gtaopdqzze.html

[Q59] 分组内累计
来源：http://hz.gaohongyu789.top/gtrjpwcfzl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtfqdowmdo.html

[Q60] 取上一行 / 下一行
来源：http://hz.sysykeji.top/gtwtpovoco.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ivvv.top/gtvjsnxxhf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.9152youxi.cn/gtpzsrhxuh.html

[Q61] 移动平均
来源：http://hz.jiagoushi.top/gtfrfndixg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgfzy.top/gtivtyqnqb.html

[Q62] 分组占比
来源：http://hz.feifeiyinyue.top/gtgeouqozm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtzzgaadiw.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtkvikncfj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtkiqyzklz.html

[Q64] 提交事务
来源：http://hz.cashguo.top/gtmafcrxvd.html

COMMIT;
来源：http://hz.redwolf501.top/gtkzsrtdan.html

[Q65] 回滚事务
来源：http://hz.smart0.xyz/gtvyvtlqno.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtygyrpvye.html

[Q66] 行锁查询
来源：http://hz.chenjidiqi.icu/gtqdxuvefa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj20258888.top/gtqlwctlga.html

[Q67] 设置隔离级别
来源：http://hz.zhengqikj.top/gtuuhgnqlw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.kuanghao11.cn/gteaneqcau.html

[Q68] 保存点
来源：http://hz.xuetiantiany.cn/gtwgshpfdb.html

SAVEPOINT sp1;
来源：http://hz.dianchejie.cn/gtkrohyrpp.html

ROLLBACK TO sp1;
来源：http://hz.ehwqpu.com/gtrmwslcky.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtpfmqzcfh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtxnlmtnec.html

[Q70] 更新统计信息
来源：http://hz.xuetiantiany.cn/gtrsjqfyaj.html

ANALYZE TABLE users;
来源：http://hz.316326.xyz/gtaxnxhode.html

[Q71] 查看建表语句
来源：http://hz.jqgfzy.top/gtkngbakwg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pengpengdd.cyou/gtbwsemccg.html

[Q72] 查看索引
来源：http://hz.aibaodan.cn/gtcgbumekn.html

SHOW INDEX FROM users;
来源：http://hz.pengpengdd.cyou/gtdpmabqbg.html

[Q73] 查看表状态
来源：http://hz.kuanghao11.cn/gtzxfmwznj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guannengcc.top/gtkrwxljfg.html

[Q74] 强制使用索引
来源：http://hz.mhx1999.top/gtvrlludhx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtwdcskyst.html

[Q75] 日期格式化
来源：http://hz.ydjk.org.cn/gtnbwubtqi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yvedp.cn/gtncrdvnkd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.quarkkingdee.top/gtczstetzy.html

[Q76] 按天统计
来源：http://hz.quarkkingdee.top/gtzmosvabo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.redwolf501.top/gtmxgykqxp.html

[Q77] 时间加减
来源：http://hz.svipenyu.cn/gttfblkciy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ivvv.top/gtfysiyuid.html

[Q78] 当前时间
来源：http://hz.0kj1m.cn/gtdjcjgsai.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.havefunace.top/gtkynxhqhj.html

[Q79] 字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtiiyldbxq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gtrzcgkowa.html

[Q80] 字符串截取
来源：http://hz.vqdsnc.cn/gtjxbdqyff.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sysykeji.top/gtxvkxezsm.html

[Q81] 字符串替换
来源：http://hz.guowangkeji.top/gtamgvjoeu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.kuanghao11.cn/gtvtkerxli.html

[Q82] 字符长度与字节长度
来源：http://hz.chenlongwang.top/gtvhgusrvx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtpiryamzp.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gtnawhiylf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtxztknqwt.html

[Q84] 去除首尾空格
来源：http://hz.mhx1999.top/gtxcblsnri.html

SELECT TRIM(name) FROM users;
来源：http://hz.guowangkeji.top/gtbzgeavwl.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtxetneeuc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhixingplan.top/gtnrdojcjf.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtoevhhexv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.vqdsnc.cn/gtlrtcsxma.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangkeji.top/gtcdlqhcda.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.smart0.xyz/gtfqkiiqsv.html


<!-- 参考信息 -->