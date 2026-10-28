代发 wailian999

[O06] 使用进程池
来源：http://hz.sweek.top/gtxtyvzyij.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.ppjwa.cn/gtdhpylcty.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhoulong.xyz/gtjvehojex.html

JS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtlqllcmeg.html

TS:   // child_process / cluster 模块
来源：http://hz.shzxlz.cn/gtpaajofgb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yj202588.top/gtomjwvhok.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhiwuduotai.top/gttlnphqeo.html

Ruby: // fork 块
来源：http://hz.redwolf501.top/gtzveazykz.html

C#:   Parallel.For
来源：http://hz.snrcjt.cn/gtjgvbjxnv.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgfafhind.html

P. 常用工具函数
来源：http://hz.ydjk.org.cn/gtqkfaqbfe.html

================================================================================
来源：http://hz.smart0.xyz/gtvlkltwru.html

[P01] 生成 UUID
来源：http://hz.hnqzz.top/gtjthqcnvm.html

Py:   str(uuid.uuid4())
来源：http://hz.dashuyun.cn/gtvkhvwmbg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sufxvd.cn/gtavhwlbhc.html

JS:   crypto.randomUUID()
来源：http://hz.9152youxi.cn/gtypiuxdld.html

TS:   crypto.randomUUID()
来源：http://hz.jinqigufen.top/gtxjpdqdql.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtnyyirvhg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.9152youxi.cn/gtpixdehsp.html

Ruby: SecureRandom.uuid
来源：http://hz.jyoumei.cn/gteedvcffk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.smart0.xyz/gtssxaalqx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangdashe.top/gtfjdlbuup.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fzhhl.top/gtgmubkshe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pycfn.com/gtavgcwtac.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pengpengdd.cyou/gtapmrveys.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nanxinkj.top/gtfwzbguqq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.aibaodan.cn/gttdnqhzox.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.0kj1m.cn/gtdowjakqm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.shanyushiyangtech.top/gtxjckypag.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.bjfxy.top/gtrcitpqil.html

[P03] 生成短随机字符串
来源：http://hz.dashuyun.cn/gtbsygueov.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtyrvjcxfl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zycfv.cn/gtoowkhwto.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtajatxsyj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtxjltwukh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.9152youxi.cn/gtgbhfsdqm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gaohongyu789.top/gtjgrpecdy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.hnqzz.top/gthqhcesip.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jianghu66.top/gtgudamofi.html

[P04] 求长度
来源：http://hz.feifeiyinyue.top/gtlusbugii.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zhixingplan.top/gtmzwjmtmj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtpguukdqe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtukbiitch.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtilegbfjp.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xuetiantiany.cn/gtbiciqldl.html

Go:   len(arr);  len(m)
来源：http://hz.shangyingyoupin.top/gtuatreynx.html

Ruby: x.length;  x.size
来源：http://hz.yangfankeji.com/gtreozjwar.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.yueranfly.top/gtbejpuigx.html

[P05] 判断两个对象内容是否相等
来源：http://hz.hfpthk.cn/gtbaovjfiz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.andypj.xyz/gtcvkomfbg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gtqykybtec.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.dashuyun.cn/gtoqytdyfi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtnlbqjdoi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.sweek.top/gtpevhhgxy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yvedp.cn/gtvxeyttlp.html

Ruby: a == b
来源：http://hz.hfpthk.cn/gtvcfsynlf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hysaishi.cn/gtgsjdnjcg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.tianlin.xyz/gtugqaodek.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.zycfv.cn/gtattyxpvc.html

PHP:  if (empty($x)) {}
来源：http://hz.gotoacloud.top/gthnfxgjhr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.tanke756.top/gtjyjkjfzw.html

TS:   if (x == null) {}
来源：http://hz.iojbl.cn/gtpdnirfpu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.hysaishi.cn/gtqdmnopli.html

Go:   if x == nil {}
来源：http://hz.yueranfly.top/gthfktkoti.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jyoumei.cn/gtnlislqut.html

C#:   if (x is null) {}
来源：http://hz.xuetiantiany.cn/gtqgwxymkp.html

