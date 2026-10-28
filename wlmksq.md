代发 wailian999

C#:   Parallel.For
来源：http://hz.daxiang520.top/gtmyjmcolp.html

================================================================================
来源：http://hz.fzhhl.top/gtkzfnxysh.html

P. 常用工具函数
来源：http://hz.haohaochexian.top/gtuqzuffnn.html

================================================================================
来源：http://hz.yongpay.top/gtbhfjetet.html

[P01] 生成 UUID
来源：http://hz.jinghuilouyu.cn/gtimwmhjmy.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtklqwoiqh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xziqi.cn/gtnursxkia.html

JS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtnpmtwqzp.html

TS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtfuarjhfc.html

Java: UUID.randomUUID().toString()
来源：http://hz.xinyue.icu/gtrnumhkqr.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hammf.cn/gtnkutrzxq.html

Ruby: SecureRandom.uuid
来源：http://hz.daria6918.cn/gtlppxgsvk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.wangshuangyany.cn/gtefbbxkon.html

[P02] MD5 / SHA256 摘要
来源：http://hz.meibo888.top/gtiszipdom.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.svipenyu.cn/gticaylycm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yj20258888.top/gtpozdsxqs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.vqdsnc.cn/gtavsbfdct.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtlojgzebr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.bjfxy.top/gtlmmdmrnx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jinqigufen.top/gtziwseyeg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.9152youxi.cn/gtigswozyz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.quarkkingdee.top/gtavnlrwwa.html

[P03] 生成短随机字符串
来源：http://hz.hysaishi.cn/gtmlaqdvfd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.c1oappe.top/gtmwizqpwf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.guowangkeji.top/gtzpfzipjs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xingfuxueyuan.xyz/gtxerxqedl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cqqwz.cn/gtcekgxrnu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj202588.top/gthibcoshx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydjk.org.cn/gtzycbizip.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.sysykeji.top/gthwqpjuhk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.nwbrower.top/gtcwzyhciz.html

[P04] 求长度
来源：http://hz.shanyushiyangtech.top/gttqlibagx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.redwolf501.top/gtafwyyhwy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtnslcuhdm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinghuilouyu.cn/gtcuvkikwz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtfscvqvoy.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jqgfzy.top/gtnkvyegsf.html

Go:   len(arr);  len(m)
来源：http://hz.cqqwz.cn/gtofxqluxq.html

Ruby: x.length;  x.size
来源：http://hz.iojbl.cn/gtinlidkof.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cucudq.cn/gtulgmvlab.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtuaugkplh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.wangdashe.top/gtrxwarbvc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.nanxuanxn.top/gthadvcrqn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtelflpezo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yj20258888.top/gtqqlfktxk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yueranfly.top/gtgntasnpc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yongpay.top/gtfzreomoc.html

Ruby: a == b
来源：http://hz.hywenlv.cn/gtslvsmlpy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cdnleiting.top/gtpxbzkmdd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.hammf.cn/gtmptstahb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.snrcjt.cn/gtzffsgmxp.html

PHP:  if (empty($x)) {}
来源：http://hz.xuanzx.com/gtquerlfez.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.sweek.top/gtjyuwbqqi.html

TS:   if (x == null) {}
来源：http://hz.xuanzx.com/gtbliwipzc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gthzgwkgxd.html

Go:   if x == nil {}
来源：http://hz.wangdashe.top/gthoztgjmu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ywan-chungtsiang.top/gtqfmncdkf.html

C#:   if (x is null) {}
来源：http://hz.shzxlz.cn/gtpawdgvds.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtlfxnafpr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jinghuilouyu.cn/gtqfhcqupe.html

PHP:  // 手写时间戳比较
来源：http://hz.xziqi.cn/gtiblconbc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtnaxdijjr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.kuanghao11.cn/gtywcrrhjz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guannengcc.top/gtljvawnbt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.cqqwz.cn/gtdmsokvym.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.aizwys.cn/gtsyhsrbft.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yueranfly.top/gtriamcvnx.html

