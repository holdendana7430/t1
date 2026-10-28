代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ywan-chungtsiang.top/gthirczhcw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenjidiqi.icu/gtmcwfsxwy.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gthbcnnoie.html

[O05] 并发执行并等待全部完成
来源：http://hz.yueranfly.top/gtvuprksmj.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xuetiantiany.cn/gtmjikgpsx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhiwuduotai.top/gtfqufpxmd.html

JS:   await Promise.all(tasks)
来源：http://hz.zycfv.cn/gtnmvuwacg.html

TS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtmvrlqdhj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenjidiqi.icu/gtblehrmgq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zycfv.cn/gttubjbvdr.html

Ruby: threads.map(&:join)
来源：http://hz.c1oappe.top/gtwjzumigz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangshuangyany.cn/gtrthpwvfg.html

[O06] 使用进程池
来源：http://hz.xingfuxueyuan.xyz/gtrjfjelin.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gotoacloud.top/gtleqpnvxl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.snrcjt.cn/gtqlytybnc.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtangsyqnx.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtcinstrql.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jinqigfzy.top/gtzvcwnofq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtntkmnjxb.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtrelucuur.html

C#:   Parallel.For
来源：http://hz.zhiwuduotai.top/gtfkhdwoyz.html

================================================================================
来源：http://hz.tanke756.top/gtbmreyewm.html

P. 常用工具函数
来源：http://hz.cdnleiting.top/gtzxzfegzv.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxpmpfawo.html

[P01] 生成 UUID
来源：http://hz.yj20258888.top/gthpfshmrg.html

Py:   str(uuid.uuid4())
来源：http://hz.yj202588.top/gtxhdymisq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gogol.net.cn/gtppkumfcu.html

JS:   crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtfcwxcjdv.html

TS:   crypto.randomUUID()
来源：http://hz.zdqjudy.top/gtuhbsyogm.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gtslqkhvtq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.daxiang520.top/gtnyqexlrx.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtcaaabost.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zdqjudy.top/gtxxcbiuei.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhixingplan.top/gtgsfyvltu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hywenlv.cn/gtvawlqmpm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cashguo.top/gtgbztkqha.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.aibaodan.cn/gtfutkpzay.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jiagoushi.top/gtalmmmecp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtgtzkyrlz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhongyouzk.top/gtauiashiw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinqigufen.top/gtayjgpved.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tian-w.cn/gtzhbfqgte.html

[P03] 生成短随机字符串
来源：http://hz.ywan-chungtsiang.top/gtcvqzslfy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.52xcode.cn/gtbszrayrc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.316326.xyz/gtzdeevmxr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.havefunace.top/gtzkzhttvi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.kuanghao11.cn/gtqjtckhvh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinyuanbaomall.cn/gtjsstykrt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.9152youxi.cn/gtclluzyhb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zdqjudy.top/gtsfocgjqy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nanxinkj.top/gtkatbbcqa.html

[P04] 求长度
来源：http://hz.birdmap.top/gtoctsqeej.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tianlin.xyz/gtfvzapccq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtcpbyltee.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sufxvd.cn/gtjdtltcwj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtftcqvwge.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gtmcerzsty.html

Go:   len(arr);  len(m)
来源：http://hz.zhengqikj.top/gtjhrfnuch.html

Ruby: x.length;  x.size
来源：http://hz.gaohongyu789.top/gtebzkcjzu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.jinyuanbaomall.cn/gtsxtmxbtr.html

[P05] 判断两个对象内容是否相等
来源：http://hz.meibo888.top/gtkvugfdth.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shuidangran.top/gtepgijmab.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.svipenyu.cn/gtnklgddrf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.pengpengdd.cyou/gtgweajzus.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gtppmgukpp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenzaomai.com/gtomlhjazy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xylfe.cn/gtsqpuqkii.html

Ruby: a == b
来源：http://hz.daria6918.cn/gtywboenwl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.guannengcc.top/gtnzkcdhbv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jlsjyb.cn/gtfrzmoorp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenlongwang.top/gtrwaarxik.html

