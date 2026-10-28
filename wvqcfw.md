代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://hz.yangfankeji.com/gtjiyylirf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.guannengcc.top/gtvpbflumw.html

JS:   await Promise.all(tasks)
来源：http://hz.sweek.top/gtrpyaocyn.html

TS:   await Promise.all(tasks)
来源：http://hz.sxryk.cn/gtsjxfxoff.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhoulong.xyz/gtyvkyfksz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yangfankeji.com/gtiziadxyu.html

Ruby: threads.map(&:join)
来源：http://hz.iojbl.cn/gtsvuotkto.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhongyouzk.top/gtzagnyjml.html

[O06] 使用进程池
来源：http://hz.sxryk.cn/gtvmhdnzax.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jinqigufen.top/gteonpqoro.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cdnleiting.top/gtqtboqnkf.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gtlgkftwkq.html

TS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtrmceonjs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zdqjudy.top/gtllkaeymu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sweek.top/gtpxqgccsj.html

Ruby: // fork 块
来源：http://hz.daxiang520.top/gtxxvkkskm.html

C#:   Parallel.For
来源：http://hz.yj202588.top/gtracrhyfz.html

================================================================================
来源：http://hz.xziqi.cn/gtfvbdrupg.html

P. 常用工具函数
来源：http://hz.jianghu66.top/gtwklmrrln.html

================================================================================
来源：http://hz.chenzaomai.com/gtppgmwdai.html

[P01] 生成 UUID
来源：http://hz.sxryk.cn/gtegigohrr.html

Py:   str(uuid.uuid4())
来源：http://hz.mhx1999.top/gtdsdagfce.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yonumen.top/gtpwzqjkvp.html

JS:   crypto.randomUUID()
来源：http://hz.pycfn.com/gtdnegdawu.html

TS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtxbpvzbne.html

Java: UUID.randomUUID().toString()
来源：http://hz.xuetiantiany.cn/gtuipocgjq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangtech.top/gtahkxmddu.html

Ruby: SecureRandom.uuid
来源：http://hz.jinqigfzy.top/gtylfhkgox.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cheryme.top/gteibrhibf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sxryk.cn/gtuycrmoqt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenjidiqi.icu/gttehpkotk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gthmzyzuhn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gzhubu.top/gtjuvfoiyn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtjetipath.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhaomingkeji.xyz/gtstytpsuo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yongpay.top/gtcgsglphf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.52xcode.cn/gteetweuzn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zycfv.cn/gtnnzlbcul.html

[P03] 生成短随机字符串
来源：http://hz.haohaochexian.top/gtlsnylzsa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtnumdgdoe.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dianchejie.cn/gtckhbsbft.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ehwqpu.com/gtwnpgvugk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.snrcjt.cn/gtfluceuna.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnqzz.top/gtoykfouua.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ppjwa.cn/gtlxrcmcfa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.daria6918.cn/gtymitmskx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.fzhhl.top/gtgbdyiswi.html

[P04] 求长度
来源：http://hz.chenjidiqi.icu/gtziqfodll.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.birdmap.top/gtwjcfcdee.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hywenlv.cn/gtinleefba.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jyoumei.cn/gtrwqijbik.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtqtjdfzzi.html

Java: list.size();  map.size();  s.length()
来源：http://hz.iojbl.cn/gtsodygzmi.html

Go:   len(arr);  len(m)
来源：http://hz.jyoumei.cn/gtlmgbvnsr.html

Ruby: x.length;  x.size
来源：http://hz.zycfv.cn/gtfivbpmrb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.nanxinkj.top/gtimyaehqz.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xziqi.cn/gtnautsfvq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shangyingyoupin.top/gtbsywlubi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.daria6918.cn/gtkbuuacqx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.haohaochexian.top/gtynbelkre.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gtmyrxrinb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.xinyue.icu/gtbplcembv.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.cqqwz.cn/gtcmdwciyy.html