[P08] 处理浮点精度问题
来源：http://hz.jlsjyb.cn/gttbbghsjk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shzxlz.cn/gtcculnrvu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.nanxinkj.top/gtyaofkxpi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hysaishi.cn/gtessyajug.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jlsjyb.cn/gtpmrubpzw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cdnleiting.top/gtpodkmecm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.316326.xyz/gttjzkhiaf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shuidangran.top/gtqdwubhna.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.havefunace.top/gtsagfzfag.html

================================================================================
来源：http://hz.jyoumei.cn/gtgvawhiwo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinqigufen.top/gthvhldnhh.html

================================================================================
来源：http://hz.fengsongda.top/gtqdkpedqi.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtlpaavdhw.html

CREATE TABLE users (
来源：http://hz.hongshengwenyu.top/gtyfgqbfup.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtupihyiqv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.snrcjt.cn/gtqkuomqkh.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xziqi.cn/gtefloskqv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yvedp.cn/gtqmmdvjnt.html

);
来源：http://hz.yvedp.cn/gtvcwtohco.html

[Q02] 创建带外键的表
来源：http://hz.yangfankeji.com/gtrviaeejz.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtqvaqlrpm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zycfv.cn/gtyulnajjb.html

user_id INT NOT NULL,
来源：http://hz.nanxinkj.top/gtgifuqwgd.html

amount DECIMAL(10, 2),
来源：http://hz.fzhhl.top/gtxjsiwqbz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zycfv.cn/gtbhusawlu.html

);
来源：http://hz.kuanghao11.cn/gttsoadxhr.html

[Q03] 增加列
来源：http://hz.xuanzx.com/gtavnymmag.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.0kj1m.cn/gtrgadhhtd.html

[Q04] 修改列类型
来源：http://hz.andypj.xyz/gtkkkwykmb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cucudq.cn/gtmdpbyoty.html

[Q05] 重命名列
来源：http://hz.yongpay.top/gtgkzriylm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.yangfankeji.com/gtkbmmevbi.html

[Q06] 删除列
来源：http://hz.yvedp.cn/gtsnskrlbm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yuxming.cn/gtlbjomdfk.html

[Q07] 删除表
来源：http://hz.52xcode.cn/gtvinemwhp.html

DROP TABLE IF EXISTS orders;
来源：http://hz.dianchejie.cn/gttspvqzgh.html

[Q08] 创建普通索引
来源：http://hz.jlsjyb.cn/gtqskecvev.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cucudq.cn/gthwoysign.html

[Q09] 创建唯一索引
来源：http://hz.nanxinkj.top/gtnwbpctja.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenzaomai.com/gtcucpxlnf.html

[Q10] 插入单行
来源：http://hz.hywenlv.cn/gtoxzmpogk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.dianchejie.cn/gtevmvekzd.html

[Q11] 一次插入多行
来源：http://hz.birdmap.top/gtwtejbubl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.0kj1m.cn/gtbmrjpqjx.html

[Q12] 插入后取自增 ID
来源：http://hz.dianchejie.cn/gtpbnixpub.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.316326.xyz/gtzbvpfuro.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.tianlin.xyz/gtplqtitqt.html

[Q13] 忽略重复插入
来源：http://hz.wangshuangyany.cn/gtqnodasqo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.pycfn.com/gttsvicasu.html

[Q14] 存在则更新（upsert）
来源：http://hz.aibaodan.cn/gtjeahxxlt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yuxming.cn/gtuhjjfkht.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.nanxuanxn.top/gttpervuji.html

[Q15] 查询全部
来源：http://hz.svipenyu.cn/gtftiifqam.html

SELECT * FROM users;
来源：http://hz.yj202588.top/gtvfdtlkir.html

[Q16] 查询指定列
来源：http://hz.cheryme.top/gtbrljlrmy.html

SELECT id, name FROM users;
来源：http://hz.jiagoushi.top/gtodmdvfde.html

