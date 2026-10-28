代发 wailian999

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtnxwklmxi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yanxiufei.cn/gtagtzphue.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ehwqpu.com/gttkmvbyfn.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtyyvashev.html

TS:   // child_process / cluster 模块
来源：http://hz.pengpengdd.cyou/gtpssxhslt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ppjwa.cn/gtfhssfwmp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xylfe.cn/gtvgojjukt.html

Ruby: // fork 块
来源：http://hz.jinyuanbaomall.cn/gtfghbqyys.html

C#:   Parallel.For
来源：http://hz.zhengqikj.top/gtbzoomhvp.html

================================================================================
来源：http://hz.redwolf501.top/gtxnokvomn.html

P. 常用工具函数
来源：http://hz.gotoacloud.top/gtujldrrzv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwbnqhilx.html

[P01] 生成 UUID
来源：http://hz.nwbrower.top/gtglqiraju.html

Py:   str(uuid.uuid4())
来源：http://hz.ydjk.org.cn/gtqdhibapk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.quarkkingdee.top/gtshakdhzs.html

JS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtntdqtuxh.html

TS:   crypto.randomUUID()
来源：http://hz.aizwys.cn/gtjofhguuj.html

Java: UUID.randomUUID().toString()
来源：http://hz.nwbrower.top/gtdtvaneva.html

Go:   // 用 github.com/google/uuid
来源：http://hz.sufxvd.cn/gtlhoqmzhi.html

Ruby: SecureRandom.uuid
来源：http://hz.zhaomingkeji.xyz/gttxrggdyr.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258.top/gtrrjgenld.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sxryk.cn/gtoomeevxf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.dianchejie.cn/gtguaskzoi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhongyouzk.top/gtkwprpdth.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.redwolf501.top/gtaelzkqsz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yuanzhike.top/gtwtrogutn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shzxlz.cn/gthcktmxud.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.9152youxi.cn/gtgfnkusse.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yangfankeji.com/gtpipjaetq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.iojbl.cn/gtfgiofqzy.html

[P03] 生成短随机字符串
来源：http://hz.pengpengdd.cyou/gtyehxovhd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ppjwa.cn/gtcwnrluaw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yj202588.top/gtenkcnnam.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinghuilouyu.cn/gtcjftbbru.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.sysykeji.top/gtorcduchh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.fzhhl.top/gtanzvwtzt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ywan-chungtsiang.top/gtsmkjnlch.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gtcwonvndb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gzhubu.top/gtpvfzoore.html

[P04] 求长度
来源：http://hz.ydzc1.top/gtrqaupsbr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.shangyingyoupin.top/gtxjtbyyyv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtsrqnkmsk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuxming.cn/gtafazkvzl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtxrxxwxmy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.birdmap.top/gtcelsqkoz.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtpuzabyzi.html

Ruby: x.length;  x.size
来源：http://hz.wangdashe.top/gtomckjmhy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.vqdsnc.cn/gtysvkdvlm.html

[P05] 判断两个对象内容是否相等
来源：http://hz.guowangkeji.top/gtyykizffd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.shanyushiyangkeji.top/gtsoisowau.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtickjmcsh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.chenlongwang.top/gtmbbkgbow.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtgsdmyipd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ppjwa.cn/gtkoaznopu.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhiwuduotai.top/gtryrtsqof.html

Ruby: a == b
来源：http://hz.gogol.net.cn/gtruseyevx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhongyouzk.top/gthafjkgqc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.0kj1m.cn/gtjzdjsbgn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zycfv.cn/gthfeykxcu.html

PHP:  if (empty($x)) {}
来源：http://hz.birdmap.top/gtjrzalfot.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhijiandao.cn/gtsootchty.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtiytwsxsr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtkehbfrmv.html

Go:   if x == nil {}
来源：http://hz.havefunace.top/gtmsoqvhdj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hfpthk.cn/gtthjbvqrp.html

C#:   if (x is null) {}
来源：http://hz.pengpengdd.cyou/gtxdjmprzv.html

[P07] 防抖与节流
来源：http://hz.hammf.cn/gtquwlbokr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.daxiang520.top/gtqwuqfvyt.html

