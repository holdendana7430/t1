代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://hz.smart0.xyz/gtbfsogroy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinqigfzy.top/gtfjuxacdu.html

JS:   await Promise.all(tasks)
来源：http://hz.birdmap.top/gtbbgdrxmx.html

TS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtshjcvsls.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.tianlin.xyz/gtgojqrnfd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.iojbl.cn/gtlydugyef.html

Ruby: threads.map(&:join)
来源：http://hz.andypj.xyz/gtgiobcxts.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.52xcode.cn/gtlpgtyvis.html

[O06] 使用进程池
来源：http://hz.tian-w.cn/gtixrkdsbq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zdqjudy.top/gtirqmgvhw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigufen.top/gttlgykyox.html

JS:   // child_process / cluster 模块
来源：http://hz.pycfn.com/gtpwhjeevt.html

TS:   // child_process / cluster 模块
来源：http://hz.dashuyun.cn/gtqwzfckyw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhoulong.xyz/gtvonvyjff.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinghuilouyu.cn/gtmvcgygnh.html

Ruby: // fork 块
来源：http://hz.yangfankeji.com/gtqkzppbip.html

C#:   Parallel.For
来源：http://hz.daxiang520.top/gtrsecssnj.html

================================================================================
来源：http://hz.guowangkeji.top/gtkieikyzh.html

P. 常用工具函数
来源：http://hz.gaohongyu789.top/gtvrhbsesg.html

================================================================================
来源：http://hz.cdnleiting.top/gtxwahsksb.html

[P01] 生成 UUID
来源：http://hz.fengsongda.top/gtjphlpwmq.html

Py:   str(uuid.uuid4())
来源：http://hz.ydzc1.top/gtjegutkxk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shzxlz.cn/gtegwafgwu.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtgmpcpaeb.html

TS:   crypto.randomUUID()
来源：http://hz.gzhubu.top/gtrybklluc.html

Java: UUID.randomUUID().toString()
来源：http://hz.kuanghao11.cn/gtdzurtxqu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.gogol.net.cn/gttsoqxwuf.html

Ruby: SecureRandom.uuid
来源：http://hz.ywan-chungtsiang.top/gtotejkfdz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jqgufenzy.top/gtvnnepwaa.html

[P02] MD5 / SHA256 摘要
来源：http://hz.guannengcc.top/gtzctqqmvw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.pycfn.com/gtgcjtmjmv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hammf.cn/gtugecuwth.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.dashuyun.cn/gtqttvijbp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.shzxlz.cn/gttapcllgp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.ehwqpu.com/gtnoblmhsw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guowangkeji.top/gtuhnlmxpq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.birdmap.top/gtdrgkixvm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.0kj1m.cn/gtphgdcgpr.html

[P03] 生成短随机字符串
来源：http://hz.jinqigfzy.top/gtuvwvqhji.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xuanzx.com/gtrjynqqlg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhongyouzk.top/gtsrjievwc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.smart0.xyz/gtldbhbelu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hnxiangtu.top/gtnpegfwfq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnxiangtu.top/gtuzjnewtk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.tianlin.xyz/gtmrqahkug.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yongpay.top/gtcnlelawc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.tianlin.xyz/gttgvdyvvy.html

[P04] 求长度
来源：http://hz.guannengcc.top/gtydfshvzw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.sweek.top/gtdszeqcdl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtsmuyened.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daxiang520.top/gtfyiqayzc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtgsecmwyg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.daxiang520.top/gtalvdnhsc.html

Go:   len(arr);  len(m)
来源：http://hz.havefunace.top/gtotxgmutv.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangkeji.top/gtvdhumgyx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.birdmap.top/gtcwmvhznd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.wangdashe.top/gtprobddzc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtdzzisngn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.9152youxi.cn/gtmrpxnpaw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jinghuilouyu.cn/gtxgmkzbdi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yuxming.cn/gtlbyeikwu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.gotoacloud.top/gtlucnixdf.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.snrcjt.cn/gtzsqwuqgq.html