PHP:  if (empty($x)) {}
来源：http://hz.hnqzz.top/gtgoitftsq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hfpthk.cn/gtwfcvhevw.html

TS:   if (x == null) {}
来源：http://hz.jqgfzy.top/gtdlkekell.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtglzxivzl.html

Go:   if x == nil {}
来源：http://hz.birdmap.top/gtaeuyfkoy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.zhiwuduotai.top/gtzqecipsm.html

C#:   if (x is null) {}
来源：http://hz.shuidangran.top/gtmhyqldct.html

[P07] 防抖与节流
来源：http://hz.andypj.xyz/gteuqheraz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinghuilouyu.cn/gtdknqadtj.html

PHP:  // 手写时间戳比较
来源：http://hz.cdnleiting.top/gtzhtqchqp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jlsjyb.cn/gtigugclqn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cqqwz.cn/gtpzzyflnk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yvedp.cn/gtmroidmoi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtteddhjjn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yongpay.top/gtkhlyxuqa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shuidangran.top/gtzzhmthia.html

[P08] 处理浮点精度问题
来源：http://hz.cheryme.top/gtdixblbtg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.sysykeji.top/gtobdbfsjl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.redwolf501.top/gtxrbnkqrn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.meibo888.top/gtwwfvszys.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jinqigfzy.top/gtzthtuicz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.andypj.xyz/gtpbadmbny.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hnxiangtu.top/gtlolifnvq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.dianchejie.cn/gtmicghfwz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.316326.xyz/gtqzeqrcou.html

================================================================================
来源：http://hz.bjfxy.top/gtotbeinkg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jlsjyb.cn/gtbobqtlup.html

================================================================================
来源：http://hz.yj20258888.top/gtmgalzofe.html

[Q01] 创建表
来源：http://hz.zhoulong.xyz/gtftaeqetg.html

CREATE TABLE users (
来源：http://hz.snrcjt.cn/gtybvlyjdx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtaogqdcpq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.ppjwa.cn/gtwgaypqza.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gzhubu.top/gtvazzxqdk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.bjfxy.top/gtzqvazaig.html

);
来源：http://hz.xziqi.cn/gtjaaysxrv.html

[Q02] 创建带外键的表
来源：http://hz.shuidangran.top/gtimbcckuw.html

CREATE TABLE orders (
来源：http://hz.chenzaomai.com/gttwgtxxst.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.aizwys.cn/gttmfwriwk.html

user_id INT NOT NULL,
来源：http://hz.pycfn.com/gtfwulcovw.html

amount DECIMAL(10, 2),
来源：http://hz.sysykeji.top/gtqnxohwfc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jqgfzy.top/gthumdzywm.html

);
来源：http://hz.yongpay.top/gtwdqbuika.html

[Q03] 增加列
来源：http://hz.xuanzx.com/gtujytlqrg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gzhubu.top/gteappyujl.html

[Q04] 修改列类型
来源：http://hz.zhoulong.xyz/gtczmexfsx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xziqi.cn/gtyzmwxwnz.html

[Q05] 重命名列
来源：http://hz.havefunace.top/gtnjvnblmy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.chenzaomai.com/gtrovuztsy.html

[Q06] 删除列
来源：http://hz.guowangkeji.top/gtagenzchp.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ppjwa.cn/gtoyuwlrad.html

[Q07] 删除表
来源：http://hz.havefunace.top/gtrrnvmtht.html

DROP TABLE IF EXISTS orders;
来源：http://hz.bjfxy.top/gtyvhcwvnh.html

[Q08] 创建普通索引
来源：http://hz.tian-w.cn/gtguexalrn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.bjfxy.top/gtzjarpbac.html

[Q09] 创建唯一索引
来源：http://hz.yongpay.top/gtxchvowas.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zycfv.cn/gtxewsqkje.html