Ruby: a == b
来源：http://hz.hysaishi.cn/gtjpszgkty.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.xingfuxueyuan.xyz/gtdatrmqrm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.gotoacloud.top/gtbwtmkjcl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jiagoushi.top/gttcvagzss.html

PHP:  if (empty($x)) {}
来源：http://hz.hnxiangtu.top/gtbvtfoyme.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guowangkeji.top/gtbdbydxzg.html

TS:   if (x == null) {}
来源：http://hz.svipenyu.cn/gtpichfaor.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.fzhhl.top/gtjgafwduj.html

Go:   if x == nil {}
来源：http://hz.xuanzx.com/gtauviivwt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jinqigufen.top/gtiutyrvet.html

C#:   if (x is null) {}
来源：http://hz.hfpthk.cn/gtraysgzyv.html

[P07] 防抖与节流
来源：http://hz.guannengcc.top/gtzavrojcd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.hammf.cn/gteuyimyap.html

PHP:  // 手写时间戳比较
来源：http://hz.cqqwz.cn/gtvprckulp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xingfuxueyuan.xyz/gtssyaseij.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtizbqmoax.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.pycfn.com/gtzgcgetun.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shzxlz.cn/gtlfbbutfx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.birdmap.top/gttaxnskrt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.fzhhl.top/gtdpkfwlte.html

[P08] 处理浮点精度问题
来源：http://hz.ppjwa.cn/gtawisixnc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zhaomingkeji.xyz/gtgemdcfou.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.shuidangran.top/gtnzugsxdf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.yonumen.top/gtzuhqfdpn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.chenlongwang.top/gtrfjmzqpg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinyuanbaomall.cn/gttvmmvuyj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hywenlv.cn/gtgvsytqzm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shzxlz.cn/gtghlxohjt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.feifeiyinyue.top/gtvgurnjae.html

================================================================================
来源：http://hz.yvedp.cn/gtejqzvkam.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nwbrower.top/gtlbflrgyz.html

================================================================================
来源：http://hz.tian-w.cn/gtovxvngeu.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtobqapvjs.html

CREATE TABLE users (
来源：http://hz.guannengcc.top/gtlxivhxob.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.svipenyu.cn/gtnspwhwxa.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fzhhl.top/gtgngsdeci.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jyoumei.cn/gtzteoeaav.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jqgufenzy.top/gtrwfauxba.html

);
来源：http://hz.aizwys.cn/gtjdunhujk.html

[Q02] 创建带外键的表
来源：http://hz.yongpay.top/gthhezgpjv.html

CREATE TABLE orders (
来源：http://hz.tanke756.top/gtuijyvtph.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yj20258888.top/gtuymlkztj.html

user_id INT NOT NULL,
来源：http://hz.chenjidiqi.icu/gtrldmyooa.html

amount DECIMAL(10, 2),
来源：http://hz.shangyingyoupin.top/gtiejgphch.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zycfv.cn/gtolelikmg.html

);
来源：http://hz.havefunace.top/gtjtbomprd.html

[Q03] 增加列
来源：http://hz.yj202588.top/gtpsscokxe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pengpengdd.cyou/gtgbhatxjo.html

[Q04] 修改列类型
来源：http://hz.tian-w.cn/gtwqsrxshr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.birdmap.top/gtlvonuals.html

[Q05] 重命名列
来源：http://hz.redwolf501.top/gtfuxizrig.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtdzkqynav.html

[Q06] 删除列
来源：http://hz.wangdashe.top/gtvwbeytpe.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jinqigufen.top/gtjazwefhs.html

[Q07] 删除表
来源：http://hz.redwolf501.top/gtjmumuhdk.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xziqi.cn/gtlguadplo.html

[Q08] 创建普通索引
来源：http://hz.bjfxy.top/gtquywfzsa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.nanxuanxn.top/gtljlnfvnh.html