Ruby: a == b
来源：http://hz.jianghu66.top/gthaohrtjm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yuanzhike.top/gtbuoectiu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sweek.top/gtelknplyp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guowangkeji.top/gtnwolxgxm.html

PHP:  if (empty($x)) {}
来源：http://hz.sxryk.cn/gtfuupwpbz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aizwys.cn/gtwbowpvhn.html

TS:   if (x == null) {}
来源：http://hz.nwbrower.top/gtnihhbwsc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ydzc1.top/gtcyhrtpqb.html

Go:   if x == nil {}
来源：http://hz.yj20258888.top/gtnvgdcevu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xingfuxueyuan.xyz/gtgqqxnlxn.html

C#:   if (x is null) {}
来源：http://hz.jyoumei.cn/gtyuezgpff.html

[P07] 防抖与节流
来源：http://hz.hywenlv.cn/gtjdlrmnhm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ppjwa.cn/gtyatdgfui.html

PHP:  // 手写时间戳比较
来源：http://hz.jiagoushi.top/gtleyyakaf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtwmvvesyw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtwlenvdub.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ywan-chungtsiang.top/gtctrozuhi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hfpthk.cn/gtnravjseu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.cucudq.cn/gtfyvxjjxn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.snrcjt.cn/gtulozzkzf.html

[P08] 处理浮点精度问题
来源：http://hz.sysykeji.top/gtostrzjpk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jinqigufen.top/gtohlelwts.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gaohongyu789.top/gtcncmraoy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangdashe.top/gtpteolxec.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.wangdashe.top/gtwxlavyhd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yuanzhike.top/gtuovjonjs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.tianlin.xyz/gtutozenuw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnqzz.top/gtzmuwborr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sxryk.cn/gtngefghrh.html

================================================================================
来源：http://hz.birdmap.top/gtdefzwoli.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangdashe.top/gtrqdwtlqk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtamkjkuya.html

[Q01] 创建表
来源：http://hz.nwbrower.top/gtpsgbtbpa.html

CREATE TABLE users (
来源：http://hz.zhengqikj.top/gthztdmwdr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtbqxbyufg.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gttyzhnkun.html

email VARCHAR(100) UNIQUE,
来源：http://hz.wangdashe.top/gtifdqngkh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sweek.top/gtqstdgjjw.html

);
来源：http://hz.chenjidiqi.icu/gtbbnxmctl.html

[Q02] 创建带外键的表
来源：http://hz.yj20258888.top/gtsznkchmr.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtwjhxfxrr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtfhdtdnvc.html

user_id INT NOT NULL,
来源：http://hz.quarkkingdee.top/gtlorkzqhg.html

amount DECIMAL(10, 2),
来源：http://hz.feifeiyinyue.top/gtxugspodl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.pycfn.com/gtsktvnzhc.html

);
来源：http://hz.316326.xyz/gtmvidbssz.html

[Q03] 增加列
来源：http://hz.yvedp.cn/gtxrrbwuaq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shzxlz.cn/gtqkasghdh.html

[Q04] 修改列类型
来源：http://hz.yangfankeji.com/gtebkelxte.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.sysykeji.top/gtmrqfdnud.html

[Q05] 重命名列
来源：http://hz.fzhhl.top/gtykwyxjlq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gthvgimzla.html

[Q06] 删除列
来源：http://hz.yj202588.top/gtefyjpnbr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.aibaodan.cn/gtxjkygupw.html

[Q07] 删除表
来源：http://hz.zhijiandao.cn/gtrsleaggl.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sufxvd.cn/gtssnxsgba.html

[Q08] 创建普通索引
来源：http://hz.pengpengdd.cyou/gtbqtswjdt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.birdmap.top/gtjonaieuq.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtysbmwmpc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yanxiufei.cn/gteklvgpdm.html

[Q10] 插入单行
来源：http://hz.smart0.xyz/gtkkgssxnd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.316326.xyz/gtrhcdxqun.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtkorejghj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.xuetiantiany.cn/gtwvahgoba.html

