代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.andypj.xyz/gtnulzrdym.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gtbectiiof.html

Ruby: threads.map(&:join)
来源：http://hz.yvedp.cn/gtkottlxkk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.havefunace.top/gthdrecabq.html

[O06] 使用进程池
来源：http://hz.bjfxy.top/gtsexskxrx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.cdnleiting.top/gtkxjwhmom.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yonumen.top/gtivlzspgr.html

JS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtibxaarux.html

TS:   // child_process / cluster 模块
来源：http://hz.chenjidiqi.icu/gtlcqsjcwh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhixingplan.top/gtjfcczpfq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cashguo.top/gtataaazbj.html

Ruby: // fork 块
来源：http://hz.0kj1m.cn/gtgwyuhuzz.html

C#:   Parallel.For
来源：http://hz.pengpengdd.cyou/gteyhwjvzn.html

================================================================================
来源：http://hz.smart0.xyz/gtguykahxw.html

P. 常用工具函数
来源：http://hz.quarkkingdee.top/gtssywtfze.html

================================================================================
来源：http://hz.gzhubu.top/gtlqxdwwoq.html

[P01] 生成 UUID
来源：http://hz.birdmap.top/gtklnzlqhu.html

Py:   str(uuid.uuid4())
来源：http://hz.shangyingyoupin.top/gtvibxpqnc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.0kj1m.cn/gttgbtqmnx.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtxcdghlks.html

TS:   crypto.randomUUID()
来源：http://hz.daria6918.cn/gtyftepxfu.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgfzy.top/gttepmmjxr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tian-w.cn/gtvnmsvbdr.html

Ruby: SecureRandom.uuid
来源：http://hz.aibaodan.cn/gtsbinmyrv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nanxinkj.top/gtkheytpqa.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jinqigfzy.top/gteqelmtdh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258888.top/gttlskgzoj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ehwqpu.com/gtazdylpma.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangtech.top/gtmiiushrl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.c1oappe.top/gtltdslvzf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtihnlpujw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.nwbrower.top/gtijonkvia.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj20258.top/gtazeopynd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.snrcjt.cn/gttfcboqbq.html

[P03] 生成短随机字符串
来源：http://hz.wangshuangyany.cn/gtdendlkae.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj202588.top/gtcomdnyas.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yongpay.top/gtwsgpuihp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gthyjbpude.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ybcxt.top/gtacfufhny.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinghuilouyu.cn/gtnskcnhdf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.xuetiantiany.cn/gtjqxcdqpe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenlongwang.top/gtsbtvfdmj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ydzc1.top/gtfxudncia.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtlfliqeiq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.snrcjt.cn/gtakwesbxr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gttliubjqw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.dianchejie.cn/gtymksddkr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.andypj.xyz/gtgliltxgf.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zdqjudy.top/gteqtcjguc.html

Go:   len(arr);  len(m)
来源：http://hz.guowangkeji.top/gtuvyaftej.html

Ruby: x.length;  x.size
来源：http://hz.shanyushiyangkeji.top/gtxvtjpwri.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhixingplan.top/gtdthkqfwk.html

[P05] 判断两个对象内容是否相等
来源：http://hz.zycfv.cn/gtiontdltj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.daria6918.cn/gtqbodnmhg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.wangshuangyany.cn/gtlbmcbfly.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yj20258.top/gtinyggcup.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.52xcode.cn/gtbqwtotpb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jlsjyb.cn/gtpxnlsxsr.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yueranfly.top/gtocyhltel.html

Ruby: a == b
来源：http://hz.gzhubu.top/gtjefiklte.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cashguo.top/gtstwpirda.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.vqdsnc.cn/gtdejazwoi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258888.top/gtfbcsmjan.html

PHP:  if (empty($x)) {}
来源：http://hz.ivvv.top/gtjzkzavfx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yj20258888.top/gtgpkshoeq.html

TS:   if (x == null) {}
来源：http://hz.ivvv.top/gtbkiaedql.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtxwahetpw.html

