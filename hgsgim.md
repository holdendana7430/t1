代发 wailian999

[O06] 使用进程池
来源：http://hz.jianghu66.top/gtanbwfryj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jlsjyb.cn/gtgoosjcyb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydjk.org.cn/gtdboxxncu.html

JS:   // child_process / cluster 模块
来源：http://hz.sweek.top/gtrkqqvlal.html

TS:   // child_process / cluster 模块
来源：http://hz.jianghu66.top/gtmcapkxas.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xuanzx.com/gtxflrnwwq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.0kj1m.cn/gtakdvixmd.html

Ruby: // fork 块
来源：http://hz.yonumen.top/gtyhizigkl.html

C#:   Parallel.For
来源：http://hz.fzhhl.top/gtwnoekxul.html

================================================================================
来源：http://hz.cdnleiting.top/gtmchshsyr.html

P. 常用工具函数
来源：http://hz.xziqi.cn/gtivrmgsoo.html

================================================================================
来源：http://hz.sxryk.cn/gtikwudsic.html

[P01] 生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtuxxvkyoz.html

Py:   str(uuid.uuid4())
来源：http://hz.yuanzhike.top/gtdnqytgbh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxuanxn.top/gtypfdglsl.html

JS:   crypto.randomUUID()
来源：http://hz.nwbrower.top/gtdffophuw.html

TS:   crypto.randomUUID()
来源：http://hz.ybcxt.top/gtkwtgijnt.html

Java: UUID.randomUUID().toString()
来源：http://hz.yuxming.cn/gtmmgcsofs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yanxiufei.cn/gtlftpsedk.html

Ruby: SecureRandom.uuid
来源：http://hz.vqdsnc.cn/gtebststcl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.redwolf501.top/gtrzvbnkvv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ppjwa.cn/gtgmphqwpz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.quarkkingdee.top/gturntlutx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yvedp.cn/gtcvygoloy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.shanyushiyangkeji.top/gtpubhqwvz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yonumen.top/gtmcakoykm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yueranfly.top/gtfapysthj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.snrcjt.cn/gtjpmstubq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yuanzhike.top/gtacjtsigk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hysaishi.cn/gtvnltjhal.html

[P03] 生成短随机字符串
来源：http://hz.gogol.net.cn/gtggtgkaak.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.guannengcc.top/gtbivvvxfv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangkeji.top/gtvgaautng.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.316326.xyz/gteajyebld.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigufen.top/gtayazixjz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.redwolf501.top/gtqoyrgitf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cucudq.cn/gtziodefsg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.mhx1999.top/gtflvospbi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.pycfn.com/gtvapnjutq.html

[P04] 求长度
来源：http://hz.sweek.top/gtgeojbmts.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.316326.xyz/gtfdtlmtcm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtgzmauacj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yuanzhike.top/gticinejbi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtvdxcptkk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nanxinkj.top/gterfzjywd.html

Go:   len(arr);  len(m)
来源：http://hz.haohaochexian.top/gtrnlkcshu.html

Ruby: x.length;  x.size
来源：http://hz.hongshengwenyu.top/gtnwxulwbr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yuanzhike.top/gtdpksoyny.html

[P05] 判断两个对象内容是否相等
来源：http://hz.cucudq.cn/gtohlhlnqg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.yj20258.top/gtowfycyyg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtexrgbgff.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.svipenyu.cn/gtfpmkpitw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gzhubu.top/gtsszopjvw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigfzy.top/gtkjrtaebz.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.quarkkingdee.top/gtlhvegurs.html

Ruby: a == b
来源：http://hz.ybcxt.top/gtthzxkspu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.cashguo.top/gthcszcnuj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.chenlongwang.top/gtyerpuxhh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.yj20258888.top/gtrhvchlqs.html

PHP:  if (empty($x)) {}
来源：http://hz.shzxlz.cn/gtjidabfnw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hfpthk.cn/gtwocajmfa.html

TS:   if (x == null) {}
来源：http://hz.gogol.net.cn/gtlzbzxrxf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtxcgfinkl.html

Go:   if x == nil {}
来源：http://hz.ydjk.org.cn/gtmrylqtjz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.havefunace.top/gtoetjksyi.html

C#:   if (x is null) {}
来源：http://hz.jqgufenzy.top/gtyikiakll.html

[P07] 防抖与节流
来源：http://hz.snrcjt.cn/gtjdeytaub.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ivvv.top/gtojaaxbfr.html

PHP:  // 手写时间戳比较
来源：http://hz.vqdsnc.cn/gtjuewogpb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sysykeji.top/gtsrkjgkaz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jiagoushi.top/gtuqwkkqdt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.mhx1999.top/gtkuvhvxjl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.xylfe.cn/gtgdnwsuxk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.hnqzz.top/gtljsoavqp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.ybcxt.top/gtxvptfizv.html