[P07] 防抖与节流
来源：http://hz.xingfuxueyuan.xyz/gtllwobaoh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yueranfly.top/gtdjmvwvvb.html

PHP:  // 手写时间戳比较
来源：http://hz.tianlin.xyz/gtmdwbximt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtbdjzyceg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ppjwa.cn/gtkcuwtshb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.snrcjt.cn/gtqeljgnef.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jianghu66.top/gtvahkweny.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.fzhhl.top/gtqxhrvojg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gaohongyu789.top/gtfdoiorsa.html

[P08] 处理浮点精度问题
来源：http://hz.fengsongda.top/gtpgrcfvtx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yuxming.cn/gtmtkwcnyw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhengqikj.top/gtgfiwcmvp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhengqikj.top/gtgfokgori.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.tanke756.top/gtwhrvxpdw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yonumen.top/gttyomuxtx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.meibo888.top/gtepxjnvby.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.ywan-chungtsiang.top/gtwxffoxtz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yj20258888.top/gtiemafhlr.html

================================================================================
来源：http://hz.ehwqpu.com/gtinjpjumu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.jinghuilouyu.cn/gtvyneyigp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcevtmwlh.html

[Q01] 创建表
来源：http://hz.jyoumei.cn/gtxxymwdoc.html

CREATE TABLE users (
来源：http://hz.ybcxt.top/gtyzmuvokh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cucudq.cn/gttwkqvzjy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.dianchejie.cn/gtyitcazyy.html

email VARCHAR(100) UNIQUE,
来源：http://hz.xziqi.cn/gttdhqujpr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ybcxt.top/gtuxjcgkfr.html

);
来源：http://hz.ydzc1.top/gthqywtdov.html

[Q02] 创建带外键的表
来源：http://hz.tian-w.cn/gtsmuooofg.html

CREATE TABLE orders (
来源：http://hz.yongpay.top/gtgoqrfkce.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yonumen.top/gtldrshiux.html

user_id INT NOT NULL,
来源：http://hz.zhongyouzk.top/gtawisvnvn.html

amount DECIMAL(10, 2),
来源：http://hz.hnqzz.top/gtptszavcd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.cqqwz.cn/gtcfbtrznz.html

);
来源：http://hz.316326.xyz/gtzxuhnirp.html

[Q03] 增加列
来源：http://hz.iojbl.cn/gtfdznbiqe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.vqdsnc.cn/gtcbfrtvbe.html

[Q04] 修改列类型
来源：http://hz.yj202588.top/gtrpuatbwx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.shangyingyoupin.top/gtvhjsoxbf.html

[Q05] 重命名列
来源：http://hz.guannengcc.top/gtdomamtcq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hongshengwenyu.top/gtanfqdiuv.html

[Q06] 删除列
来源：http://hz.jinyuanbaomall.cn/gtxqgojztq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.zhengqikj.top/gtsicnlydx.html

[Q07] 删除表
来源：http://hz.zhixingplan.top/gtcocenxou.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhoulong.xyz/gtznjirvvf.html

[Q08] 创建普通索引
来源：http://hz.yangfankeji.com/gtihkcxlyh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.zycfv.cn/gtohvteyin.html

[Q09] 创建唯一索引
来源：http://hz.kuanghao11.cn/gthcpgdnnv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cashguo.top/gtdpjmpdst.html

[Q10] 插入单行
来源：http://hz.chenlongwang.top/gtdelrcnee.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cqqwz.cn/gtjftsblxm.html

[Q11] 一次插入多行
来源：http://hz.yj20258.top/gtyvjenyxc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hongshengwenyu.top/gtaybynbxv.html

[Q12] 插入后取自增 ID
来源：http://hz.9152youxi.cn/gtwwtoxjac.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtdkxzfvpo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtfbvpmdbm.html

[Q13] 忽略重复插入
来源：http://hz.ivvv.top/gtteaxzbkc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.shuidangran.top/gtvuikmaya.html

[Q14] 存在则更新（upsert）
来源：http://hz.sxryk.cn/gtzxgnscnr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.yongpay.top/gthmrdttzo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.jyoumei.cn/gtdsotgtmm.html