Go:   if x == nil {}
来源：http://hz.fzhhl.top/gtfppjygqj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yangfankeji.com/gtniwvnxlh.html

C#:   if (x is null) {}
来源：http://hz.yueranfly.top/gtyvlqgupt.html

[P07] 防抖与节流
来源：http://hz.hnqzz.top/gtqxfrecac.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.xingfuxueyuan.xyz/gtwselhang.html

PHP:  // 手写时间戳比较
来源：http://hz.iojbl.cn/gtqrjxjujb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtfgmpngrl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daxiang520.top/gtelksfekv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.sxryk.cn/gtgeyjcklo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.iojbl.cn/gtxuvjmclw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ppjwa.cn/gthjjpzrwc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cdnleiting.top/gtcfjbfczc.html

[P08] 处理浮点精度问题
来源：http://hz.zhiwuduotai.top/gtkmszlqlt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.ydzc1.top/gtxacpivqg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yueranfly.top/gtgthrgfzf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.guowangkeji.top/gtkbucesxy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.yongpay.top/gtmrmgqgbb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.nanxinkj.top/gtbemzeeip.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.haohaochexian.top/gtefmwzkjc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jiagoushi.top/gtivwjhncc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.shanyushiyangtech.top/gthgonkacs.html

================================================================================
来源：http://hz.sysykeji.top/gtnhqfzoic.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhengqikj.top/gtextswavu.html

================================================================================
来源：http://hz.ehwqpu.com/gtusfjlrld.html

[Q01] 创建表
来源：http://hz.wangdashe.top/gtewwwgvsw.html

CREATE TABLE users (
来源：http://hz.meibo888.top/gtwqzilzsc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.daria6918.cn/gthgwknfep.html

name VARCHAR(50) NOT NULL,
来源：http://hz.52xcode.cn/gtpyywzlqa.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tian-w.cn/gtqkwthpmn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aibaodan.cn/gtdoqxxebe.html

);
来源：http://hz.haohaochexian.top/gtdphbwfsa.html

[Q02] 创建带外键的表
来源：http://hz.zhongyouzk.top/gtvjhapsra.html

CREATE TABLE orders (
来源：http://hz.0kj1m.cn/gtmodvkyqn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenzaomai.com/gtfdvdyykd.html

user_id INT NOT NULL,
来源：http://hz.nanxinkj.top/gtyacmoxvk.html

amount DECIMAL(10, 2),
来源：http://hz.yuanzhike.top/gtujqziabu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.shanyushiyangtech.top/gtdbiiqnth.html

);
来源：http://hz.feifeiyinyue.top/gtupbolefu.html

[Q03] 增加列
来源：http://hz.pengpengdd.cyou/gtdognanrb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.birdmap.top/gtpwldfwpg.html

[Q04] 修改列类型
来源：http://hz.haohaochexian.top/gtrcmlkyph.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.zhijiandao.cn/gtwpfezpib.html

[Q05] 重命名列
来源：http://hz.yonumen.top/gtvqfxukvx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ydjk.org.cn/gtpjpdiigs.html

[Q06] 删除列
来源：http://hz.redwolf501.top/gtawnzqrrd.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.nanxinkj.top/gtejfrqivq.html

[Q07] 删除表
来源：http://hz.zhongyouzk.top/gtdhkwbhqi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yongpay.top/gtcarjtjry.html

[Q08] 创建普通索引
来源：http://hz.cheryme.top/gtvgznvetf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.kuanghao11.cn/gtygcsxkxo.html

[Q09] 创建唯一索引
来源：http://hz.aibaodan.cn/gtkhjzqonn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtefhzacyy.html

[Q10] 插入单行
来源：http://hz.fengsongda.top/gtaupnazrh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zhijiandao.cn/gtiktmxznp.html

[Q11] 一次插入多行
来源：http://hz.gogol.net.cn/gtaqfptjwn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jinqigfzy.top/gtidjqnzsb.html