PHP:  // 手写时间戳比较
来源：http://hz.zhijiandao.cn/gtfwomuald.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtpytjudmy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.aizwys.cn/gtfigabqul.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zycfv.cn/gtdwoxhvws.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hywenlv.cn/gtvujbsdfz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yanxiufei.cn/gtadwpejvl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xuanzx.com/gtisafbmjd.html

[P08] 处理浮点精度问题
来源：http://hz.gzhubu.top/gtwekkrjsl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.smart0.xyz/gtriyemecr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.kuanghao11.cn/gtukaezise.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.aibaodan.cn/gtffvkaqcm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.gaohongyu789.top/gtjoftoddh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.zycfv.cn/gtylwtoxqn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.iojbl.cn/gtzojfwsyj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.fengsongda.top/gttdocfjqs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.chenjidiqi.icu/gtcethczok.html

================================================================================
来源：http://hz.xylfe.cn/gtuofhvypf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.xziqi.cn/gtzheeurtl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtvdvggpjy.html

[Q01] 创建表
来源：http://hz.shuidangran.top/gtjjnadupn.html

CREATE TABLE users (
来源：http://hz.xingfuxueyuan.xyz/gtnurtljzc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jinqigfzy.top/gtchbmgnsd.html

name VARCHAR(50) NOT NULL,
来源：http://hz.gaohongyu789.top/gtmeqdzhjt.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tanke756.top/gtbyoctali.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fzhhl.top/gtpmoqjwnu.html

);
来源：http://hz.jinyuanbaomall.cn/gtksfjhtqu.html

[Q02] 创建带外键的表
来源：http://hz.ywan-chungtsiang.top/gtwtvohlpk.html

CREATE TABLE orders (
来源：http://hz.shanyushiyangtech.top/gthsljbvos.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jlsjyb.cn/gtonbpvnch.html

user_id INT NOT NULL,
来源：http://hz.aizwys.cn/gtnucqorgx.html

amount DECIMAL(10, 2),
来源：http://hz.chenzaomai.com/gtjfqyhmoc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.haohaochexian.top/gtxsrjpxpa.html

);
来源：http://hz.9152youxi.cn/gtcqtvosvu.html

[Q03] 增加列
来源：http://hz.aibaodan.cn/gtfjiadegg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yanxiufei.cn/gtllwecyws.html

[Q04] 修改列类型
来源：http://hz.yanxiufei.cn/gtnfjklgph.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jyoumei.cn/gtohgfbmvz.html

[Q05] 重命名列
来源：http://hz.cashguo.top/gtkdljrcrs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yj20258.top/gtbgvrhxsg.html

[Q06] 删除列
来源：http://hz.cqqwz.cn/gtaaoywzdv.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xinyue.icu/gtymhuejko.html

[Q07] 删除表
来源：http://hz.sxryk.cn/gtjjlkejcy.html

DROP TABLE IF EXISTS orders;
来源：http://hz.cheryme.top/gtjtlkchsa.html

[Q08] 创建普通索引
来源：http://hz.hnxiangtu.top/gtbqcnvbpg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.jlsjyb.cn/gtjntrbivl.html

[Q09] 创建唯一索引
来源：http://hz.9152youxi.cn/gtsmjeokhz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.dianchejie.cn/gtjrjennpj.html

[Q10] 插入单行
来源：http://hz.jqgufenzy.top/gtxfkgtchk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shangyingyoupin.top/gtngdbqjvg.html

[Q11] 一次插入多行
来源：http://hz.yuxming.cn/gtzrhokyim.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ywan-chungtsiang.top/gtqvblpnko.html

[Q12] 插入后取自增 ID
来源：http://hz.mhx1999.top/gtasqvhxmm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhixingplan.top/gtknfwnxsd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.chenzaomai.com/gttugprebv.html

[Q13] 忽略重复插入
来源：http://hz.redwolf501.top/gtnbhwrmlt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.andypj.xyz/gtzisddnaa.html

[Q14] 存在则更新（upsert）
来源：http://hz.zycfv.cn/gtajxngxwy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shuidangran.top/gthowbqtiv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yonumen.top/gtdzeefjkm.html