[Q10] 插入单行
来源：http://hz.nanxinkj.top/gtjqmktjys.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.guannengcc.top/gtqalhjcci.html

[Q11] 一次插入多行
来源：http://hz.ydjk.org.cn/gtbxhsnkkz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj202588.top/gtqfypxyfa.html

[Q12] 插入后取自增 ID
来源：http://hz.birdmap.top/gtrgzonyzo.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gzhubu.top/gtvsvinflc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gzhubu.top/gtefbzhptl.html

[Q13] 忽略重复插入
来源：http://hz.yj20258888.top/gtkkrtrxue.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgfzy.top/gtlyagsvrg.html

[Q14] 存在则更新（upsert）
来源：http://hz.gzhubu.top/gtzsmjrnun.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yj202588.top/gtifwfjzjp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yanxiufei.cn/gtezzhqwgw.html

[Q15] 查询全部
来源：http://hz.yvedp.cn/gtkyddpxku.html

SELECT * FROM users;
来源：http://hz.cqqwz.cn/gtynvrqknb.html

[Q16] 查询指定列
来源：http://hz.daxiang520.top/gtqywwvzrd.html

SELECT id, name FROM users;
来源：http://hz.havefunace.top/gtphtaldwq.html

[Q17] 条件查询
来源：http://hz.havefunace.top/gtnydmdhid.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtjavvyltj.html

[Q18] 模糊匹配
来源：http://hz.yvedp.cn/gtiuayxokd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jlsjyb.cn/gtmumnzkbk.html

[Q19] 范围查询
来源：http://hz.guowangkeji.top/gtijtxitqw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtsfoqetjw.html

[Q20] IN 列表
来源：http://hz.mhx1999.top/gturvvnjmy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenzaomai.com/gteobrtiri.html

[Q21] 空值判断
来源：http://hz.haohaochexian.top/gtdifvlbpx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.redwolf501.top/gtiprbcakz.html

[Q22] 排序
来源：http://hz.ivvv.top/gtinppzdiz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xingfuxueyuan.xyz/gtotngpejd.html

[Q23] 分页
来源：http://hz.yvedp.cn/gtsyczfciq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gogol.net.cn/gtiekgndox.html

[Q24] 去重
来源：http://hz.xingfuxueyuan.xyz/gtacckxexm.html

SELECT DISTINCT city FROM users;
来源：http://hz.pengpengdd.cyou/gtcstyvjwt.html

[Q25] 只取前 N 条
来源：http://hz.ivvv.top/gtjmzgzgrb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xinyue.icu/gtxuvbnfaj.html

[Q26] 计数
来源：http://hz.jianghu66.top/gtexfwsird.html

SELECT COUNT(*) FROM users;
来源：http://hz.cheryme.top/gtfemjauwm.html

[Q27] 条件计数
来源：http://hz.jinyuanbaomall.cn/gtotphxlqv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ehwqpu.com/gtpxzkqmjz.html

[Q28] 求和与平均
来源：http://hz.guannengcc.top/gtuxvflnzv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yangfankeji.com/gteohwfeyw.html

[Q29] 最大最小值
来源：http://hz.yuanzhike.top/gtowmafnbn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cdnleiting.top/gthcfmdejs.html

[Q30] 分组统计
来源：http://hz.aibaodan.cn/gtijdisfrj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtjejylpot.html

[Q31] 分组后过滤
来源：http://hz.haohaochexian.top/gtrzlvztbh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gogol.net.cn/gtilqpqegu.html

[Q32] 分组拼接字符串
来源：http://hz.cqqwz.cn/gtnigsrhzq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.c1oappe.top/gtbbmyljnf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinghuilouyu.cn/gtqcydrdeu.html

[Q33] 多列分组
来源：http://hz.wangshuangyany.cn/gtoycdwdmk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnxiangtu.top/gtxtodottp.html

[Q34] 每组取第一条
来源：http://hz.cheryme.top/gtkhdbjioo.html

