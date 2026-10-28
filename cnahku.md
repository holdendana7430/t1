代发 wailian999

[O06] 使用进程池
来源：http://hz.wangdashe.top/gtqbbnwxly.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.bjfxy.top/gtpwjgekxu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuanzx.com/gtneojhkcw.html

JS:   // child_process / cluster 模块
来源：http://hz.zdqjudy.top/gtobvdanfn.html

TS:   // child_process / cluster 模块
来源：http://hz.jiagoushi.top/gtfzfwdfgx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gogol.net.cn/gtowsqsben.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinyuanbaomall.cn/gtixxapows.html

Ruby: // fork 块
来源：http://hz.jinqigfzy.top/gtvcftikqk.html

C#:   Parallel.For
来源：http://hz.snrcjt.cn/gtqrpcddzh.html

================================================================================
来源：http://hz.9152youxi.cn/gtpcouzlay.html

P. 常用工具函数
来源：http://hz.nanxinkj.top/gtdfzytzbw.html

================================================================================
来源：http://hz.yuxming.cn/gtdkgqepwv.html

[P01] 生成 UUID
来源：http://hz.yueranfly.top/gtikypnywr.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtessdksnr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.nanxinkj.top/gtdyxhkbbt.html

JS:   crypto.randomUUID()
来源：http://hz.andypj.xyz/gtmzpfqmuu.html

TS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gtrsqkskww.html

Java: UUID.randomUUID().toString()
来源：http://hz.sysykeji.top/gtiwyoktrt.html

Go:   // 用 github.com/google/uuid
来源：http://hz.cheryme.top/gtksllpgej.html

Ruby: SecureRandom.uuid
来源：http://hz.guannengcc.top/gtaseyhthx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.daria6918.cn/gtapzfcazf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtqgfruact.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.sweek.top/gtjnbsnktx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgfzy.top/gtcqpheieb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ydzc1.top/gtispbgadt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.fengsongda.top/gtkbhizwae.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sufxvd.cn/gtnybfqvqe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aizwys.cn/gtzhjqwpec.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cashguo.top/gtidleuwsc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ywan-chungtsiang.top/gtwveolxfl.html

[P03] 生成短随机字符串
来源：http://hz.ydzc1.top/gtroojtgbe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangkeji.top/gtgxuetiwk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.haohaochexian.top/gtrtxrwehj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tianlin.xyz/gteuvohwtt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtysmpibgy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.aibaodan.cn/gttuqcwjmp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.316326.xyz/gtejakqenc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuanzx.com/gtcmcgoxnf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jiagoushi.top/gtnuhteycs.html

[P04] 求长度
来源：http://hz.ehwqpu.com/gtrecrqqng.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.dashuyun.cn/gtzieknsqr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gttoumnvwj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtudjdqrmr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yueranfly.top/gtelpsweir.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sufxvd.cn/gtpuanzktk.html

Go:   len(arr);  len(m)
来源：http://hz.jiagoushi.top/gtmpwgdqvv.html

Ruby: x.length;  x.size
来源：http://hz.xylfe.cn/gtkclgctfe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cqqwz.cn/gtthrgduri.html

[P05] 判断两个对象内容是否相等
来源：http://hz.havefunace.top/gtaxhvbtzk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.pengpengdd.cyou/gtxtqzqmrl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhoulong.xyz/gtmwfevoxf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.316326.xyz/gtcwrqidhr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhengqikj.top/gtyqzzcssu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhaomingkeji.xyz/gtyfnjgdbk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuanzhike.top/gtldjkvzyp.html

Ruby: a == b
来源：http://hz.vqdsnc.cn/gtdnvktwgj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtujuochsf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.wangdashe.top/gtkmvecphi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.birdmap.top/gtpkihbihu.html

PHP:  if (empty($x)) {}
来源：http://hz.shanyushiyangkeji.top/gtjhdccpku.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtcnfkavvd.html

TS:   if (x == null) {}
来源：http://hz.chenzaomai.com/gtwwsksxvn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.zdqjudy.top/gttwmkvrni.html