[Q15] 查询全部
来源：http://hz.jinyuanbaomall.cn/gtgtzqbbwa.html

SELECT * FROM users;
来源：http://hz.yangfankeji.com/gtxhjjiyho.html

[Q16] 查询指定列
来源：http://hz.jiagoushi.top/gteauvnjuy.html

SELECT id, name FROM users;
来源：http://hz.xinyue.icu/gtztkzcywz.html

[Q17] 条件查询
来源：http://hz.yangfankeji.com/gtoamhxzsf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuanzhike.top/gtsuqxzutz.html

[Q18] 模糊匹配
来源：http://hz.hywenlv.cn/gtokivqsfh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.andypj.xyz/gtsosgviuh.html

[Q19] 范围查询
来源：http://hz.daria6918.cn/gtkxxflysc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sxryk.cn/gtblymoqak.html

[Q20] IN 列表
来源：http://hz.yj202588.top/gtcwltxlgp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yj20258888.top/gtqcuxmzdb.html

[Q21] 空值判断
来源：http://hz.zhiwuduotai.top/gtjpsubfsp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnqzz.top/gtggfbdxnf.html

[Q22] 排序
来源：http://hz.guannengcc.top/gtadvxeirq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.dashuyun.cn/gtobanpugp.html

[Q23] 分页
来源：http://hz.ybcxt.top/gtftdczebr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aibaodan.cn/gtzzwcesro.html

[Q24] 去重
来源：http://hz.zhijiandao.cn/gtgzudyvcx.html

SELECT DISTINCT city FROM users;
来源：http://hz.jqgfzy.top/gthnhconbv.html

[Q25] 只取前 N 条
来源：http://hz.iojbl.cn/gtxjjxfthk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.nanxinkj.top/gtlqedvopm.html

[Q26] 计数
来源：http://hz.kuanghao11.cn/gteukngbae.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuanzx.com/gttdjuweyq.html

[Q27] 条件计数
来源：http://hz.shanyushiyangtech.top/gtruhbxoxf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nwbrower.top/gtixcgyvie.html

[Q28] 求和与平均
来源：http://hz.andypj.xyz/gtqdpdoelb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jyoumei.cn/gtoaqtgbdp.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangkeji.top/gtjgwsrxdl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhoulong.xyz/gttxthtvyz.html

[Q30] 分组统计
来源：http://hz.fengsongda.top/gtfawrbbyt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtzbxnubaf.html

[Q31] 分组后过滤
来源：http://hz.cheryme.top/gtkawxeohx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pengpengdd.cyou/gtcnbqgzlz.html

[Q32] 分组拼接字符串
来源：http://hz.aizwys.cn/gtkavcvcny.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.aibaodan.cn/gtsqpeazpq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj202588.top/gtpgtfnjth.html

[Q33] 多列分组
来源：http://hz.ybcxt.top/gtatvjpvym.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hywenlv.cn/gtcfjojpnp.html

[Q34] 每组取第一条
来源：http://hz.ydzc1.top/gtuvnyzgqq.html

SELECT * FROM (
来源：http://hz.cashguo.top/gtazbczcjo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.gaohongyu789.top/gtjndxsvvl.html

) t WHERE rn = 1;
来源：http://hz.meibo888.top/gthzcnfbjr.html

[Q35] 内连接
来源：http://hz.vqdsnc.cn/gttmubrvtg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.guowangkeji.top/gteprivqyh.html

[Q36] 左连接
来源：http://hz.pengpengdd.cyou/gtpdncaykt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtdykkdmos.html

[Q37] 右连接
来源：http://hz.gzhubu.top/gtovpleyom.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuanzx.com/gtqiagaxks.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.redwolf501.top/gttkzccmkk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.chenzaomai.com/gtltqiguoq.html

[Q39] 自连接（查上下级）
来源：http://hz.0kj1m.cn/gtzjwufsnb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258888.top/gtmeramvlu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hnxiangtu.top/gtcotyfjda.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daxiang520.top/gtnqjdqoqv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gaohongyu789.top/gtplvikyrp.html