SELECT * FROM (
来源：http://hz.jinqigufen.top/gtrjcfprre.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.svipenyu.cn/gtsoqwduii.html

) t WHERE rn = 1;
来源：http://hz.birdmap.top/gttovzwrua.html

[Q35] 内连接
来源：http://hz.hnxiangtu.top/gtqihlckof.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.nwbrower.top/gtscgogukd.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gtvyxyipzf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtjpexeeoa.html

[Q37] 右连接
来源：http://hz.jinqigfzy.top/gtxnyxdkni.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.snrcjt.cn/gtqnedwkti.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangshuangyany.cn/gtghlcgfns.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtcjlkeimk.html

[Q39] 自连接（查上下级）
来源：http://hz.hnxiangtu.top/gtgvckqgzw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ybcxt.top/gtvmicqvny.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.meibo888.top/gtbysdywaa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.pengpengdd.cyou/gtvhajibcv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shangyingyoupin.top/gtywufwtnd.html

[Q41] 多表连接
来源：http://hz.wangshuangyany.cn/gtovxovsau.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yj20258.top/gteznjwank.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yonumen.top/gtvuwbeenp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hysaishi.cn/gtpkkpgzfn.html

[Q42] 连接条件附加过滤
来源：http://hz.jlsjyb.cn/gtiiwhnvxn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.pengpengdd.cyou/gtoyhdrjfk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yvedp.cn/gtapnhnyaf.html

[Q43] 标量子查询
来源：http://hz.zhijiandao.cn/gtwjxrztxa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sysykeji.top/gtckkrswzv.html

[Q44] IN 子查询
来源：http://hz.cqqwz.cn/gtdunkjegk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cheryme.top/gtkllcjisd.html

[Q45] EXISTS 判断存在
来源：http://hz.hnxiangtu.top/gtvxhtakfg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtcfhtuwsz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aizwys.cn/gtewqgwoft.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtgebzenmb.html

[Q47] 与平均值比较
来源：http://hz.ppjwa.cn/gtcdczithf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnxiangtu.top/gtpqltwnug.html

[Q48] CTE 公用表表达式
来源：http://hz.guowangkeji.top/gtrdiwfkas.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.mhx1999.top/gtfrfniukk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fzhhl.top/gtwyvxkfid.html

[Q49] 更新单行
来源：http://hz.xuetiantiany.cn/gtwojjnvvl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hfpthk.cn/gtuppikgus.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtiiylyoel.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jqgufenzy.top/gtzgrffhxo.html

[Q51] 用子查询更新
来源：http://hz.xuetiantiany.cn/gtnpmfsrvc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenjidiqi.icu/gtpmhyufrz.html

[Q52] 删除指定行
来源：http://hz.ydzc1.top/gtlbijffid.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangdashe.top/gtutqptecu.html

[Q53] 按条件删除
来源：http://hz.xuanzx.com/gtoldwbpvk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.meibo888.top/gteoymqnrq.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gtgngowonu.html

TRUNCATE TABLE logs;
来源：http://hz.nanxuanxn.top/gtznmgqsrj.html

[Q55] 排名（并列占位）
来源：http://hz.zycfv.cn/gtcfjlpypn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ybcxt.top/gtxylizwzl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zycfv.cn/gtgeszpmsw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.kuanghao11.cn/gtmjpeonpb.html

[Q57] 行号
来源：http://hz.aibaodan.cn/gtjwvuxxqj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydzc1.top/gtujfeoicj.html

[Q58] 累计求和
来源：http://hz.shuidangran.top/gtuvopeafs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jyoumei.cn/gtrntcjiit.html

[Q59] 分组内累计
来源：http://hz.snrcjt.cn/gttewwsykx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.gaohongyu789.top/gtjsiuvzvv.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinqigufen.top/gtluydzhto.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shangyingyoupin.top/gtjedqfkms.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jinghuilouyu.cn/gtbzaymvfb.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtwknjeaaw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gttbecmhil.html