[Q09] 创建唯一索引
来源：http://hz.wangshuangyany.cn/gtcwsujegt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.gotoacloud.top/gtxqkxcuok.html

[Q10] 插入单行
来源：http://hz.gzhubu.top/gtfvsxjlip.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.yueranfly.top/gtwhayrvpj.html

[Q11] 一次插入多行
来源：http://hz.aizwys.cn/gtnxhitmgx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.dashuyun.cn/gtojrclhoy.html

[Q12] 插入后取自增 ID
来源：http://hz.daxiang520.top/gtgdkllltf.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.redwolf501.top/gteacsppqt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtrdrcqpoo.html

[Q13] 忽略重复插入
来源：http://hz.feifeiyinyue.top/gtqnzgwnxu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtgjglezvd.html

[Q14] 存在则更新（upsert）
来源：http://hz.pengpengdd.cyou/gtnutsiypx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hammf.cn/gtyyswpjqc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gotoacloud.top/gttwbkplel.html

[Q15] 查询全部
来源：http://hz.cqqwz.cn/gtsjnlrxxm.html

SELECT * FROM users;
来源：http://hz.zhoulong.xyz/gtznerfndz.html

[Q16] 查询指定列
来源：http://hz.zhaomingkeji.xyz/gthzbtwsag.html

SELECT id, name FROM users;
来源：http://hz.gzhubu.top/gtmkwjihws.html

[Q17] 条件查询
来源：http://hz.tian-w.cn/gtfksfizld.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.redwolf501.top/gtgkkxaznb.html

[Q18] 模糊匹配
来源：http://hz.aibaodan.cn/gtabllercw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jqgfzy.top/gtinsugubk.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gtxlwatqdn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.ivvv.top/gthncvpzie.html

[Q20] IN 列表
来源：http://hz.xziqi.cn/gthvwblpka.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zdqjudy.top/gttffqrsvc.html

[Q21] 空值判断
来源：http://hz.svipenyu.cn/gthfnqqqpj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhixingplan.top/gtlfgthoco.html

[Q22] 排序
来源：http://hz.havefunace.top/gtumxaaflu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tian-w.cn/gtaxruiipi.html

[Q23] 分页
来源：http://hz.nanxuanxn.top/gtumnlqevh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xylfe.cn/gtdlljeagf.html

[Q24] 去重
来源：http://hz.ppjwa.cn/gttzshbqit.html

SELECT DISTINCT city FROM users;
来源：http://hz.birdmap.top/gtifrvasnr.html

[Q25] 只取前 N 条
来源：http://hz.jinghuilouyu.cn/gtukzzjaby.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.haohaochexian.top/gtjurwyxww.html

[Q26] 计数
来源：http://hz.chenjidiqi.icu/gtzhsoletp.html

SELECT COUNT(*) FROM users;
来源：http://hz.yj20258.top/gtzrpcbzng.html

[Q27] 条件计数
来源：http://hz.sweek.top/gtdtanfvds.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenzaomai.com/gthyuztcnm.html

[Q28] 求和与平均
来源：http://hz.chenjidiqi.icu/gtjxrwkpne.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.yuxming.cn/gtegutxbpw.html

[Q29] 最大最小值
来源：http://hz.yonumen.top/gtoozbqaex.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hywenlv.cn/gtuchmdaan.html

[Q30] 分组统计
来源：http://hz.wangshuangyany.cn/gtazltczsy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtpvyntrww.html

[Q31] 分组后过滤
来源：http://hz.chenjidiqi.icu/gtcetroibw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhongyouzk.top/gtiaiycyre.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gtoahmdadx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtbsmexqml.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.andypj.xyz/gtzjrrekht.html

[Q33] 多列分组
来源：http://hz.snrcjt.cn/gtdaaizddu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.andypj.xyz/gtszpgxlrl.html

[Q34] 每组取第一条
来源：http://hz.jqgufenzy.top/gtucwchqhi.html