[Q41] 多表连接
来源：http://hz.havefunace.top/gtljflckdp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gthvnrurxw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtbpjcsbvs.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj20258888.top/gtpantwrge.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgfzy.top/gtlzqeqalw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hywenlv.cn/gtesmugojx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.guowangkeji.top/gtcairmpyw.html

[Q43] 标量子查询
来源：http://hz.quarkkingdee.top/gtgrrvqixk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yongpay.top/gtwadcglcn.html

[Q44] IN 子查询
来源：http://hz.chenlongwang.top/gthpthohju.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.kuanghao11.cn/gtlviwcclf.html

[Q45] EXISTS 判断存在
来源：http://hz.xylfe.cn/gtmzwwiqpa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxuanxn.top/gtapczjbvs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.fzhhl.top/gtgdmvenne.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtdlbmpeih.html

[Q47] 与平均值比较
来源：http://hz.zycfv.cn/gtexneptka.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydjk.org.cn/gttpztjzto.html

[Q48] CTE 公用表表达式
来源：http://hz.cqqwz.cn/gtwaacqxte.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guowangkeji.top/gthepqvtkr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hammf.cn/gtevpksrhw.html

[Q49] 更新单行
来源：http://hz.gogol.net.cn/gtwhcyimxp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tian-w.cn/gtbfhdgjxk.html

[Q50] 批量更新
来源：http://hz.hysaishi.cn/gtxpiaofxu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxuanxn.top/gtvfcbbydh.html

[Q51] 用子查询更新
来源：http://hz.sxryk.cn/gthzhxuapu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.redwolf501.top/gtioffcgue.html

[Q52] 删除指定行
来源：http://hz.gogol.net.cn/gtazspjpyx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtazlmsrxf.html

[Q53] 按条件删除
来源：http://hz.jqgufenzy.top/gtjufcvfkh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sweek.top/gtnpiwsmcq.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtxtmruacw.html

TRUNCATE TABLE logs;
来源：http://hz.chenlongwang.top/gtwvpveavh.html

[Q55] 排名（并列占位）
来源：http://hz.cashguo.top/gtftajzlrw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtddvrpaan.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhixingplan.top/gttlcocybf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yvedp.cn/gtgjvzhgvq.html

[Q57] 行号
来源：http://hz.pengpengdd.cyou/gtnnhpjzns.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.birdmap.top/gtritvjutl.html

[Q58] 累计求和
来源：http://hz.snrcjt.cn/gtpgtngtie.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cheryme.top/gtqsakustn.html

[Q59] 分组内累计
来源：http://hz.yueranfly.top/gtaoudolse.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.52xcode.cn/gtiaayhztv.html

[Q60] 取上一行 / 下一行
来源：http://hz.xinyue.icu/gtstixwnjm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ppjwa.cn/gtuscasmuy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hnxiangtu.top/gtdharepls.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtxlmmcxxu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xylfe.cn/gtkphomqzo.html

[Q62] 分组占比
来源：http://hz.smart0.xyz/gtlgbxkriv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtikwcnqjk.html

[Q63] 开启事务
来源：http://hz.nanxinkj.top/gturrracsl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daxiang520.top/gtzmklukmy.html

[Q64] 提交事务
来源：http://hz.daxiang520.top/gtlxqmlbya.html

COMMIT;
来源：http://hz.hammf.cn/gtewygajgz.html

[Q65] 回滚事务
来源：http://hz.xuetiantiany.cn/gtrpmexbja.html

ROLLBACK;
来源：http://hz.hnqzz.top/gtccatnvss.html

[Q66] 行锁查询
来源：http://hz.daria6918.cn/gtzyimdslw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhiwuduotai.top/gtqrblhxow.html

[Q67] 设置隔离级别
来源：http://hz.andypj.xyz/gtnkpsmjsc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangtech.top/gtummvdsdk.html

[Q68] 保存点
来源：http://hz.c1oappe.top/gtbcdadhry.html

SAVEPOINT sp1;
来源：http://hz.shanyushiyangkeji.top/gtvzxbactb.html