[Q12] 插入后取自增 ID
来源：http://hz.smart0.xyz/gtnrxuqdnb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhijiandao.cn/gtywzhgzhq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuanzx.com/gtggkqrckv.html

[Q13] 忽略重复插入
来源：http://hz.cdnleiting.top/gtyoufiuoz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigfzy.top/gtuchjbyrp.html

[Q14] 存在则更新（upsert）
来源：http://hz.xinyue.icu/gtnzecvjcq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtngmgerwg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtzrdfoggz.html

[Q15] 查询全部
来源：http://hz.cdnleiting.top/gtsgolyzeo.html

SELECT * FROM users;
来源：http://hz.9152youxi.cn/gtnrekpruu.html

[Q16] 查询指定列
来源：http://hz.shuidangran.top/gtupsyaymw.html

SELECT id, name FROM users;
来源：http://hz.yuxming.cn/gtvohglykj.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtokqyfrqe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jqgufenzy.top/gtxwvlmkxd.html

[Q18] 模糊匹配
来源：http://hz.hfpthk.cn/gtnmrmuklo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.chenzaomai.com/gtekdvlkas.html

[Q19] 范围查询
来源：http://hz.yanxiufei.cn/gtzwxjqqco.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj202588.top/gtghqfjwra.html

[Q20] IN 列表
来源：http://hz.gzhubu.top/gtkjrukmpz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zdqjudy.top/gtnbblgwdu.html

[Q21] 空值判断
来源：http://hz.yueranfly.top/gtafatgjvh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hongshengwenyu.top/gtefnhnlmo.html

[Q22] 排序
来源：http://hz.nanxinkj.top/gtccyawouk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangtech.top/gtuxduwaxa.html

[Q23] 分页
来源：http://hz.guowangkeji.top/gtcqmkvkxc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhoulong.xyz/gtivcrydcs.html

[Q24] 去重
来源：http://hz.smart0.xyz/gtzadkqmdv.html

SELECT DISTINCT city FROM users;
来源：http://hz.hfpthk.cn/gtzavgdwwe.html

[Q25] 只取前 N 条
来源：http://hz.hongshengwenyu.top/gtaxtqymzn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.wangdashe.top/gtummhsmox.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtajhbmabv.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj202588.top/gtvhbvblmh.html

[Q27] 条件计数
来源：http://hz.pengpengdd.cyou/gtiwaoylkm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hfpthk.cn/gtiulijozo.html

[Q28] 求和与平均
来源：http://hz.hnxiangtu.top/gtqjxbvqpr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.cheryme.top/gtcjupirlt.html

[Q29] 最大最小值
来源：http://hz.feifeiyinyue.top/gtiwxkgcyg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.tianlin.xyz/gtxuwxuuql.html

[Q30] 分组统计
来源：http://hz.zhengqikj.top/gtgmlbwgeo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtupxbbqdc.html

[Q31] 分组后过滤
来源：http://hz.jianghu66.top/gtdhalgkwk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gzhubu.top/gtyrhqajyq.html

[Q32] 分组拼接字符串
来源：http://hz.snrcjt.cn/gtwtpskdwv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sysykeji.top/gtnucbhaqy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zhongyouzk.top/gtuzdrsoqg.html

[Q33] 多列分组
来源：http://hz.hnqzz.top/gtufbxsyld.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sweek.top/gttyaeoatt.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtwzpdrtgd.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtexzohsey.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cheryme.top/gtornqdojd.html

) t WHERE rn = 1;
来源：http://hz.meibo888.top/gtvpjjoorx.html

[Q35] 内连接
来源：http://hz.svipenyu.cn/gtnemiwhne.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.aibaodan.cn/gtklnpeiom.html

[Q36] 左连接
来源：http://hz.hysaishi.cn/gtqogjssih.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.mhx1999.top/gtwzmzljjh.html