[P08] 处理浮点精度问题
来源：http://hz.yj20258.top/gtuzpzotkf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yanxiufei.cn/gtoozjqinf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.snrcjt.cn/gtwkzmaxxb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hnqzz.top/gtshfpdmdv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.nanxinkj.top/gtngiusryf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.c1oappe.top/gtqhgykulg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.andypj.xyz/gtzugertkn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.sweek.top/gtzsjxtuvh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.birdmap.top/gtuauozvku.html

================================================================================
来源：http://hz.haohaochexian.top/gtauvwbacv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ywan-chungtsiang.top/gtomqrxkun.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbkjdxjgn.html

[Q01] 创建表
来源：http://hz.sxryk.cn/gtqrznysvu.html

CREATE TABLE users (
来源：http://hz.fzhhl.top/gtqaqzmtxe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.zhongyouzk.top/gtbtzipyvk.html

name VARCHAR(50) NOT NULL,
来源：http://hz.shzxlz.cn/gtrxblloyo.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gaohongyu789.top/gtqdtmsgft.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinqigufen.top/gtnwedykqd.html

);
来源：http://hz.haohaochexian.top/gtlcvzlnca.html

[Q02] 创建带外键的表
来源：http://hz.yuanzhike.top/gtkcsnivqk.html

CREATE TABLE orders (
来源：http://hz.wangdashe.top/gtxspsljvv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.52xcode.cn/gtuzmzzyqn.html

user_id INT NOT NULL,
来源：http://hz.zhoulong.xyz/gtxitwttjb.html

amount DECIMAL(10, 2),
来源：http://hz.yj20258888.top/gtubwnmzap.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.aibaodan.cn/gtsbyipltu.html

);
来源：http://hz.shuidangran.top/gtfolxfrer.html

[Q03] 增加列
来源：http://hz.zycfv.cn/gtvbmptszl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenlongwang.top/gtficsyoxw.html

[Q04] 修改列类型
来源：http://hz.pengpengdd.cyou/gtnwznsypw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.vqdsnc.cn/gtvzvnlbgu.html

[Q05] 重命名列
来源：http://hz.shanyushiyangkeji.top/gtxslietzx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ybcxt.top/gtiwsiccpf.html

[Q06] 删除列
来源：http://hz.zhijiandao.cn/gtzosiqjrb.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.ybcxt.top/gtnawrrafb.html

[Q07] 删除表
来源：http://hz.jlsjyb.cn/gtociqaapc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhongyouzk.top/gtafxavujd.html

[Q08] 创建普通索引
来源：http://hz.pengpengdd.cyou/gtmreerdse.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtxtvcfgms.html

[Q09] 创建唯一索引
来源：http://hz.jinqigufen.top/gtvmxyhavx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtwytjdrwt.html

[Q10] 插入单行
来源：http://hz.jqgufenzy.top/gtttuohzdw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.meibo888.top/gttnjexpwt.html

[Q11] 一次插入多行
来源：http://hz.yj202588.top/gtoeuqbtod.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhaomingkeji.xyz/gtrohnasyc.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangkeji.top/gtlqeksofj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hammf.cn/gtbcxzpfuc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.guannengcc.top/gtpqgngotz.html

[Q13] 忽略重复插入
来源：http://hz.ydzc1.top/gtuyxkkbba.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ybcxt.top/gtqvsqxjei.html

[Q14] 存在则更新（upsert）
来源：http://hz.svipenyu.cn/gtsveroiig.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhijiandao.cn/gtnajvhjxn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ivvv.top/gtdailijtd.html

[Q15] 查询全部
来源：http://hz.gogol.net.cn/gtqresizcv.html

SELECT * FROM users;
来源：http://hz.snrcjt.cn/gtpkizqfby.html

[Q16] 查询指定列
来源：http://hz.jqgufenzy.top/gtysiiilih.html

SELECT id, name FROM users;
来源：http://hz.jyoumei.cn/gtanweaben.html

[Q17] 条件查询
来源：http://hz.wangdashe.top/gtnchjztzr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xziqi.cn/gtydhcunqk.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gthsvpnomc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydzc1.top/gtdzljwcqp.html

[Q19] 范围查询
来源：http://hz.tanke756.top/gtyrexkyyv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.xziqi.cn/gtzwmkjngw.html

[Q20] IN 列表
来源：http://hz.chenjidiqi.icu/gtwqddvqva.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.chenjidiqi.icu/gtauzpcswz.html

[Q21] 空值判断
来源：http://hz.xinyue.icu/gtzmmrvxbr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.snrcjt.cn/gttftrkfci.html

[Q22] 排序
来源：http://hz.zhoulong.xyz/gtnvzlfgcr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gtkghbukkn.html

[Q23] 分页
来源：http://hz.jinghuilouyu.cn/gtmwplnvlq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cdnleiting.top/gtnzlbpudk.html

