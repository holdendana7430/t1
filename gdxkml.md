代发 wailian999

TS:   // child_process / cluster 模块
来源：http://hz.dianchejie.cn/gtmarlscav.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gtjnvzrssc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangdashe.top/gtmwxqtmwm.html

Ruby: // fork 块
来源：http://hz.ppjwa.cn/gtfkexsiqk.html

C#:   Parallel.For
来源：http://hz.yongpay.top/gthegcwvcc.html

================================================================================
来源：http://hz.cdnleiting.top/gttgmcbgkk.html

P. 常用工具函数
来源：http://hz.tanke756.top/gtgiqefhvl.html

================================================================================
来源：http://hz.jyoumei.cn/gtzsdzgpqn.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangtech.top/gtdzncbrwp.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtaoakdvfn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ppjwa.cn/gtdknwtnjj.html

JS:   crypto.randomUUID()
来源：http://hz.cashguo.top/gtesnbounh.html

TS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtkcfbtjac.html

Java: UUID.randomUUID().toString()
来源：http://hz.mhx1999.top/gtacbknopf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zycfv.cn/gtdrmjvuju.html

Ruby: SecureRandom.uuid
来源：http://hz.svipenyu.cn/gtfpccreut.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.vqdsnc.cn/gtmekhbedg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jiagoushi.top/gtbpilnasf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.quarkkingdee.top/gtgoswpdrm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.haohaochexian.top/gtmwxziucd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.smart0.xyz/gtasysxoyg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhiwuduotai.top/gtkdeloyau.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinqigfzy.top/gthisxlkpf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj202588.top/gtjupufvmw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jlsjyb.cn/gtgunfaxwb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jqgfzy.top/gtbmmyjqme.html

[P03] 生成短随机字符串
来源：http://hz.hnxiangtu.top/gtjuuzorid.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.tianlin.xyz/gtjhuibjbu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.sysykeji.top/gtldlgrrya.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.aibaodan.cn/gtpiapgyzt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhaomingkeji.xyz/gttrgoynkz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yj20258888.top/gtvozfeens.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.guannengcc.top/gtjvpybeww.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuxming.cn/gtddjistjv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.zhoulong.xyz/gtytjrclwg.html

[P04] 求长度
来源：http://hz.wangshuangyany.cn/gtlloexarz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.vqdsnc.cn/gtrickgvyu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtpuprmjhr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtwqwqhpbt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangkeji.top/gtgepqshnd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.yanxiufei.cn/gtovzukcgq.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtzkzijxrm.html

Ruby: x.length;  x.size
来源：http://hz.zhiwuduotai.top/gthmwoxjti.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.quarkkingdee.top/gtzjorkrgc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.snrcjt.cn/gtgsxmouex.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.0kj1m.cn/gtkyutsjnj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.meibo888.top/gtqzvngpgq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dashuyun.cn/gttfqlrtmg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yanxiufei.cn/gtkorvnqpq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.havefunace.top/gtfhjsifyn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aibaodan.cn/gtfurxvfol.html

Ruby: a == b
来源：http://hz.smart0.xyz/gtmvjxmeys.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.kuanghao11.cn/gtuwcrtzqc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhaomingkeji.xyz/gtwbyckwqi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.chenzaomai.com/gtsgezfdfu.html

PHP:  if (empty($x)) {}
来源：http://hz.chenjidiqi.icu/gtjccroogn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.bjfxy.top/gtogyzwwgw.html

TS:   if (x == null) {}
来源：http://hz.shanyushiyangkeji.top/gthqykfzcz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.redwolf501.top/gtlxwjdhcp.html

Go:   if x == nil {}
来源：http://hz.ydzc1.top/gtwpowyrse.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jyoumei.cn/gtxnhogves.html

C#:   if (x is null) {}
来源：http://hz.52xcode.cn/gtdysnpjsb.html

[P07] 防抖与节流
来源：http://hz.andypj.xyz/gtwrarpytl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.0kj1m.cn/gtduyjkszj.html