[Q37] 右连接
来源：http://hz.shuidangran.top/gtagnoxkmb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.havefunace.top/gtdjjldjwr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zycfv.cn/gteptdooxe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yonumen.top/gtwioaxbzs.html

[Q39] 自连接（查上下级）
来源：http://hz.jinghuilouyu.cn/gtgklgcryz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gtjvuibodm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.feifeiyinyue.top/gteiaorgby.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydzc1.top/gthjtrljeb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhijiandao.cn/gtrybwptza.html

[Q41] 多表连接
来源：http://hz.cashguo.top/gteyfathgi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuanzhike.top/gtaqecumsy.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shanyushiyangtech.top/gtwgkxkfpt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.redwolf501.top/gtzxrynddj.html

[Q42] 连接条件附加过滤
来源：http://hz.pengpengdd.cyou/gtudxznstx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhongyouzk.top/gtcpplapbk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daria6918.cn/gtbuvfdkrd.html

[Q43] 标量子查询
来源：http://hz.yonumen.top/gtvxquiwhs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tian-w.cn/gtwlkhrtcb.html

[Q44] IN 子查询
来源：http://hz.guowangkeji.top/gtfwhdbgjc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj20258888.top/gtylzqnkdl.html

[Q45] EXISTS 判断存在
来源：http://hz.cucudq.cn/gtqqdrckzj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtwujbltuj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.hammf.cn/gtgypkhyca.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tanke756.top/gtkhvwaygr.html

[Q47] 与平均值比较
来源：http://hz.hongshengwenyu.top/gtsztxdtoo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aibaodan.cn/gtdzjseuri.html

[Q48] CTE 公用表表达式
来源：http://hz.ppjwa.cn/gtgudrpppe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.0kj1m.cn/gtbroecybj.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.bjfxy.top/gtnwixxeav.html

[Q49] 更新单行
来源：http://hz.aibaodan.cn/gtowxtccon.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.redwolf501.top/gtcqksocje.html

[Q50] 批量更新
来源：http://hz.gotoacloud.top/gtsaklvheb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cqqwz.cn/gtssroiagx.html

[Q51] 用子查询更新
来源：http://hz.wangshuangyany.cn/gtalfcivuj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gogol.net.cn/gtgnpgnlbt.html

[Q52] 删除指定行
来源：http://hz.zhixingplan.top/gtbyzawrok.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtrkzlsnsn.html

[Q53] 按条件删除
来源：http://hz.snrcjt.cn/gttumothwu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yanxiufei.cn/gthfklxnnw.html

[Q54] 清空表
来源：http://hz.jinghuilouyu.cn/gtttmfulde.html

TRUNCATE TABLE logs;
来源：http://hz.hysaishi.cn/gttnstbhti.html

[Q55] 排名（并列占位）
来源：http://hz.wangdashe.top/gtptbfubsi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ydzc1.top/gtawynrlkl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guannengcc.top/gtcqjhuoxx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtjrrnqivr.html

[Q57] 行号
来源：http://hz.xziqi.cn/gtksnnogvs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.0kj1m.cn/gtsjfntkkm.html

[Q58] 累计求和
来源：http://hz.meibo888.top/gtipxwqayu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cashguo.top/gtkttvtbeh.html

[Q59] 分组内累计
来源：http://hz.yj202588.top/gtggygezdq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yuanzhike.top/gtocbvvpqe.html

[Q60] 取上一行 / 下一行
来源：http://hz.ivvv.top/gtxkkwhvfd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.iojbl.cn/gtdcmanrby.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aibaodan.cn/gtvcoiwdkt.html

[Q61] 移动平均
来源：http://hz.52xcode.cn/gtyhhssnik.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.guannengcc.top/gtlsbsydnf.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtjzfmecew.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtdvikwape.html

[Q63] 开启事务
来源：http://hz.chenzaomai.com/gtrydunrex.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cdnleiting.top/gtagenlwyh.html

[Q64] 提交事务
来源：http://hz.0kj1m.cn/gtodxhjdqy.html