[Q62] 分组占比
来源：http://hz.zhoulong.xyz/gtcgddfcxe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.feifeiyinyue.top/gtzjtwgtfa.html

[Q63] 开启事务
来源：http://hz.dashuyun.cn/gtxyiuyflh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtgqggwlay.html

[Q64] 提交事务
来源：http://hz.zhoulong.xyz/gttbpechgb.html

COMMIT;
来源：http://hz.ybcxt.top/gtnurxgskh.html

[Q65] 回滚事务
来源：http://hz.yvedp.cn/gttldikflq.html

ROLLBACK;
来源：http://hz.zhiwuduotai.top/gtrptgpeyf.html

[Q66] 行锁查询
来源：http://hz.hywenlv.cn/gtfwwlbnju.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sweek.top/gtkdpessgv.html

[Q67] 设置隔离级别
来源：http://hz.jianghu66.top/gtlbecfjrx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.vqdsnc.cn/gtjjkiydje.html

[Q68] 保存点
来源：http://hz.yuxming.cn/gtuesusmbc.html

SAVEPOINT sp1;
来源：http://hz.andypj.xyz/gtuasnxjrr.html

ROLLBACK TO sp1;
来源：http://hz.xingfuxueyuan.xyz/gtsdamgunt.html

[Q69] 查看执行计划
来源：http://hz.kuanghao11.cn/gtiiymudds.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.havefunace.top/gtgupzqyem.html

[Q70] 更新统计信息
来源：http://hz.zhijiandao.cn/gtuhaicfyk.html

ANALYZE TABLE users;
来源：http://hz.zhoulong.xyz/gtarsrbsdo.html

[Q71] 查看建表语句
来源：http://hz.gotoacloud.top/gtzoddyden.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnxiangtu.top/gtvjtwsjzb.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtuvvgqajg.html

SHOW INDEX FROM users;
来源：http://hz.iojbl.cn/gtybrxlouy.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gtfouhvaut.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gtzgeloldw.html

[Q74] 强制使用索引
来源：http://hz.jlsjyb.cn/gtcuuzaunj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gtcnamoswv.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gthhmykciw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gotoacloud.top/gtcsersbdu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.316326.xyz/gtwuckgsiz.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtoryrutzl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yuxming.cn/gtnyyprkzq.html

[Q77] 时间加减
来源：http://hz.hnqzz.top/gtufsjnsfg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ybcxt.top/gtehrqxisp.html

[Q78] 当前时间
来源：http://hz.jianghu66.top/gtyzxyqehx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.bjfxy.top/gtyrcrcmvc.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtbsgxtpwl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cheryme.top/gtjmvwzwae.html

[Q80] 字符串截取
来源：http://hz.zhoulong.xyz/gtkrtanryy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yvedp.cn/gtdbecsrcl.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtozqovwmh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtcvbovlrn.html

[Q82] 字符长度与字节长度
来源：http://hz.yuanzhike.top/gtuzkqgsvy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.vqdsnc.cn/gtgilnbblh.html

[Q83] 大小写转换
来源：http://hz.xuetiantiany.cn/gtdfvuunyp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ehwqpu.com/gtswaolegw.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gtgokryooa.html

SELECT TRIM(name) FROM users;
来源：http://hz.gaohongyu789.top/gtkrlnvvpo.html

[Q85] 数值取整
来源：http://hz.pycfn.com/gtofefebrv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.c1oappe.top/gtpusfaoqh.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtsvrbyxgx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gtgerkpcwk.html

[Q87] JSON 字段做条件
来源：http://hz.gaohongyu789.top/gtalhvjtag.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhongyouzk.top/gtwldjomrq.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenlongwang.top/gtmgqsfakq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pycfn.com/gthydstocq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shzxlz.cn/gtauoawoqp.html

[Q89] 判断表是否存在
来源：http://hz.jinyuanbaomall.cn/gtliccoucc.html


<!-- 参考信息 -->