PHP:  // 手写时间戳比较
来源：http://hz.yangfankeji.com/gtkeyqiatp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtskwaqsnv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtfongezed.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.andypj.xyz/gtyiajdurx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yanxiufei.cn/gtjibtjnrk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yueranfly.top/gtgkmaewzl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhaomingkeji.xyz/gtkftpolhy.html

[P08] 处理浮点精度问题
来源：http://hz.iojbl.cn/gtlmvpqlmp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.xziqi.cn/gtwumgtbda.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ybcxt.top/gtjziiotma.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.wangshuangyany.cn/gtrtgywkzc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.quarkkingdee.top/gtjqdlqkvp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ybcxt.top/gtebcrlssb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.sufxvd.cn/gtertikyun.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.gogol.net.cn/gtyqzvsaoy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gtpoqyhvid.html

================================================================================
来源：http://hz.tian-w.cn/gtekdoyyrx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yangfankeji.com/gtiqgbfwoe.html

================================================================================
来源：http://hz.gzhubu.top/gtdhubskdy.html

[Q01] 创建表
来源：http://hz.aizwys.cn/gtfpuakvxo.html

CREATE TABLE users (
来源：http://hz.xuanzx.com/gtbhgaflxx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtuaaamxzf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.svipenyu.cn/gtfylqaiyy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.tanke756.top/gtisynzvns.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.chenjidiqi.icu/gtupoqwffh.html

);
来源：http://hz.zhixingplan.top/gtwhxdrksm.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtzazzwlvd.html

CREATE TABLE orders (
来源：http://hz.jlsjyb.cn/gtghbdodwf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.chenjidiqi.icu/gtukgrlnws.html

user_id INT NOT NULL,
来源：http://hz.jinghuilouyu.cn/gtgslpohnt.html

amount DECIMAL(10, 2),
来源：http://hz.hysaishi.cn/gtminccvad.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.feifeiyinyue.top/gttagxfjax.html

);
来源：http://hz.fzhhl.top/gtperubcym.html

[Q03] 增加列
来源：http://hz.yueranfly.top/gtssoeatvd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.meibo888.top/gtruiwudid.html

[Q04] 修改列类型
来源：http://hz.chenjidiqi.icu/gtwdbdzdyn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hysaishi.cn/gtdiyxvtit.html

[Q05] 重命名列
来源：http://hz.hysaishi.cn/gtkmjexxfg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.gotoacloud.top/gtoapgtbep.html

[Q06] 删除列
来源：http://hz.hnxiangtu.top/gtwsqsucng.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.dashuyun.cn/gtofgpnqbu.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtadavytfm.html

DROP TABLE IF EXISTS orders;
来源：http://hz.chenjidiqi.icu/gtnfcltoqc.html

[Q08] 创建普通索引
来源：http://hz.chenlongwang.top/gtmytbikhl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtxwucqtma.html

[Q09] 创建唯一索引
来源：http://hz.yj202588.top/gtbiarwmtj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xuetiantiany.cn/gtwwnckapq.html

[Q10] 插入单行
来源：http://hz.hnqzz.top/gtqtzdosot.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zycfv.cn/gtillpklly.html

[Q11] 一次插入多行
来源：http://hz.aizwys.cn/gtafgxnxhr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.yj20258.top/gtvwuuxnfe.html

[Q12] 插入后取自增 ID
来源：http://hz.wangshuangyany.cn/gtdfqzhggv.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nanxuanxn.top/gtxcmutodr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.meibo888.top/gtfjbcnzkl.html

[Q13] 忽略重复插入
来源：http://hz.hongshengwenyu.top/gtleevllrc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.quarkkingdee.top/gtkcdxrshb.html

[Q14] 存在则更新（upsert）
来源：http://hz.xuetiantiany.cn/gtoypmbvri.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.shanyushiyangkeji.top/gtmmvnyjpb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhongyouzk.top/gtrosgiedw.html