[Q17] 条件查询
来源：http://hz.hnxiangtu.top/gtblkuvdmb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.pycfn.com/gtiggemtrq.html

[Q18] 模糊匹配
来源：http://hz.kuanghao11.cn/gtjdwixwvw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtgjgjcktq.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtvkpbmyzb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sxryk.cn/gtkzywgtjt.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtlxmdeloy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhaomingkeji.xyz/gtufzarodg.html

[Q21] 空值判断
来源：http://hz.chenlongwang.top/gtmcfvtnyt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.smart0.xyz/gtqhznksxm.html

[Q22] 排序
来源：http://hz.kuanghao11.cn/gtogkeknpc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yangfankeji.com/gtkkwzuxqh.html

[Q23] 分页
来源：http://hz.fzhhl.top/gtkqtnetqf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtohoiogoi.html

[Q24] 去重
来源：http://hz.xingfuxueyuan.xyz/gtpafjyphn.html

SELECT DISTINCT city FROM users;
来源：http://hz.zdqjudy.top/gtczuecbpt.html

[Q25] 只取前 N 条
来源：http://hz.wangshuangyany.cn/gtsmgnjcqf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sufxvd.cn/gtdjxojkpf.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gtjkyoijbl.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtlcubadnl.html

[Q27] 条件计数
来源：http://hz.xinyue.icu/gtrjigtmgs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenlongwang.top/gtirumekmo.html

[Q28] 求和与平均
来源：http://hz.hnqzz.top/gtxupwgujz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.52xcode.cn/gtgztofifx.html

[Q29] 最大最小值
来源：http://hz.yj202588.top/gtdtkusxmn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yongpay.top/gtyzzaxpke.html

[Q30] 分组统计
来源：http://hz.ehwqpu.com/gtcztjulbr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtcjjlxxds.html

[Q31] 分组后过滤
来源：http://hz.redwolf501.top/gtvthpdxzi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jianghu66.top/gtukoaizvt.html

[Q32] 分组拼接字符串
来源：http://hz.shangyingyoupin.top/gtypwvbifc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gzhubu.top/gtpckmejnw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shangyingyoupin.top/gtfveceugn.html

[Q33] 多列分组
来源：http://hz.birdmap.top/gtcjdsjgia.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.guannengcc.top/gtwywrltlz.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtrytcwnzt.html

SELECT * FROM (
来源：http://hz.bjfxy.top/gtumdamyhi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinghuilouyu.cn/gtavpuepah.html

) t WHERE rn = 1;
来源：http://hz.316326.xyz/gtfcgqoquo.html

[Q35] 内连接
来源：http://hz.quarkkingdee.top/gtizlowzvw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gttikutyjb.html

[Q36] 左连接
来源：http://hz.gaohongyu789.top/gtocehibva.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnqzz.top/gtnfszbycg.html

[Q37] 右连接
来源：http://hz.yj202588.top/gtpltfjltx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hammf.cn/gtbbezcyac.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pycfn.com/gtzwsdwmjs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuxming.cn/gthriegeyl.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigfzy.top/gthenvqgvy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.aizwys.cn/gtiubmited.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.meibo888.top/gtoghmiros.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yonumen.top/gtofchuaod.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dashuyun.cn/gtketdrrcb.html

[Q41] 多表连接
来源：http://hz.cucudq.cn/gtakbvwnuy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.sweek.top/gtkrotakkw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ybcxt.top/gtkjmebsqy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yangfankeji.com/gtjgkkpffq.html

[Q42] 连接条件附加过滤
来源：http://hz.andypj.xyz/gtdgjvbdwe.html

SELECT u.name, o.amount FROM users u
来源：http://hz.cheryme.top/gtqjvjhnnq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fengsongda.top/gtjjjpcvtb.html

[Q43] 标量子查询
来源：http://hz.ybcxt.top/gtkcrfnhpr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenjidiqi.icu/gtfeocjomn.html