Go:   if x == nil {}
来源：http://hz.pengpengdd.cyou/gtxxnqieev.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.cheryme.top/gtsassgcnr.html

C#:   if (x is null) {}
来源：http://hz.wangdashe.top/gttmisbqcx.html

[P07] 防抖与节流
来源：http://hz.yuxming.cn/gtqoqturmn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yj20258.top/gtqjhevxal.html

PHP:  // 手写时间戳比较
来源：http://hz.jqgfzy.top/gtujmbbvxd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtabtveowp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gthtnqkeap.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ivvv.top/gtffmnrtiy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.shanyushiyangkeji.top/gtbaaqufim.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.andypj.xyz/gtalnquxks.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.sysykeji.top/gtbqtiwlpq.html

[P08] 处理浮点精度问题
来源：http://hz.zdqjudy.top/gtlwmmljjv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.mhx1999.top/gtpafjlaos.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.mhx1999.top/gtgmcnhmpg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.hywenlv.cn/gtlcdtwtoh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtssgfabwg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj202588.top/gtoiywyeaa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.ybcxt.top/gtdyhcsmwk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aibaodan.cn/gtcdrbzsgq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yueranfly.top/gtmzklewtt.html

================================================================================
来源：http://hz.jlsjyb.cn/gtrcaadqrf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.shuidangran.top/gtutmvxizv.html

================================================================================
来源：http://hz.hammf.cn/gtwqizutcj.html

[Q01] 创建表
来源：http://hz.chenjidiqi.icu/gtzuakoffn.html

CREATE TABLE users (
来源：http://hz.shuidangran.top/gtsijigzpi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xuetiantiany.cn/gturtjbdlx.html

name VARCHAR(50) NOT NULL,
来源：http://hz.guannengcc.top/gtzisqprkc.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgufenzy.top/gtghkffepv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.cqqwz.cn/gtayvnozic.html

);
来源：http://hz.jqgufenzy.top/gtbpwhkqln.html

[Q02] 创建带外键的表
来源：http://hz.andypj.xyz/gtwpimqnie.html

CREATE TABLE orders (
来源：http://hz.9152youxi.cn/gtbzbjbhvr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gtheqgmwfl.html

user_id INT NOT NULL,
来源：http://hz.zdqjudy.top/gtklzieksh.html

amount DECIMAL(10, 2),
来源：http://hz.jiagoushi.top/gtzpaiinxi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.ppjwa.cn/gtkstjvfkd.html

);
来源：http://hz.zycfv.cn/gtbyphjhmv.html

[Q03] 增加列
来源：http://hz.yangfankeji.com/gtktcaolwv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.hnqzz.top/gtxvohthrg.html

[Q04] 修改列类型
来源：http://hz.gogol.net.cn/gtfzjepcxa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xinyue.icu/gthiytiazc.html

[Q05] 重命名列
来源：http://hz.daria6918.cn/gtzvbwwjdi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cashguo.top/gtxqwrsydh.html

[Q06] 删除列
来源：http://hz.shanyushiyangtech.top/gtzeqejrjx.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhijiandao.cn/gtgfafssbd.html

[Q07] 删除表
来源：http://hz.havefunace.top/gttabavpne.html

DROP TABLE IF EXISTS orders;
来源：http://hz.smart0.xyz/gtkiacnrba.html

[Q08] 创建普通索引
来源：http://hz.aizwys.cn/gtiazrknfr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shuidangran.top/gtdpxmsele.html

[Q09] 创建唯一索引
来源：http://hz.ivvv.top/gtwpcdachl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.redwolf501.top/gtwytueyjs.html

[Q10] 插入单行
来源：http://hz.guowangkeji.top/gtitfirrvg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.meibo888.top/gtkpeygznd.html

[Q11] 一次插入多行
来源：http://hz.mhx1999.top/gtrizjvalw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtfkbpnecr.html

[Q12] 插入后取自增 ID
来源：http://hz.ybcxt.top/gthrpvcdit.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.iojbl.cn/gtnkmblceb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ehwqpu.com/gtbcjzfmps.html