SELECT * FROM (
来源：http://hz.jinqigfzy.top/gtysgomcan.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.birdmap.top/gtbncfgycu.html

) t WHERE rn = 1;
来源：http://hz.ehwqpu.com/gtkazoruhe.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtdjhkyeej.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.andypj.xyz/gtzygxjcjd.html

[Q36] 左连接
来源：http://hz.xuetiantiany.cn/gtcmyfpdrd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinyuanbaomall.cn/gtsmivijpe.html

[Q37] 右连接
来源：http://hz.zhaomingkeji.xyz/gtykwyuywf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhixingplan.top/gtegmpcxxa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258.top/gtcjpspaik.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtpdpxnhcp.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtapjlvlpl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.dianchejie.cn/gtjcmfujfr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gtyqouitvh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guowangkeji.top/gtglyhopth.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ivvv.top/gtvpdayybz.html

[Q41] 多表连接
来源：http://hz.jqgfzy.top/gtndmrkfit.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhaomingkeji.xyz/gtlvdaqrzj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.birdmap.top/gtzlievllq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ywan-chungtsiang.top/gtqtgpecls.html

[Q42] 连接条件附加过滤
来源：http://hz.vqdsnc.cn/gtqhtdxbsi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yanxiufei.cn/gtzumpzkpt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guowangkeji.top/gtqeotlbsg.html

[Q43] 标量子查询
来源：http://hz.shuidangran.top/gtjvwdyoyq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ybcxt.top/gtifaoclbz.html

[Q44] IN 子查询
来源：http://hz.haohaochexian.top/gtxrriyqju.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtjgppjmwx.html

[Q45] EXISTS 判断存在
来源：http://hz.yuanzhike.top/gtlyhjqnvd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtatchhtbg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gtvspjeibm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtnbsoxswe.html

[Q47] 与平均值比较
来源：http://hz.zhijiandao.cn/gtporttljt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aibaodan.cn/gtmdqlwitn.html

[Q48] CTE 公用表表达式
来源：http://hz.quarkkingdee.top/gtufsfwitt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sxryk.cn/gtlvvymtan.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtemhtoafn.html

[Q49] 更新单行
来源：http://hz.cucudq.cn/gtfurkuifp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtmrxpuziw.html

[Q50] 批量更新
来源：http://hz.pengpengdd.cyou/gtojliolqw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.havefunace.top/gtjmgrbort.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtzrvujaaf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jianghu66.top/gtocktfbei.html

[Q52] 删除指定行
来源：http://hz.fengsongda.top/gtlescentw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jianghu66.top/gtakhxkbqm.html

[Q53] 按条件删除
来源：http://hz.zycfv.cn/gtkqeajbwo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtdgrkdwgz.html

[Q54] 清空表
来源：http://hz.chenlongwang.top/gtezszyary.html

TRUNCATE TABLE logs;
来源：http://hz.xingfuxueyuan.xyz/gtlengllhk.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtvetrpebj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zycfv.cn/gtrosektan.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yueranfly.top/gtzfiovlpi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangshuangyany.cn/gtnczvhhgi.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtbzjkxoug.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.vqdsnc.cn/gtnglibiae.html

[Q58] 累计求和
来源：http://hz.yvedp.cn/gtoclftpkh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jianghu66.top/gtozuowstm.html

[Q59] 分组内累计
来源：http://hz.yangfankeji.com/gtahtdturo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtzpkoqhli.html

[Q60] 取上一行 / 下一行
来源：http://hz.gotoacloud.top/gtqynkshns.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gotoacloud.top/gtywcmcpei.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cqqwz.cn/gtvrptzjsq.html

[Q61] 移动平均
来源：http://hz.hammf.cn/gtmeaflwba.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yanxiufei.cn/gtxxghefoh.html

[Q62] 分组占比
来源：http://hz.cheryme.top/gtvufzcarp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cqqwz.cn/gteksebrhd.html