[Q15] 查询全部
来源：http://hz.fzhhl.top/gtyaypbxih.html

SELECT * FROM users;
来源：http://hz.ybcxt.top/gtyvwldrwb.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gthtyvjjhw.html

SELECT id, name FROM users;
来源：http://hz.kuanghao11.cn/gtujpbtlnd.html

[Q17] 条件查询
来源：http://hz.cqqwz.cn/gtrrfkytrj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yuxming.cn/gtempjuwhc.html

[Q18] 模糊匹配
来源：http://hz.iojbl.cn/gthucnnlkl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cucudq.cn/gtxzdwnuxt.html

[Q19] 范围查询
来源：http://hz.jinyuanbaomall.cn/gtbmhmtxps.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jqgfzy.top/gtbemgdbjl.html

[Q20] IN 列表
来源：http://hz.jqgfzy.top/gtfwyrcyod.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cdnleiting.top/gtktldxqzl.html

[Q21] 空值判断
来源：http://hz.gzhubu.top/gtfpbolfkg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.hnxiangtu.top/gtbqetxywy.html

[Q22] 排序
来源：http://hz.jinghuilouyu.cn/gtuwuvdtoh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xziqi.cn/gtokqznoks.html

[Q23] 分页
来源：http://hz.nanxuanxn.top/gtoyiukvbz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hywenlv.cn/gtjhwypqah.html

[Q24] 去重
来源：http://hz.daxiang520.top/gthgxmanpp.html

SELECT DISTINCT city FROM users;
来源：http://hz.dianchejie.cn/gtugcguwuj.html

[Q25] 只取前 N 条
来源：http://hz.wangdashe.top/gtzllcatre.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gtqutkbgzv.html

[Q26] 计数
来源：http://hz.xylfe.cn/gtttufcvhs.html

SELECT COUNT(*) FROM users;
来源：http://hz.xuetiantiany.cn/gtcxfuggxh.html

[Q27] 条件计数
来源：http://hz.yuxming.cn/gthxvxykfp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.ybcxt.top/gtdofyceso.html

[Q28] 求和与平均
来源：http://hz.gzhubu.top/gtbqfosmrg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dianchejie.cn/gtbtmbrnrl.html

[Q29] 最大最小值
来源：http://hz.aizwys.cn/gtfjittqlr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.chenzaomai.com/gtcwrdhlhk.html

[Q30] 分组统计
来源：http://hz.tanke756.top/gtnzoxwaeo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gtptagdzgj.html

[Q31] 分组后过滤
来源：http://hz.chenzaomai.com/gtqovbdsqp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenlongwang.top/gtsqnkjrkh.html

[Q32] 分组拼接字符串
来源：http://hz.birdmap.top/gtkkcedcwb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtnvzhhskl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aizwys.cn/gttxteohkt.html

[Q33] 多列分组
来源：http://hz.shanyushiyangtech.top/gtpgruxvmv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangkeji.top/gtiqsstcqq.html

[Q34] 每组取第一条
来源：http://hz.cdnleiting.top/gtsqosyvgy.html

SELECT * FROM (
来源：http://hz.shanyushiyangkeji.top/gtndcpvcjc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ehwqpu.com/gtwtjfcbzp.html

) t WHERE rn = 1;
来源：http://hz.c1oappe.top/gthscmzytg.html

[Q35] 内连接
来源：http://hz.hnxiangtu.top/gtqwbdybqf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yongpay.top/gthdzhcvjv.html

[Q36] 左连接
来源：http://hz.ybcxt.top/gtwxpusbza.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.nanxuanxn.top/gtnwecfwxp.html

[Q37] 右连接
来源：http://hz.guannengcc.top/gtdsvkdyal.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sufxvd.cn/gtklrjuwco.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.vqdsnc.cn/gtfapexfrv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.guowangkeji.top/gtxlovsziv.html

[Q39] 自连接（查上下级）
来源：http://hz.shuidangran.top/gtrkqsfbbg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hammf.cn/gteojrkyup.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yvedp.cn/gtijqasexe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhixingplan.top/gtjqiieirj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtvqqglcjc.html