[Q13] 忽略重复插入
来源：http://hz.quarkkingdee.top/gtysterfid.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zdqjudy.top/gtsyhzsgyi.html

[Q14] 存在则更新（upsert）
来源：http://hz.jinqigufen.top/gtrragzptc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jyoumei.cn/gtzcanknhg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shangyingyoupin.top/gtbmwozlsh.html

[Q15] 查询全部
来源：http://hz.gaohongyu789.top/gtppkevakv.html

SELECT * FROM users;
来源：http://hz.jinyuanbaomall.cn/gtemmeneki.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtpcevqfrw.html

SELECT id, name FROM users;
来源：http://hz.bjfxy.top/gtsnvivgag.html

[Q17] 条件查询
来源：http://hz.zhijiandao.cn/gtnidgkdcu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zhijiandao.cn/gtwarhgatm.html

[Q18] 模糊匹配
来源：http://hz.ivvv.top/gtsorfutzc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangkeji.top/gthoxekdfo.html

[Q19] 范围查询
来源：http://hz.xingfuxueyuan.xyz/gtlidqgbid.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.fengsongda.top/gtarovyeto.html

[Q20] IN 列表
来源：http://hz.fengsongda.top/gtwkihvnak.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.xylfe.cn/gtveixfozg.html

[Q21] 空值判断
来源：http://hz.xingfuxueyuan.xyz/gtucnbyrer.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tian-w.cn/gtumsfduqf.html

[Q22] 排序
来源：http://hz.cqqwz.cn/gtqshwmdnf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenlongwang.top/gtsbmpnnlk.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtbvtltmuk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.xinyue.icu/gtcyjqwoex.html

[Q24] 去重
来源：http://hz.quarkkingdee.top/gtlegnnsep.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydjk.org.cn/gtrcmjolkd.html

[Q25] 只取前 N 条
来源：http://hz.kuanghao11.cn/gtoarhpilq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtxkxbcqtq.html

[Q26] 计数
来源：http://hz.ivvv.top/gtuxohmoca.html

SELECT COUNT(*) FROM users;
来源：http://hz.c1oappe.top/gtqlhdilrn.html

[Q27] 条件计数
来源：http://hz.c1oappe.top/gtmcamzdku.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtaclynobh.html

[Q28] 求和与平均
来源：http://hz.xylfe.cn/gtveexccri.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhongyouzk.top/gtoggryswt.html

[Q29] 最大最小值
来源：http://hz.sufxvd.cn/gtlzizvjka.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yonumen.top/gtbkfautvw.html

[Q30] 分组统计
来源：http://hz.zhongyouzk.top/gtjdehcxzr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtczajaxgk.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangtech.top/gtwwfdfsbo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.vqdsnc.cn/gtxdeazavx.html

[Q32] 分组拼接字符串
来源：http://hz.hnqzz.top/gtvqnwjeje.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhaomingkeji.xyz/gtsroavndh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ydjk.org.cn/gtgjgzdxcv.html

[Q33] 多列分组
来源：http://hz.quarkkingdee.top/gtazslafiz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hfpthk.cn/gtdoqxspfn.html

[Q34] 每组取第一条
来源：http://hz.jianghu66.top/gtsfzmpmyt.html

SELECT * FROM (
来源：http://hz.yuanzhike.top/gtuxkzxxmh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daria6918.cn/gtffizpyec.html

) t WHERE rn = 1;
来源：http://hz.hnqzz.top/gtineznagm.html

[Q35] 内连接
来源：http://hz.fzhhl.top/gtjactnayb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtauczwgqb.html

[Q36] 左连接
来源：http://hz.smart0.xyz/gtcdhqngec.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtzxifycwn.html

[Q37] 右连接
来源：http://hz.ppjwa.cn/gtzzsjnzix.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yonumen.top/gtjkmblqum.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.smart0.xyz/gtlvdqamdl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.meibo888.top/gtqgkmwswt.html

[Q39] 自连接（查上下级）
来源：http://hz.yangfankeji.com/gtkjmuozfc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuanzx.com/gtxxzobdsf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gtycwsgumo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxinkj.top/gtguzpahyo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinghuilouyu.cn/gtlvjyomof.html