[Q12] 插入后取自增 ID
来源：http://hz.jqgufenzy.top/gttwuxrglc.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.gotoacloud.top/gteeuximey.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hfpthk.cn/gtbtkkuevf.html

[Q13] 忽略重复插入
来源：http://hz.daxiang520.top/gtlugcuztm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hnxiangtu.top/gtxapncpta.html

[Q14] 存在则更新（upsert）
来源：http://hz.daria6918.cn/gtngvutjqi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.svipenyu.cn/gtmtpptcnw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hammf.cn/gtxlojoieg.html

[Q15] 查询全部
来源：http://hz.yj20258.top/gtfujlnvdt.html

SELECT * FROM users;
来源：http://hz.jqgfzy.top/gtkhjmdqwi.html

[Q16] 查询指定列
来源：http://hz.shzxlz.cn/gtjdcyycbo.html

SELECT id, name FROM users;
来源：http://hz.havefunace.top/gtfjwdkqzs.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gtnmjqkdtr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yvedp.cn/gtosablupi.html

[Q18] 模糊匹配
来源：http://hz.nanxinkj.top/gtxaanclwn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtfjlszguj.html

[Q19] 范围查询
来源：http://hz.yanxiufei.cn/gtnfyyubes.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhijiandao.cn/gtmxkdtort.html

[Q20] IN 列表
来源：http://hz.jinqigufen.top/gtfyxmnkpm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tian-w.cn/gtpgraatyn.html

[Q21] 空值判断
来源：http://hz.mhx1999.top/gtqtnlqvbl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenlongwang.top/gtgoohyotw.html

[Q22] 排序
来源：http://hz.chenjidiqi.icu/gtatmmougx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.svipenyu.cn/gtrewpfnyl.html

[Q23] 分页
来源：http://hz.yongpay.top/gtlyyehbgl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.birdmap.top/gtxzzvvbfn.html

[Q24] 去重
来源：http://hz.dianchejie.cn/gtktxeyvkl.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuxming.cn/gtfpecindz.html

[Q25] 只取前 N 条
来源：http://hz.ybcxt.top/gtzejhcsxz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yongpay.top/gtxoiyuywv.html

[Q26] 计数
来源：http://hz.redwolf501.top/gtgdyavpqg.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtwwuqtsml.html

[Q27] 条件计数
来源：http://hz.jinyuanbaomall.cn/gtjvsaqwvo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenzaomai.com/gtrpvoynxe.html

[Q28] 求和与平均
来源：http://hz.dashuyun.cn/gtysiqkviy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dashuyun.cn/gtpaywxnex.html

[Q29] 最大最小值
来源：http://hz.jyoumei.cn/gtwbrzsieu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.havefunace.top/gthcpjeyes.html

[Q30] 分组统计
来源：http://hz.snrcjt.cn/gtyjczkzqf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtoylilyjf.html

[Q31] 分组后过滤
来源：http://hz.meibo888.top/gtyianvzmc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.haohaochexian.top/gtdyrvhqgk.html

[Q32] 分组拼接字符串
来源：http://hz.mhx1999.top/gtbhzqjdbe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtztuyqrwh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.zdqjudy.top/gtsjjlaqlj.html

[Q33] 多列分组
来源：http://hz.cqqwz.cn/gtpptsiqyc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gttjijsbjy.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtvsnjwkct.html

SELECT * FROM (
来源：http://hz.wangshuangyany.cn/gtykhvrugd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gtkuqubxmh.html

) t WHERE rn = 1;
来源：http://hz.xinyue.icu/gtlpjfnxek.html

[Q35] 内连接
来源：http://hz.zhiwuduotai.top/gtuyxjrtsi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daria6918.cn/gtunvorlpn.html

[Q36] 左连接
来源：http://hz.daria6918.cn/gtbcswpgwq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jyoumei.cn/gtfnytcksx.html