[Q15] 查询全部
来源：http://hz.shuidangran.top/gttmikbbrq.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtegqcpfav.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gtaoouaayi.html

SELECT id, name FROM users;
来源：http://hz.tanke756.top/gtegvyqiop.html

[Q17] 条件查询
来源：http://hz.c1oappe.top/gtchuqobli.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.vqdsnc.cn/gtgliifdgb.html

[Q18] 模糊匹配
来源：http://hz.sysykeji.top/gtpxqiijqx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nanxuanxn.top/gtitnbxfsp.html

[Q19] 范围查询
来源：http://hz.vqdsnc.cn/gttienagmc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yangfankeji.com/gtrqzzormn.html

[Q20] IN 列表
来源：http://hz.jiagoushi.top/gtzfeirmmc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ydjk.org.cn/gtafcwhcby.html

[Q21] 空值判断
来源：http://hz.snrcjt.cn/gtzumblrhq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.xziqi.cn/gtvywuxujx.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtswoxrnzn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jianghu66.top/gttxkbzklp.html

[Q23] 分页
来源：http://hz.hammf.cn/gtxywofhyp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ydzc1.top/gtaqngwbbk.html

[Q24] 去重
来源：http://hz.mhx1999.top/gthdyhhfvk.html

SELECT DISTINCT city FROM users;
来源：http://hz.daria6918.cn/gtcppibdls.html

[Q25] 只取前 N 条
来源：http://hz.shuidangran.top/gtuiaqdjri.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj202588.top/gtvomdqdru.html

[Q26] 计数
来源：http://hz.daxiang520.top/gtfdaslnfy.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtewynajbv.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gtnfpolfip.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.iojbl.cn/gtlevvurdv.html

[Q28] 求和与平均
来源：http://hz.guannengcc.top/gtnubltjxq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.wangdashe.top/gtokohsmee.html

[Q29] 最大最小值
来源：http://hz.jlsjyb.cn/gtgyxfqzbz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hnqzz.top/gtejobnajg.html

[Q30] 分组统计
来源：http://hz.yonumen.top/gtqnvtvovd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtifzvppzt.html

[Q31] 分组后过滤
来源：http://hz.xingfuxueyuan.xyz/gtoejuydoz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.wangshuangyany.cn/gtrwonmygg.html

[Q32] 分组拼接字符串
来源：http://hz.zycfv.cn/gterjpfxpz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtwbqygfjj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.chenjidiqi.icu/gtoiyfzkch.html

[Q33] 多列分组
来源：http://hz.c1oappe.top/gtjzaurlgb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.sysykeji.top/gtqgkerfmx.html

[Q34] 每组取第一条
来源：http://hz.fzhhl.top/gtzzbuuvsf.html

SELECT * FROM (
来源：http://hz.bjfxy.top/gtjuretvhr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.fzhhl.top/gtuhgeilly.html

) t WHERE rn = 1;
来源：http://hz.pycfn.com/gtzremzgqz.html

[Q35] 内连接
来源：http://hz.yuxming.cn/gtgjpgojze.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.bjfxy.top/gtfxzatrtk.html

[Q36] 左连接
来源：http://hz.dashuyun.cn/gtjygcbdbm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258888.top/gtreklzkvs.html

[Q37] 右连接
来源：http://hz.mhx1999.top/gtjsdptryd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cheryme.top/gtktotmbbi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ehwqpu.com/gtyghmngve.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shanyushiyangtech.top/gtkrmnegsv.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gtcbzaznyv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jianghu66.top/gtklfumhok.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ydzc1.top/gtutzjzjwm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jqgufenzy.top/gtdihyhrfs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shzxlz.cn/gtoigfkjjy.html

[Q41] 多表连接
来源：http://hz.quarkkingdee.top/gtblluynpy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gtsmcfivip.html

JOIN users u ON u.id = o.user_id
来源：http://hz.0kj1m.cn/gtvdcsorwl.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.kuanghao11.cn/gtjkvmokil.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gttlbpotzt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.feifeiyinyue.top/gtkvyuhevp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fengsongda.top/gttedrzply.html