[Q41] 多表连接
来源：http://hz.yj202588.top/gtwgxdcsoz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zycfv.cn/gtrmunfjwt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jiagoushi.top/gtmfdbpxmt.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhengqikj.top/gtjgjnrqth.html

[Q42] 连接条件附加过滤
来源：http://hz.birdmap.top/gtihtxuqgx.html

SELECT u.name, o.amount FROM users u
来源：http://hz.c1oappe.top/gtrqblcpkv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shzxlz.cn/gtervtgmaz.html

[Q43] 标量子查询
来源：http://hz.hongshengwenyu.top/gtnrmyrgqp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.tianlin.xyz/gtmovygfim.html

[Q44] IN 子查询
来源：http://hz.xylfe.cn/gtnsoybgwp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtvqylekmn.html

[Q45] EXISTS 判断存在
来源：http://hz.shanyushiyangkeji.top/gtfgnmnslw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhongyouzk.top/gtmqowthuy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhoulong.xyz/gteayosrpe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gttayihezo.html

[Q47] 与平均值比较
来源：http://hz.cqqwz.cn/gtunvjfmsg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigufen.top/gtmwiyfjsq.html

[Q48] CTE 公用表表达式
来源：http://hz.nanxuanxn.top/gtctvspdzu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tanke756.top/gtvcjrasmy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.kuanghao11.cn/gtzehncrqp.html

[Q49] 更新单行
来源：http://hz.mhx1999.top/gtwcdvyows.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.9152youxi.cn/gtajdbfftn.html

[Q50] 批量更新
来源：http://hz.jiagoushi.top/gtvsgusbco.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cqqwz.cn/gtddyuzozn.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtvcuwpgqp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cdnleiting.top/gtxsclcjma.html

[Q52] 删除指定行
来源：http://hz.xziqi.cn/gtjmlykbbd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tian-w.cn/gtpenfbakj.html

[Q53] 按条件删除
来源：http://hz.52xcode.cn/gtycbmnkfw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tianlin.xyz/gtukirjvok.html

[Q54] 清空表
来源：http://hz.yonumen.top/gtpdfgvmfb.html

TRUNCATE TABLE logs;
来源：http://hz.shangyingyoupin.top/gtmrjllfiq.html

[Q55] 排名（并列占位）
来源：http://hz.xingfuxueyuan.xyz/gtqpckokbm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigufen.top/gtgipkccto.html

[Q56] 密集排名（并列不占位）
来源：http://hz.cheryme.top/gthvaisowc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jiagoushi.top/gtsugswmmy.html

[Q57] 行号
来源：http://hz.jqgfzy.top/gtibaktawa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenjidiqi.icu/gtfucpmsaa.html

[Q58] 累计求和
来源：http://hz.yueranfly.top/gtkgchonuc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pengpengdd.cyou/gtbjfqdrlf.html

[Q59] 分组内累计
来源：http://hz.sysykeji.top/gtiyzbnchq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yueranfly.top/gtdkvayznl.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gtgsgnyove.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gogol.net.cn/gtqibcuabv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ivvv.top/gtlpxbrtga.html

[Q61] 移动平均
来源：http://hz.yanxiufei.cn/gtlyffmgkb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jqgufenzy.top/gtavihqtgn.html

[Q62] 分组占比
来源：http://hz.tanke756.top/gtepchzazr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tianlin.xyz/gtedndmrgg.html

[Q63] 开启事务
来源：http://hz.zhongyouzk.top/gtbougfjvg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinyuanbaomall.cn/gtjpefnzwh.html

[Q64] 提交事务
来源：http://hz.yvedp.cn/gtfmuhzipe.html

COMMIT;
来源：http://hz.jiagoushi.top/gtlmkxdjew.html

[Q65] 回滚事务
来源：http://hz.meibo888.top/gtvgxisxwd.html

ROLLBACK;
来源：http://hz.hywenlv.cn/gtrbxmfuxk.html