COMMIT;
来源：http://hz.chenzaomai.com/gtadrusfdf.html

[Q65] 回滚事务
来源：http://hz.jyoumei.cn/gtndadytgt.html

ROLLBACK;
来源：http://hz.dashuyun.cn/gttkqouelq.html

[Q66] 行锁查询
来源：http://hz.snrcjt.cn/gtwcxetulz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gtuypfehhu.html

[Q67] 设置隔离级别
来源：http://hz.shzxlz.cn/gtlrckgnvh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.c1oappe.top/gtcpbpfvxb.html

[Q68] 保存点
来源：http://hz.jinghuilouyu.cn/gtbbmouvmp.html

SAVEPOINT sp1;
来源：http://hz.ehwqpu.com/gtttrybesd.html

ROLLBACK TO sp1;
来源：http://hz.shuidangran.top/gtngqdabev.html

[Q69] 查看执行计划
来源：http://hz.chenzaomai.com/gtktgyufps.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zdqjudy.top/gtnrvyvylj.html

[Q70] 更新统计信息
来源：http://hz.nanxinkj.top/gtfojszvoi.html

ANALYZE TABLE users;
来源：http://hz.hongshengwenyu.top/gtcbwruztw.html

[Q71] 查看建表语句
来源：http://hz.birdmap.top/gttxcivpfl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shanyushiyangtech.top/gtmpdeqoem.html

[Q72] 查看索引
来源：http://hz.xylfe.cn/gtkinbosep.html

SHOW INDEX FROM users;
来源：http://hz.daria6918.cn/gtmmgoetzv.html

[Q73] 查看表状态
来源：http://hz.gzhubu.top/gteluozvjc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtfwlwxunc.html

[Q74] 强制使用索引
来源：http://hz.dashuyun.cn/gtqvspvbxv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.guannengcc.top/gtcndxucrq.html

[Q75] 日期格式化
来源：http://hz.ppjwa.cn/gtzrgixdll.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtardnlbqv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhijiandao.cn/gtmdloexlu.html

[Q76] 按天统计
来源：http://hz.wangdashe.top/gttvsbhgny.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gthuyimfre.html

[Q77] 时间加减
来源：http://hz.zhiwuduotai.top/gtewiwigaf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.0kj1m.cn/gtmclevmgo.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtldsmmiay.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuanzx.com/gtzcmefriu.html

[Q79] 字符串拼接
来源：http://hz.smart0.xyz/gttvdaawsx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydzc1.top/gtzmnpzhzv.html

[Q80] 字符串截取
来源：http://hz.svipenyu.cn/gtyhckmmhx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sysykeji.top/gtbwawolbo.html

[Q81] 字符串替换
来源：http://hz.yuanzhike.top/gtefbeknnl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yvedp.cn/gtncetidcq.html

[Q82] 字符长度与字节长度
来源：http://hz.jlsjyb.cn/gtzizybdks.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnxiangtu.top/gtetpbwaxw.html

[Q83] 大小写转换
来源：http://hz.ppjwa.cn/gtjrjnudvh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhengqikj.top/gtppmpzvgs.html

[Q84] 去除首尾空格
来源：http://hz.jqgfzy.top/gtvaamcahp.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtthgaumwk.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gteiynsdwr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guannengcc.top/gtekkcptbr.html

[Q86] 读取 JSON 字段
来源：http://hz.zhongyouzk.top/gthgssjyjh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.meibo888.top/gtkwvuvrar.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtqdinsedz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yj20258888.top/gtvqudupyz.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhaomingkeji.xyz/gtluwaeuop.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.quarkkingdee.top/gtherxayme.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhongyouzk.top/gtlcmgqfvq.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtmglkzcln.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yangfankeji.com/gtlmsqibag.html

[Q90] 生成序号列
来源：http://hz.52xcode.cn/gtrekyqtxv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.0kj1m.cn/gtsfdogvmz.html

================================================================================
来源：http://hz.xziqi.cn/gtdohypmio.html


<!-- 参考信息 -->