[Q41] 多表连接
来源：http://hz.yangfankeji.com/gtrilfhxga.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cdnleiting.top/gtygnurbyv.html

JOIN users u ON u.id = o.user_id
来源：http://hz.kuanghao11.cn/gtqnxttsfx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.vqdsnc.cn/gtdtqqearl.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigufen.top/gtdzqrxdni.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shzxlz.cn/gtdqjtcfxt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.xingfuxueyuan.xyz/gtpwkhlhrp.html

[Q43] 标量子查询
来源：http://hz.jqgufenzy.top/gtruopitxd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gtjohziucz.html

[Q44] IN 子查询
来源：http://hz.hnxiangtu.top/gtmrbizbxq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.kuanghao11.cn/gtbhnlalbm.html

[Q45] EXISTS 判断存在
来源：http://hz.hywenlv.cn/gtfpkqqyjk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xuanzx.com/gtyblbbpvs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yangfankeji.com/gtbdqbunvn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtusewxraw.html

[Q47] 与平均值比较
来源：http://hz.fengsongda.top/gtihdhaqzj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.birdmap.top/gtdgycjzbx.html

[Q48] CTE 公用表表达式
来源：http://hz.shanyushiyangkeji.top/gtwguufkup.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtuviwlddi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinyuanbaomall.cn/gttspjhjta.html

[Q49] 更新单行
来源：http://hz.jlsjyb.cn/gtiopufqkg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.smart0.xyz/gtzlbsgvio.html

[Q50] 批量更新
来源：http://hz.sxryk.cn/gtplhurjjt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sxryk.cn/gtbskvsacr.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtsptysebi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.haohaochexian.top/gtluffklre.html

[Q52] 删除指定行
来源：http://hz.nanxuanxn.top/gtoewhovvb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jyoumei.cn/gtdvojkiww.html

[Q53] 按条件删除
来源：http://hz.kuanghao11.cn/gtnodwjkdn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangtech.top/gtjkwmxcaj.html

[Q54] 清空表
来源：http://hz.ivvv.top/gtlibaavph.html

TRUNCATE TABLE logs;
来源：http://hz.dashuyun.cn/gtwilqunve.html

[Q55] 排名（并列占位）
来源：http://hz.hnxiangtu.top/gtnswhctwt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.redwolf501.top/gtqlsvmvoi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nwbrower.top/gterdcaddb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gogol.net.cn/gtbffzevhm.html

[Q57] 行号
来源：http://hz.pycfn.com/gtsxrlsdbl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinghuilouyu.cn/gtumrcblmb.html

[Q58] 累计求和
来源：http://hz.yj20258.top/gtgylaotkn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtndhyczbf.html

[Q59] 分组内累计
来源：http://hz.gzhubu.top/gtxfcvupkw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tian-w.cn/gtanwoznba.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj202588.top/gttvzrduyy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yongpay.top/gtpmkuhspa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258.top/gtmlkroevw.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtfsiyfvvb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtymyadruo.html

[Q62] 分组占比
来源：http://hz.jqgufenzy.top/gtxnxgmwne.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.iojbl.cn/gtcsnnzysa.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gttocfpnrd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zycfv.cn/gtjrbobfft.html

[Q64] 提交事务
来源：http://hz.cheryme.top/gtfaxnhzyi.html

COMMIT;
来源：http://hz.chenjidiqi.icu/gtnxasvddn.html

[Q65] 回滚事务
来源：http://hz.jinqigufen.top/gtjryaerus.html

ROLLBACK;
来源：http://hz.bjfxy.top/gtlhslbcgb.html

[Q66] 行锁查询
来源：http://hz.pycfn.com/gtfhqtycrd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ehwqpu.com/gtjpuclfvn.html

[Q67] 设置隔离级别
来源：http://hz.nwbrower.top/gtdrtsqgkk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtedlobnnd.html

[Q68] 保存点
来源：http://hz.jianghu66.top/gtduhrwwaz.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtlwynsfyv.html

ROLLBACK TO sp1;
来源：http://hz.haohaochexian.top/gtbakoeuyf.html