[Q43] 标量子查询
来源：http://hz.smart0.xyz/gtvngxrlzk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.snrcjt.cn/gtvxzzafrb.html

[Q44] IN 子查询
来源：http://hz.dianchejie.cn/gtzpfnulcg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.cheryme.top/gtiyqzstlp.html

[Q45] EXISTS 判断存在
来源：http://hz.chenlongwang.top/gtnyrjlezr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtuzdplttz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xingfuxueyuan.xyz/gtatopzvsv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtonbvenxj.html

[Q47] 与平均值比较
来源：http://hz.nanxinkj.top/gtsluhainw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtbwfnjror.html

[Q48] CTE 公用表表达式
来源：http://hz.wangdashe.top/gtuqwllxym.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.52xcode.cn/gtfllphzks.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cheryme.top/gtnhstwknz.html

[Q49] 更新单行
来源：http://hz.gaohongyu789.top/gtsbmfxosf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xingfuxueyuan.xyz/gtngyjfxeb.html

[Q50] 批量更新
来源：http://hz.dianchejie.cn/gttjxjbjfi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.c1oappe.top/gtqcjtxsjs.html

[Q51] 用子查询更新
来源：http://hz.zhaomingkeji.xyz/gtjfgpadki.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtjckaupcx.html

[Q52] 删除指定行
来源：http://hz.shuidangran.top/gtnikmgcas.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydzc1.top/gtkkyjuvxm.html

[Q53] 按条件删除
来源：http://hz.sxryk.cn/gtjtfqcutw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhengqikj.top/gtttbvdvag.html

[Q54] 清空表
来源：http://hz.cheryme.top/gtnevazvtp.html

TRUNCATE TABLE logs;
来源：http://hz.shanyushiyangkeji.top/gtiadhetfz.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtkguvtwxj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.aizwys.cn/gtngbwxewi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuetiantiany.cn/gtqirnusls.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtoomhkrve.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gtwiaqhdrt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.9152youxi.cn/gtahqigejf.html

[Q58] 累计求和
来源：http://hz.ehwqpu.com/gtouuialqf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cashguo.top/gtdzugtgco.html

[Q59] 分组内累计
来源：http://hz.ppjwa.cn/gtvnkajxhg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.dianchejie.cn/gtcehnrydk.html

[Q60] 取上一行 / 下一行
来源：http://hz.316326.xyz/gtvgbirbun.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.meibo888.top/gtwgomhugz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.52xcode.cn/gtcacsmbkk.html

[Q61] 移动平均
来源：http://hz.nwbrower.top/gtwmfqxqib.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.birdmap.top/gtzsedjuqt.html

[Q62] 分组占比
来源：http://hz.tian-w.cn/gthagdalga.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.316326.xyz/gttxxjwlef.html

[Q63] 开启事务
来源：http://hz.sweek.top/gtxcmjjfhw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xylfe.cn/gtzmgajtuw.html

[Q64] 提交事务
来源：http://hz.dashuyun.cn/gtciianucm.html

COMMIT;
来源：http://hz.yangfankeji.com/gtgwsnayiu.html

[Q65] 回滚事务
来源：http://hz.yonumen.top/gtnaohcwxu.html

ROLLBACK;
来源：http://hz.aizwys.cn/gtsqqubbcr.html

[Q66] 行锁查询
来源：http://hz.gotoacloud.top/gtbeyzwgxl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj202588.top/gtuuhaxwiy.html

[Q67] 设置隔离级别
来源：http://hz.jyoumei.cn/gtxukoixgn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jiagoushi.top/gtiffilvso.html

[Q68] 保存点
来源：http://hz.zhaomingkeji.xyz/gtagafnoiu.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtabjwdzvm.html

ROLLBACK TO sp1;
来源：http://hz.zhaomingkeji.xyz/gtholimbfd.html