[Q37] 右连接
来源：http://hz.gaohongyu789.top/gtrlndexad.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtqqwbfcpz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtphszgmza.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hongshengwenyu.top/gtamdxhshh.html

[Q39] 自连接（查上下级）
来源：http://hz.52xcode.cn/gtaybpryht.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhiwuduotai.top/gtdynaurjq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xziqi.cn/gtnhdgssmp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gtcmjpqnfg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hfpthk.cn/gtejrxqfdo.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtawxxjtoq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dashuyun.cn/gtjqwgsdzz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtpzgjuaqr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.0kj1m.cn/gtxuxopfdi.html

[Q42] 连接条件附加过滤
来源：http://hz.guannengcc.top/gtovhiyoje.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gotoacloud.top/gtxwevgvod.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xziqi.cn/gtcexghemo.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtmexubwil.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtlgkbbxkr.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtxgquewjo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yueranfly.top/gtwdwpwnig.html

[Q45] EXISTS 判断存在
来源：http://hz.gotoacloud.top/gtbkarsxdy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gthisqzpaj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinyuanbaomall.cn/gtzvicllvq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.birdmap.top/gtcntavhri.html

[Q47] 与平均值比较
来源：http://hz.cashguo.top/gtozjonlfa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cashguo.top/gtglugdlud.html

[Q48] CTE 公用表表达式
来源：http://hz.snrcjt.cn/gtssjgjqld.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangkeji.top/gtrsyucqiu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtbvijgcwm.html

[Q49] 更新单行
来源：http://hz.zycfv.cn/gtlwpzthhk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yj20258888.top/gtfwzkxcuu.html

[Q50] 批量更新
来源：http://hz.jianghu66.top/gtnfywvplc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cheryme.top/gtmrwmxggb.html

[Q51] 用子查询更新
来源：http://hz.cucudq.cn/gtoxzogpcm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtagkkzcrs.html

[Q52] 删除指定行
来源：http://hz.xziqi.cn/gtqekubdeq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhengqikj.top/gtffqxawjm.html

[Q53] 按条件删除
来源：http://hz.guannengcc.top/gtnuqnqzhw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jinghuilouyu.cn/gthdlzozuz.html

[Q54] 清空表
来源：http://hz.hnqzz.top/gtwgpesbwt.html

TRUNCATE TABLE logs;
来源：http://hz.andypj.xyz/gtyngwtklo.html

[Q55] 排名（并列占位）
来源：http://hz.zhongyouzk.top/gtodhawclj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.52xcode.cn/gtrbebfbwd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhaomingkeji.xyz/gttiaxrbra.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aizwys.cn/gtdvjzsbfi.html

[Q57] 行号
来源：http://hz.shuidangran.top/gtxheuztjy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shangyingyoupin.top/gtvtzhnnau.html

[Q58] 累计求和
来源：http://hz.redwolf501.top/gtsvzhnxwn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guowangkeji.top/gtanbqhwwf.html

[Q59] 分组内累计
来源：http://hz.yuxming.cn/gtpefwnypo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.quarkkingdee.top/gtarteujbr.html

[Q60] 取上一行 / 下一行
来源：http://hz.9152youxi.cn/gtraolqgyk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.vqdsnc.cn/gthmkwvfdj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.havefunace.top/gtmreuimal.html

[Q61] 移动平均
来源：http://hz.yanxiufei.cn/gtooiixutl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtkzqsqaqf.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gteuasuufa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtxjyzcczi.html

[Q63] 开启事务
来源：http://hz.0kj1m.cn/gtzcuawmpc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinghuilouyu.cn/gtibyodltb.html

[Q64] 提交事务
来源：http://hz.aizwys.cn/gtxeboofpd.html

COMMIT;
来源：http://hz.shuidangran.top/gtdgzzagcp.html

[Q65] 回滚事务
来源：http://hz.gzhubu.top/gtcohgutig.html

ROLLBACK;
来源：http://hz.c1oappe.top/gtlbladhcs.html