[Q63] 开启事务
来源：http://hz.daria6918.cn/gtdfaqycdz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gtlixrqose.html

[Q64] 提交事务
来源：http://hz.xingfuxueyuan.xyz/gtmcnzxgvc.html

COMMIT;
来源：http://hz.hnxiangtu.top/gtzcatgtml.html

[Q65] 回滚事务
来源：http://hz.xuanzx.com/gtzraedtcp.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gtejyuiwkh.html

[Q66] 行锁查询
来源：http://hz.pengpengdd.cyou/gtfuubibsk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinghuilouyu.cn/gtrlolnkth.html

[Q67] 设置隔离级别
来源：http://hz.cucudq.cn/gtdagahwin.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.smart0.xyz/gtdwxkqhkx.html

[Q68] 保存点
来源：http://hz.daxiang520.top/gtsnzkxrcd.html

SAVEPOINT sp1;
来源：http://hz.ydzc1.top/gtppckfqej.html

ROLLBACK TO sp1;
来源：http://hz.sysykeji.top/gtcidgqmfz.html

[Q69] 查看执行计划
来源：http://hz.pengpengdd.cyou/gtvratkxhq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pengpengdd.cyou/gtcwhodycx.html

[Q70] 更新统计信息
来源：http://hz.hammf.cn/gtymlbdlbi.html

ANALYZE TABLE users;
来源：http://hz.jinyuanbaomall.cn/gtnxfctbor.html

[Q71] 查看建表语句
来源：http://hz.zhiwuduotai.top/gtfgwhxvjb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhoulong.xyz/gtloywwxzw.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtfzxtpkul.html

SHOW INDEX FROM users;
来源：http://hz.daxiang520.top/gtxolhqeae.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtzfenkcci.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.iojbl.cn/gtcvnlbuli.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gtbvhodwbq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zdqjudy.top/gtxhsktsyj.html

[Q75] 日期格式化
来源：http://hz.dashuyun.cn/gtsmvcnrdr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhoulong.xyz/gtyfwhyyjv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jlsjyb.cn/gtyglhzuwm.html

[Q76] 按天统计
来源：http://hz.snrcjt.cn/gtdbzlpgug.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtdmaeuczy.html

[Q77] 时间加减
来源：http://hz.shanyushiyangkeji.top/gtwjgbquvf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.c1oappe.top/gthdvcuhgz.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gtodwgodhl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtgdchsdrq.html

[Q79] 字符串拼接
来源：http://hz.yueranfly.top/gtvlcymznz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenjidiqi.icu/gtljzqklfm.html

[Q80] 字符串截取
来源：http://hz.haohaochexian.top/gtnjzlgguw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhongyouzk.top/gtjyhlapic.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtjrgfrkxc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtlwhgfwvg.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtugjvwcrg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtyqothgxt.html

[Q83] 大小写转换
来源：http://hz.dashuyun.cn/gtxeouters.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhijiandao.cn/gtohsfnufj.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtmkjtfdev.html

SELECT TRIM(name) FROM users;
来源：http://hz.yonumen.top/gtqcalgiyf.html

[Q85] 数值取整
来源：http://hz.jinqigufen.top/gtmekrwgwu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.smart0.xyz/gtscwkmwzm.html

[Q86] 读取 JSON 字段
来源：http://hz.hywenlv.cn/gttradgojc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhoulong.xyz/gtrbubmlag.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gtyyscmwyr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tianlin.xyz/gtavzwffuu.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gthwrydozc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.wangdashe.top/gtvtmjynud.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sufxvd.cn/gtnhqypurt.html

[Q89] 判断表是否存在
来源：http://hz.mhx1999.top/gtbbhdqgnr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shangyingyoupin.top/gtejhclfrz.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtinfojoqr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.smart0.xyz/gtwmdfghsv.html

================================================================================
来源：http://hz.chenzaomai.com/gtduwryuqe.html


<!-- 参考信息 -->