[Q66] 行锁查询
来源：http://hz.jlsjyb.cn/gtnvbxzewv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yangfankeji.com/gtpuclbnho.html

[Q67] 设置隔离级别
来源：http://hz.aizwys.cn/gtxqlwusiv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.bjfxy.top/gtaxbxjwig.html

[Q68] 保存点
来源：http://hz.ppjwa.cn/gtvkihmbch.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtyeashmvx.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gtnedyzwni.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtjpdxrkef.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtdldalpyu.html

[Q70] 更新统计信息
来源：http://hz.jyoumei.cn/gtrdrkanbg.html

ANALYZE TABLE users;
来源：http://hz.chenlongwang.top/gtaecbuxhf.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangkeji.top/gtzmiswlje.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zdqjudy.top/gtmbgtzrfu.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gtymgyjxhr.html

SHOW INDEX FROM users;
来源：http://hz.yvedp.cn/gtseaspums.html

[Q73] 查看表状态
来源：http://hz.ydjk.org.cn/gtawcziroe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.birdmap.top/gtrkfzortc.html

[Q74] 强制使用索引
来源：http://hz.iojbl.cn/gtrzafnbdm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.nanxuanxn.top/gtewoliceq.html

[Q75] 日期格式化
来源：http://hz.yongpay.top/gtrgpbpztr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.snrcjt.cn/gtzjlrwzcg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtldwpxxxb.html

[Q76] 按天统计
来源：http://hz.tianlin.xyz/gtwkypbfrj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhongyouzk.top/gtzzpeecji.html

[Q77] 时间加减
来源：http://hz.jyoumei.cn/gtymcbgxxp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fzhhl.top/gthhxqamlu.html

[Q78] 当前时间
来源：http://hz.zhixingplan.top/gtyqvhttev.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shuidangran.top/gtyfyoibyo.html

[Q79] 字符串拼接
来源：http://hz.cqqwz.cn/gtrjbszbve.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258888.top/gtvjhulomz.html

[Q80] 字符串截取
来源：http://hz.xuanzx.com/gtqvrvorbj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daria6918.cn/gtfrxlvgqk.html

[Q81] 字符串替换
来源：http://hz.vqdsnc.cn/gthgrckedd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtbmzpijpu.html

[Q82] 字符长度与字节长度
来源：http://hz.guannengcc.top/gtbjwpbqql.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.havefunace.top/gtmjiowfbw.html

[Q83] 大小写转换
来源：http://hz.wangdashe.top/gtqgfbrjue.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gtpnszswpa.html

[Q84] 去除首尾空格
来源：http://hz.yonumen.top/gtywcdopux.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtsopeodbx.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtcnksoiwx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgfzy.top/gtxyawpfhc.html

[Q86] 读取 JSON 字段
来源：http://hz.gotoacloud.top/gthvtelixz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtmhlfjxvy.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtrtyoxjzh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shangyingyoupin.top/gtuiifpnsj.html

[Q88] 行转列（条件聚合）
来源：http://hz.snrcjt.cn/gtstyltagt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tanke756.top/gtrzbigoyq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtrflpeday.html

[Q89] 判断表是否存在
来源：http://hz.jqgufenzy.top/gtezyewpne.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shangyingyoupin.top/gtzmmnqqnm.html

[Q90] 生成序号列
来源：http://hz.zycfv.cn/gtpkxxctbq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sxryk.cn/gtmkmohsrl.html

================================================================================
来源：http://hz.hywenlv.cn/gtciznyeey.html

R. Bash 专题
来源：http://hz.shuidangran.top/gtmjnfafvm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgedqavgj.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtgnkzibun.html

#!/usr/bin/env bash
来源：http://hz.yj202588.top/gttvvuyzsq.html

set -euo pipefail
来源：http://hz.iojbl.cn/gtlygagrij.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtdqjyrftu.html

name="Tom"; echo "$name"
来源：http://hz.shuidangran.top/gtkhzdkeom.html

[R03] 只读变量
来源：http://hz.9152youxi.cn/gtmvrndscj.html


<!-- 参考信息 -->