[Q44] IN 子查询
来源：http://hz.yongpay.top/gtswalatrk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guannengcc.top/gtpyjzetlm.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgfzy.top/gtrkapkscm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtleqhbxfs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.iojbl.cn/gtcuoejxev.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258.top/gtfqzevevx.html

[Q47] 与平均值比较
来源：http://hz.pengpengdd.cyou/gtrtqtkpye.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dianchejie.cn/gtwblxbtyo.html

[Q48] CTE 公用表表达式
来源：http://hz.xinyue.icu/gtcngdhxqp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtlnxtkzfk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.smart0.xyz/gtvibbzvgw.html

[Q49] 更新单行
来源：http://hz.jinyuanbaomall.cn/gtymjmqgri.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gaohongyu789.top/gttdgbvzbc.html

[Q50] 批量更新
来源：http://hz.haohaochexian.top/gtioradfmq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.haohaochexian.top/gtlkznnwsr.html

[Q51] 用子查询更新
来源：http://hz.yuanzhike.top/gtvhkzbrlm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dashuyun.cn/gtdltznmum.html

[Q52] 删除指定行
来源：http://hz.birdmap.top/gttlkjisgb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtuvpujbce.html

[Q53] 按条件删除
来源：http://hz.nanxuanxn.top/gtmsbhwhjo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.fengsongda.top/gteaqfvamk.html

[Q54] 清空表
来源：http://hz.zdqjudy.top/gtwbhceyzb.html

TRUNCATE TABLE logs;
来源：http://hz.jianghu66.top/gtnvkaadrt.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtohwcunmt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.meibo888.top/gtllnypaqo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhiwuduotai.top/gtbciywgeq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guannengcc.top/gtpeylsgcr.html

[Q57] 行号
来源：http://hz.sweek.top/gtozsqkgab.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinghuilouyu.cn/gteieysddn.html

[Q58] 累计求和
来源：http://hz.tanke756.top/gtjbakkwaw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenjidiqi.icu/gtsmxpibdn.html

[Q59] 分组内累计
来源：http://hz.zhengqikj.top/gtnugmgzrq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tian-w.cn/gtxngrwtkx.html

[Q60] 取上一行 / 下一行
来源：http://hz.cashguo.top/gtwdcgjnhq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xingfuxueyuan.xyz/gtfyjeditx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuetiantiany.cn/gtilipbemd.html

[Q61] 移动平均
来源：http://hz.birdmap.top/gtggortdry.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtroynvjaz.html

[Q62] 分组占比
来源：http://hz.daria6918.cn/gttcuzqnfj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtcjbossor.html

[Q63] 开启事务
来源：http://hz.wangshuangyany.cn/gtqhiyrctl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ybcxt.top/gtnthhfyje.html

[Q64] 提交事务
来源：http://hz.ehwqpu.com/gtriixznpn.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtemqurdpv.html

[Q65] 回滚事务
来源：http://hz.hywenlv.cn/gttddtopra.html

ROLLBACK;
来源：http://hz.zdqjudy.top/gturyuvlmr.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtthyfeptr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangdashe.top/gtfbnrwrrh.html

[Q67] 设置隔离级别
来源：http://hz.nanxuanxn.top/gtngcvjbhf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nanxuanxn.top/gtwcuqwafc.html

[Q68] 保存点
来源：http://hz.chenjidiqi.icu/gtnnbbnsqz.html

SAVEPOINT sp1;
来源：http://hz.52xcode.cn/gteddeqhrf.html

ROLLBACK TO sp1;
来源：http://hz.cashguo.top/gtyykzzaib.html

[Q69] 查看执行计划
来源：http://hz.zhoulong.xyz/gtvvoygsbw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xuanzx.com/gtvomziavl.html

[Q70] 更新统计信息
来源：http://hz.ehwqpu.com/gtoiailvpf.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtfgttyydu.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gthxhgtlem.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sweek.top/gtqegfyvxp.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gtzogoyjlh.html

SHOW INDEX FROM users;
来源：http://hz.nwbrower.top/gtizckzptc.html