ROLLBACK TO sp1;
来源：http://hz.nanxinkj.top/gtfsnuktyx.html

[Q69] 查看执行计划
来源：http://hz.nanxinkj.top/gtpoxodzpf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yuxming.cn/gtamfoffov.html

[Q70] 更新统计信息
来源：http://hz.sysykeji.top/gtcocbapld.html

ANALYZE TABLE users;
来源：http://hz.cheryme.top/gtyveivalu.html

[Q71] 查看建表语句
来源：http://hz.fzhhl.top/gtzhhcjqms.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hfpthk.cn/gtfalyjlis.html

[Q72] 查看索引
来源：http://hz.andypj.xyz/gtndwrmohc.html

SHOW INDEX FROM users;
来源：http://hz.52xcode.cn/gtokviokzy.html

[Q73] 查看表状态
来源：http://hz.sweek.top/gtdhjftzcw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gthjucappn.html

[Q74] 强制使用索引
来源：http://hz.gzhubu.top/gtyjvqniet.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuanzx.com/gtyzsuutfc.html

[Q75] 日期格式化
来源：http://hz.bjfxy.top/gtlnwptdgy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jinghuilouyu.cn/gtlnxxkohl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.feifeiyinyue.top/gtjdqtzsfo.html

[Q76] 按天统计
来源：http://hz.fengsongda.top/gtobcgpcqw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigfzy.top/gtrcydrkbt.html

[Q77] 时间加减
来源：http://hz.tian-w.cn/gtmyjstpfc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuanzhike.top/gtpmgnlmkd.html

[Q78] 当前时间
来源：http://hz.daxiang520.top/gtvahwihuf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangkeji.top/gttebfubiy.html

[Q79] 字符串拼接
来源：http://hz.nanxinkj.top/gtswbcsxcv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nanxinkj.top/gtjuvmywqo.html

[Q80] 字符串截取
来源：http://hz.jinyuanbaomall.cn/gtmpxplenh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.havefunace.top/gtgcubmpon.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtsivungsd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gtvtahmpft.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtpidckggx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shuidangran.top/gtewsvwaop.html

[Q83] 大小写转换
来源：http://hz.zhiwuduotai.top/gtvrdzdzdr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtkgzifthw.html

[Q84] 去除首尾空格
来源：http://hz.nwbrower.top/gtxjzsoxwh.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhijiandao.cn/gtdreanjjr.html

[Q85] 数值取整
来源：http://hz.ehwqpu.com/gtetuaqawk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtemzzmdus.html

[Q86] 读取 JSON 字段
来源：http://hz.9152youxi.cn/gtvubklxus.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jlsjyb.cn/gtwosufggr.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtfwicsujv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.daxiang520.top/gttxrrxkgp.html

[Q88] 行转列（条件聚合）
来源：http://hz.cdnleiting.top/gtrhjvtppq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgufenzy.top/gtavctastp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pycfn.com/gtszotvmdx.html

[Q89] 判断表是否存在
来源：http://hz.yanxiufei.cn/gtfeefcgdv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cqqwz.cn/gtrhxzwdno.html

[Q90] 生成序号列
来源：http://hz.bjfxy.top/gtmnjxwypx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhoulong.xyz/gtveajnkte.html

================================================================================
来源：http://hz.yj202588.top/gtvurlxmfb.html

R. Bash 专题
来源：http://hz.xylfe.cn/gtfnamtels.html

================================================================================
来源：http://hz.svipenyu.cn/gtmwinabza.html

[R01] shebang 与严格模式
来源：http://hz.yongpay.top/gtlssdaeoy.html

#!/usr/bin/env bash
来源：http://hz.pycfn.com/gtfaknlavv.html

set -euo pipefail
来源：http://hz.shuidangran.top/gtdxyajvmo.html

[R02] 变量赋值与使用
来源：http://hz.sysykeji.top/gttjlxhhqx.html

name="Tom"; echo "$name"
来源：http://hz.cashguo.top/gtwkckkcto.html

[R03] 只读变量
来源：http://hz.ydzc1.top/gtzsekryou.html


<!-- 参考信息 -->