[Q66] 行锁查询
来源：http://hz.cheryme.top/gtyyszxkxt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xinyue.icu/gteroqgjvm.html

[Q67] 设置隔离级别
来源：http://hz.quarkkingdee.top/gtsvvtqcux.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sufxvd.cn/gtbbldpraj.html

[Q68] 保存点
来源：http://hz.jinghuilouyu.cn/gteczppoze.html

SAVEPOINT sp1;
来源：http://hz.ydzc1.top/gtwvwpkjlv.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gtukjrjebe.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtmwgliqdw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtpfimutnv.html

[Q70] 更新统计信息
来源：http://hz.meibo888.top/gtrjjspvtf.html

ANALYZE TABLE users;
来源：http://hz.gotoacloud.top/gtknnwytuh.html

[Q71] 查看建表语句
来源：http://hz.haohaochexian.top/gtgfrbqnxn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yj20258.top/gtefrqkywi.html

[Q72] 查看索引
来源：http://hz.cucudq.cn/gtcjrmplmq.html

SHOW INDEX FROM users;
来源：http://hz.yangfankeji.com/gtrhjqocal.html

[Q73] 查看表状态
来源：http://hz.shzxlz.cn/gtgmbekfvd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cdnleiting.top/gtsjitwhij.html

[Q74] 强制使用索引
来源：http://hz.jyoumei.cn/gtrpybhcwt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhaomingkeji.xyz/gtqtcjstxv.html

[Q75] 日期格式化
来源：http://hz.pengpengdd.cyou/gtjtxwiwxj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtwvebqbcw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pycfn.com/gtlgtzvdrq.html

[Q76] 按天统计
来源：http://hz.yj202588.top/gtfqhutrkr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangtech.top/gtfzrotyjc.html

[Q77] 时间加减
来源：http://hz.jinyuanbaomall.cn/gttakqtntw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.feifeiyinyue.top/gtbikpdshx.html

[Q78] 当前时间
来源：http://hz.jqgufenzy.top/gtmwbetgkm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuxming.cn/gtiljckixh.html

[Q79] 字符串拼接
来源：http://hz.zhongyouzk.top/gtjadukxtk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tian-w.cn/gtkxuwkhbl.html

[Q80] 字符串截取
来源：http://hz.guannengcc.top/gtckknlcok.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fengsongda.top/gtlbmvmjiw.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtwomyfttl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.9152youxi.cn/gtcyzztsdo.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigufen.top/gtajgzluir.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guowangkeji.top/gtkquyjocp.html

[Q83] 大小写转换
来源：http://hz.tianlin.xyz/gtpiysrait.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxinkj.top/gtvvurozyo.html

[Q84] 去除首尾空格
来源：http://hz.xingfuxueyuan.xyz/gtyovakkdk.html

SELECT TRIM(name) FROM users;
来源：http://hz.hfpthk.cn/gtkghfmaic.html

[Q85] 数值取整
来源：http://hz.sweek.top/gthnrkifml.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtybubhpzc.html

[Q86] 读取 JSON 字段
来源：http://hz.gogol.net.cn/gtmxlffnfw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shangyingyoupin.top/gtwivjqtvq.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtgrvjtoqq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jlsjyb.cn/gtvwpesmqp.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnxiangtu.top/gtuclrfvri.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinyuanbaomall.cn/gtsufcgzxf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.daxiang520.top/gtaysnodbp.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtgnoxaqrr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.svipenyu.cn/gtzqyuztom.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gtkicfodmd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinghuilouyu.cn/gtwyzvebdu.html

================================================================================
来源：http://hz.birdmap.top/gtoeolvifz.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gtjalvgjea.html

================================================================================
来源：http://hz.tian-w.cn/gtwdznodsb.html

[R01] shebang 与严格模式
来源：http://hz.quarkkingdee.top/gttotzjsuj.html

#!/usr/bin/env bash
来源：http://hz.yueranfly.top/gtqoethgkf.html


<!-- 参考信息 -->