[Q69] 查看执行计划
来源：http://hz.gaohongyu789.top/gtwyotyihc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pengpengdd.cyou/gtercwryuc.html

[Q70] 更新统计信息
来源：http://hz.guowangkeji.top/gtcwwksxzp.html

ANALYZE TABLE users;
来源：http://hz.hnxiangtu.top/gtzteegbro.html

[Q71] 查看建表语句
来源：http://hz.cucudq.cn/gtjkvwtehc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dianchejie.cn/gtowufdsqf.html

[Q72] 查看索引
来源：http://hz.birdmap.top/gtqczhsbsh.html

SHOW INDEX FROM users;
来源：http://hz.cashguo.top/gtpsmcaavn.html

[Q73] 查看表状态
来源：http://hz.svipenyu.cn/gtuhcjzpkk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.andypj.xyz/gtzamgqrta.html

[Q74] 强制使用索引
来源：http://hz.svipenyu.cn/gtaddooxol.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.quarkkingdee.top/gtzjwdwabb.html

[Q75] 日期格式化
来源：http://hz.hysaishi.cn/gtvfgzumka.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hongshengwenyu.top/gtqgknqcca.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.mhx1999.top/gtesorebut.html

[Q76] 按天统计
来源：http://hz.haohaochexian.top/gtwnblcgxz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gtxhlzcvfo.html

[Q77] 时间加减
来源：http://hz.yanxiufei.cn/gtzahwuwik.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangkeji.top/gtvuvpsbrj.html

[Q78] 当前时间
来源：http://hz.ydjk.org.cn/gtbhudbrdh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aibaodan.cn/gtuexjnslu.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtcqpzgvvx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gtvxklvxmn.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gtdvutdqyy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.haohaochexian.top/gtorjxblyo.html

[Q81] 字符串替换
来源：http://hz.zhengqikj.top/gtgaddpdmk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.birdmap.top/gttsitypiq.html

[Q82] 字符长度与字节长度
来源：http://hz.zhaomingkeji.xyz/gtelqgeexr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtkkforprk.html

[Q83] 大小写转换
来源：http://hz.hammf.cn/gtqgggojiu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtqmonwuip.html

[Q84] 去除首尾空格
来源：http://hz.gzhubu.top/gtxvbiairg.html

SELECT TRIM(name) FROM users;
来源：http://hz.cqqwz.cn/gtdthhbcjk.html

[Q85] 数值取整
来源：http://hz.jyoumei.cn/gtkvywowbc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.c1oappe.top/gtgjlnyvsp.html

[Q86] 读取 JSON 字段
来源：http://hz.ydjk.org.cn/gtjdeyhfoo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangkeji.top/gtdyenwhgs.html

[Q87] JSON 字段做条件
来源：http://hz.havefunace.top/gtqxhurutm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aizwys.cn/gtniieodrv.html

[Q88] 行转列（条件聚合）
来源：http://hz.ivvv.top/gtefhghesd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.andypj.xyz/gtkqjkvtio.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgufenzy.top/gtffeoxafd.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtdrdrchmp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtgbvfwbar.html

[Q90] 生成序号列
来源：http://hz.yueranfly.top/gtqoqnugvs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.snrcjt.cn/gtxnyaziew.html

================================================================================
来源：http://hz.zhijiandao.cn/gtaixiibrl.html

R. Bash 专题
来源：http://hz.feifeiyinyue.top/gtzapvluvx.html

================================================================================
来源：http://hz.yangfankeji.com/gtdmuagdah.html

[R01] shebang 与严格模式
来源：http://hz.ivvv.top/gtsqeczpxc.html

#!/usr/bin/env bash
来源：http://hz.svipenyu.cn/gtjsgvwzjt.html

set -euo pipefail
来源：http://hz.zhengqikj.top/gtupyjrdto.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gtfpdxuvgu.html

name="Tom"; echo "$name"
来源：http://hz.yonumen.top/gtlpsqtpzp.html

[R03] 只读变量
来源：http://hz.sweek.top/gtrlukyqcz.html


<!-- 参考信息 -->