[Q24] 去重
来源：http://hz.xingfuxueyuan.xyz/gttnftwqzc.html

SELECT DISTINCT city FROM users;
来源：http://hz.shuidangran.top/gtmcdqcrqq.html

[Q25] 只取前 N 条
来源：http://hz.sysykeji.top/gtrbmfaufn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigufen.top/gtpixkhosu.html

[Q26] 计数
来源：http://hz.zhengqikj.top/gtjgcjwkfb.html

SELECT COUNT(*) FROM users;
来源：http://hz.yuxming.cn/gtrqkvuqay.html

[Q27] 条件计数
来源：http://hz.gaohongyu789.top/gtmwakrqar.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.tianlin.xyz/gthazatzqp.html

[Q28] 求和与平均
来源：http://hz.yj20258888.top/gtokzqgwiz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gtvattrrml.html

[Q29] 最大最小值
来源：http://hz.yueranfly.top/gtifcblvmh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhongyouzk.top/gtkcrvykkk.html

[Q30] 分组统计
来源：http://hz.hnqzz.top/gtazscpwye.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydzc1.top/gttrsjlxmx.html

[Q31] 分组后过滤
来源：http://hz.jianghu66.top/gtseufokzw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sysykeji.top/gtezzvkgtb.html

[Q32] 分组拼接字符串
来源：http://hz.cdnleiting.top/gtpfhcmpdk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtyplmhqvp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuanzhike.top/gtvoalumco.html

[Q33] 多列分组
来源：http://hz.tian-w.cn/gtfazrwgpx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zhixingplan.top/gthzmehmtv.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtaextyvfd.html

SELECT * FROM (
来源：http://hz.0kj1m.cn/gtewnsrjcp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yuxming.cn/gtbntemiwc.html

) t WHERE rn = 1;
来源：http://hz.fengsongda.top/gtcafsggxm.html

[Q35] 内连接
来源：http://hz.yonumen.top/gttnvzbrmw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.quarkkingdee.top/gtvkwvybyn.html

[Q36] 左连接
来源：http://hz.wangshuangyany.cn/gtkjkgrhyj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sweek.top/gtwueasosh.html

[Q37] 右连接
来源：http://hz.hnqzz.top/gtkonbdixk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangdashe.top/gtuyvzibns.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cdnleiting.top/gtkmbtcaoc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtkyavvtwv.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtaazuplvi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.smart0.xyz/gtjisuwqkh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xziqi.cn/gtiafapuhn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nwbrower.top/gtqnlzwrkb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yvedp.cn/gtxxnhuzme.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtttmfohkz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtmvzvlphv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ybcxt.top/gtbjlsxrex.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yueranfly.top/gtwdvclopp.html

[Q42] 连接条件附加过滤
来源：http://hz.pengpengdd.cyou/gtxhdscelo.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gogol.net.cn/gtzvzdxsem.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zhongyouzk.top/gtwutwssmf.html

[Q43] 标量子查询
来源：http://hz.ivvv.top/gtivcwhvjz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtmrnljubr.html

[Q44] IN 子查询
来源：http://hz.gogol.net.cn/gtykbmrvkf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.meibo888.top/gtsyficqnq.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtayusiijd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhixingplan.top/gtujjefghh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gtfbgwuqoj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.iojbl.cn/gtmabzbxqg.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtvkngbvit.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.316326.xyz/gtmvorbemh.html

[Q48] CTE 公用表表达式
来源：http://hz.jianghu66.top/gtczbestgt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtvvtfrmjf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.sxryk.cn/gtlogimtzo.html

[Q49] 更新单行
来源：http://hz.yj202588.top/gttzskupgj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.meibo888.top/gtkdhzvjdg.html

[Q50] 批量更新
来源：http://hz.chenzaomai.com/gtnjstsapq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.52xcode.cn/gtzcqbzcvn.html

[Q51] 用子查询更新
来源：http://hz.aibaodan.cn/gtnskrbhtv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenjidiqi.icu/gtckhqhrna.html

[Q52] 删除指定行
来源：http://hz.cucudq.cn/gtpgndrdcn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.haohaochexian.top/gtrxdhzfvl.html

[Q53] 按条件删除
来源：http://hz.yuxming.cn/gtwlrsabxn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xingfuxueyuan.xyz/gtceitmifu.html

[Q54] 清空表
来源：http://hz.316326.xyz/gtmonhocfc.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigufen.top/gtflsnwcjq.html

[Q55] 排名（并列占位）
来源：http://hz.xinyue.icu/gtnklqvjgs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.snrcjt.cn/gtfgfkjoet.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhaomingkeji.xyz/gtkzoalqam.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gtqddiankx.html

[Q57] 行号
来源：http://hz.0kj1m.cn/gtdedtzlrq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhixingplan.top/gtfpoxetlo.html