[Q69] 查看执行计划
来源：http://hz.jyoumei.cn/gtoyqunrik.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtfbtmqost.html

[Q70] 更新统计信息
来源：http://hz.zycfv.cn/gtxcllchbn.html

ANALYZE TABLE users;
来源：http://hz.bjfxy.top/gtsirxaqih.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangtech.top/gtmqfihnkn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yuanzhike.top/gtdxbkfjea.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gtjfxfdjtw.html

SHOW INDEX FROM users;
来源：http://hz.tian-w.cn/gtzfhpuupr.html

[Q73] 查看表状态
来源：http://hz.ehwqpu.com/gtofpibjnq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.snrcjt.cn/gtyuwhlrrb.html

[Q74] 强制使用索引
来源：http://hz.sufxvd.cn/gtcapwqlzj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.sufxvd.cn/gtwakkiygg.html

[Q75] 日期格式化
来源：http://hz.yj202588.top/gtqlkacgpi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.52xcode.cn/gtnreylocf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj202588.top/gtpwllshwy.html

[Q76] 按天统计
来源：http://hz.xuanzx.com/gtqafvxodl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xziqi.cn/gtjpjssknw.html

[Q77] 时间加减
来源：http://hz.cucudq.cn/gtgeagresi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gtsknzpmue.html

[Q78] 当前时间
来源：http://hz.cashguo.top/gtsbioseum.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.316326.xyz/gtlvexsxqj.html

[Q79] 字符串拼接
来源：http://hz.vqdsnc.cn/gtuxkjvzsf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhoulong.xyz/gtunxpgxra.html

[Q80] 字符串截取
来源：http://hz.kuanghao11.cn/gtwytvforv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtqgeqifkj.html

[Q81] 字符串替换
来源：http://hz.ivvv.top/gtflgllejz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.c1oappe.top/gtmosrjies.html

[Q82] 字符长度与字节长度
来源：http://hz.ybcxt.top/gtwvqwfndx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtbpejszut.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtxdsnyzhh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtpptccrjo.html

[Q84] 去除首尾空格
来源：http://hz.ppjwa.cn/gtasfhliog.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtmcjdsyvf.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtkkflatrn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangtech.top/gtawklbwhh.html

[Q86] 读取 JSON 字段
来源：http://hz.mhx1999.top/gtjvqtuyce.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sufxvd.cn/gtbqqcrusl.html

[Q87] JSON 字段做条件
来源：http://hz.ivvv.top/gtndlfopge.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sysykeji.top/gtnfkbndoy.html

[Q88] 行转列（条件聚合）
来源：http://hz.cashguo.top/gttvfukevt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sxryk.cn/gtfnaxlcvm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nwbrower.top/gtekrgwvhx.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtpnvumlit.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.vqdsnc.cn/gtdntnnwix.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtrpmjgphz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shangyingyoupin.top/gtdsdlrple.html

================================================================================
来源：http://hz.chenzaomai.com/gtylffeeed.html

R. Bash 专题
来源：http://hz.yuxming.cn/gtprxkxmac.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtmpcntyvy.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtsrohlcvu.html

#!/usr/bin/env bash
来源：http://hz.svipenyu.cn/gtqbcpkzcf.html

set -euo pipefail
来源：http://hz.meibo888.top/gtrwqfzfen.html

[R02] 变量赋值与使用
来源：http://hz.ydjk.org.cn/gtyralettc.html

name="Tom"; echo "$name"
来源：http://hz.cqqwz.cn/gteivtbrlz.html

[R03] 只读变量
来源：http://hz.9152youxi.cn/gtovccwmpk.html

readonly PI=3.14
来源：http://hz.cashguo.top/gtkiblzwvk.html

[R04] 位置参数
来源：http://hz.xziqi.cn/gtyqgtyqkd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sweek.top/gtsxwdxant.html

[R05] 参数默认值
来源：http://hz.zhongyouzk.top/gtqxyajlsg.html


<!-- 参考信息 -->