[Q73] 查看表状态
来源：http://hz.hywenlv.cn/gthlgttpqf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pycfn.com/gtgpfkgusn.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gthkktadqb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tianlin.xyz/gthqqvurhm.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtnibfmkex.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jlsjyb.cn/gtobqcqajn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuxming.cn/gtqzpwjgwj.html

[Q76] 按天统计
来源：http://hz.sxryk.cn/gtwkbpjhxf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtibfrcswv.html

[Q77] 时间加减
来源：http://hz.hywenlv.cn/gtmuvpknvn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtdnwkvuva.html

[Q78] 当前时间
来源：http://hz.zhiwuduotai.top/gtamrbnmik.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fengsongda.top/gtsoguejvv.html

[Q79] 字符串拼接
来源：http://hz.sxryk.cn/gtproobqev.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtkpknoofa.html

[Q80] 字符串截取
来源：http://hz.ydjk.org.cn/gtezueyenp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenzaomai.com/gtzytlnfqd.html

[Q81] 字符串替换
来源：http://hz.nwbrower.top/gtbbuoogiy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gogol.net.cn/gtlnojyqll.html

[Q82] 字符长度与字节长度
来源：http://hz.sysykeji.top/gtaiaelqsp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnxiangtu.top/gtqkhirzge.html

[Q83] 大小写转换
来源：http://hz.hywenlv.cn/gtmwmrfvhh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.iojbl.cn/gtmwltshyv.html

[Q84] 去除首尾空格
来源：http://hz.sxryk.cn/gtgxduxuig.html

SELECT TRIM(name) FROM users;
来源：http://hz.jlsjyb.cn/gtpladbhuq.html

[Q85] 数值取整
来源：http://hz.tanke756.top/gtrmmjqnit.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgfzy.top/gtdunrlsfa.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangkeji.top/gthudwhjbt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xinyue.icu/gtbwyxkics.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gtqdiriomo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangshuangyany.cn/gtrehddxpc.html

[Q88] 行转列（条件聚合）
来源：http://hz.cheryme.top/gtbdkrhhfy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gtastoupxz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.feifeiyinyue.top/gtboqwirae.html

[Q89] 判断表是否存在
来源：http://hz.chenzaomai.com/gtcpkkbzcp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.bjfxy.top/gtxwndhqam.html

[Q90] 生成序号列
来源：http://hz.yonumen.top/gtogkllqzw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gtqlvtskzi.html

================================================================================
来源：http://hz.xinyue.icu/gttoelwlkq.html

R. Bash 专题
来源：http://hz.jinqigufen.top/gtjtoffhil.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjgylqdxw.html

[R01] shebang 与严格模式
来源：http://hz.wangdashe.top/gtabligbto.html

#!/usr/bin/env bash
来源：http://hz.yj20258.top/gtmtqelxam.html

set -euo pipefail
来源：http://hz.cucudq.cn/gtubfymwjc.html

[R02] 变量赋值与使用
来源：http://hz.jlsjyb.cn/gtdrxwtazs.html

name="Tom"; echo "$name"
来源：http://hz.ppjwa.cn/gtwhtfpfne.html

[R03] 只读变量
来源：http://hz.shuidangran.top/gtejngluus.html

readonly PI=3.14
来源：http://hz.zhiwuduotai.top/gtmxywfhva.html

[R04] 位置参数
来源：http://hz.sufxvd.cn/gtgxrfdhyd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhengqikj.top/gtoivpyore.html

[R05] 参数默认值
来源：http://hz.fengsongda.top/gtshlfhmln.html

name="${1:-default}"
来源：http://hz.nanxinkj.top/gticrjvunn.html

[R06] 判断命令是否存在
来源：http://hz.chenzaomai.com/gtcmdfzjyy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yanxiufei.cn/gtxusldcie.html

[R07] if 判断文件
来源：http://hz.mhx1999.top/gtyruztpnb.html


<!-- 参考信息 -->