[Q58] 累计求和
来源：http://hz.guowangkeji.top/gttkovklsb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenzaomai.com/gteundkown.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtkfgvipco.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtchmplxjy.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gthipobrtd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydzc1.top/gtzssjcbau.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258.top/gtpbknwpbg.html

[Q61] 移动平均
来源：http://hz.zhengqikj.top/gtnbbrwqxu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtzbtolctz.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gtsgyvcdcl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtomxjpigk.html

[Q63] 开启事务
来源：http://hz.xylfe.cn/gtxjrebqmo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.gaohongyu789.top/gtrrpnkvze.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gtjskhscpn.html

COMMIT;
来源：http://hz.chenjidiqi.icu/gtmodnvzoj.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gttnddqger.html

ROLLBACK;
来源：http://hz.gaohongyu789.top/gtmjpmjxcr.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtbexaaaqu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gtzmcwbvhp.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtkvuytarx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtbrqyotie.html

[Q68] 保存点
来源：http://hz.cashguo.top/gtnpydrwgd.html

SAVEPOINT sp1;
来源：http://hz.jianghu66.top/gtvemqdpte.html

ROLLBACK TO sp1;
来源：http://hz.ivvv.top/gtycvrcbvd.html

[Q69] 查看执行计划
来源：http://hz.xuanzx.com/gtzrpyyyed.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nwbrower.top/gthsqfbtco.html

[Q70] 更新统计信息
来源：http://hz.ehwqpu.com/gtkueilzll.html

ANALYZE TABLE users;
来源：http://hz.guannengcc.top/gtpvppapgn.html

[Q71] 查看建表语句
来源：http://hz.gzhubu.top/gtlopkblob.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.andypj.xyz/gtwpzhxkoc.html

[Q72] 查看索引
来源：http://hz.andypj.xyz/gtgjnoycht.html

SHOW INDEX FROM users;
来源：http://hz.chenzaomai.com/gtylqcsqjw.html

[Q73] 查看表状态
来源：http://hz.iojbl.cn/gttuvqkzac.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtjxwrfjeg.html

[Q74] 强制使用索引
来源：http://hz.hnxiangtu.top/gtdacmhjfy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinghuilouyu.cn/gtfhcjynoa.html

[Q75] 日期格式化
来源：http://hz.cucudq.cn/gtjlivovju.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhijiandao.cn/gtuhgtivgu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtfxqoblbe.html

[Q76] 按天统计
来源：http://hz.kuanghao11.cn/gtdwngmakg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ybcxt.top/gtkpyotwls.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtiqqlkwta.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.52xcode.cn/gtafapjjsb.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gtkbmwxpzp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xziqi.cn/gtwilmitgk.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtqvablami.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yanxiufei.cn/gtoqxqrmdc.html

[Q80] 字符串截取
来源：http://hz.aizwys.cn/gtionfnlkr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhongyouzk.top/gtqoaohjrx.html

[Q81] 字符串替换
来源：http://hz.52xcode.cn/gtsftdwkml.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tian-w.cn/gthnwtnvhv.html

[Q82] 字符长度与字节长度
来源：http://hz.0kj1m.cn/gtdydhqgvz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtpucvylvj.html

[Q83] 大小写转换
来源：http://hz.gaohongyu789.top/gtowawhweu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cqqwz.cn/gtpdpkzvxm.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtjstaiaok.html

SELECT TRIM(name) FROM users;
来源：http://hz.gogol.net.cn/gtefutimxb.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtpmepxpkq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aizwys.cn/gtggfvgvln.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtwgiyvlny.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtdopxyixd.html

[Q87] JSON 字段做条件
来源：http://hz.xuetiantiany.cn/gtjqngayoc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.wangdashe.top/gtbyoiraqx.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtsgedykze.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xylfe.cn/gttnfeltut.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtddwiyujy.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtzffjxnlr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.meibo888.top/gtjaengext.html

[Q90] 生成序号列
来源：http://hz.tian-w.cn/gtfpnlgwik.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yuanzhike.top/gtklrpaocu.html

================================================================================
来源：http://hz.yj20258.top/gttnrogqah.html

R. Bash 专题
来源：http://hz.nanxinkj.top/gtjnzbntpa.html

================================================================================
来源：http://hz.andypj.xyz/gtvfbgphqy.html

[R01] shebang 与严格模式
来源：http://hz.hfpthk.cn/gtqrsiltls.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtmduwnrqv.html

set -euo pipefail
来源：http://hz.daxiang520.top/gtlfyhkkpy.html

[R02] 变量赋值与使用
来源：http://hz.hysaishi.cn/gtywwechjh.html

name="Tom"; echo "$name"
来源：http://hz.dashuyun.cn/gtxxcowujd.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtiqxjdtsq.html


<!-- 参考信息 -->