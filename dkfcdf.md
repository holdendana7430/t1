代发 wailian999

[O06] 使用进程池
来源：http://hz.zhijiandao.cn/gtsqlxgcxl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hysaishi.cn/gtvitjykwp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258.top/gtwvcfwgwf.html

JS:   // child_process / cluster 模块
来源：http://hz.yueranfly.top/gtjfrmeywn.html

TS:   // child_process / cluster 模块
来源：http://hz.zhoulong.xyz/gtydsfkuwc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zycfv.cn/gtxvpifqqv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hammf.cn/gtktmgmojh.html

Ruby: // fork 块
来源：http://hz.birdmap.top/gtqdxgeksh.html

C#:   Parallel.For
来源：http://hz.xinyue.icu/gtajeuebgo.html

================================================================================
来源：http://hz.yj20258888.top/gtwriyegtr.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtxnopgbhi.html

================================================================================
来源：http://hz.zhixingplan.top/gtarzlmcjl.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gtcpvxzlec.html

Py:   str(uuid.uuid4())
来源：http://hz.cashguo.top/gtkvbqovyi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tanke756.top/gtwdgvicsy.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtssirnoup.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtfwdvrxds.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtjtffqyoy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinyuanbaomall.cn/gtoqvpefwi.html

Ruby: SecureRandom.uuid
来源：http://hz.bjfxy.top/gtoeiqrevl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gzhubu.top/gtadoefnom.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shzxlz.cn/gtkjypkevh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.feifeiyinyue.top/gtyujerben.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.daxiang520.top/gtusscrejk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.xylfe.cn/gtxkslyrzu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yongpay.top/gtrpaghxzm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jinghuilouyu.cn/gtmhofrgsm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hywenlv.cn/gtnmhgluqu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daxiang520.top/gtrzwpdtvg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.kuanghao11.cn/gtluaaizsl.html

[P03] 生成短随机字符串
来源：http://hz.shangyingyoupin.top/gtcmhavsek.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cheryme.top/gtofxqvjqp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.dashuyun.cn/gtlspbxisx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.tian-w.cn/gthmfagzcs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtdlujfryl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nwbrower.top/gtwmtchjto.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.aizwys.cn/gtqjlcelbz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.xuetiantiany.cn/gtqwekkyso.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuanzhike.top/gtqqonbkls.html

[P04] 求长度
来源：http://hz.guowangkeji.top/gtitwrbhos.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ehwqpu.com/gtbemztuir.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gthjtkotyd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtgzknroko.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.havefunace.top/gtvqsberys.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gtchxqhvia.html

Go:   len(arr);  len(m)
来源：http://hz.ydzc1.top/gtcnfuyrfb.html

Ruby: x.length;  x.size
来源：http://hz.yj20258888.top/gtpgpbtcfz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ybcxt.top/gtjfpyxetd.html

[P05] 判断两个对象内容是否相等
来源：http://hz.sysykeji.top/gtcndgiyho.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.havefunace.top/gtmihwlanj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gzhubu.top/gtpoflygml.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.cqqwz.cn/gtvozljwgg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtpmeonqpc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ybcxt.top/gtobhajatn.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.yuxming.cn/gtuqjjuows.html

Ruby: a == b
来源：http://hz.andypj.xyz/gtoejcfsft.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangkeji.top/gtbkwsuugm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.sysykeji.top/gtvkjzxrep.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jyoumei.cn/gtcawpznox.html

PHP:  if (empty($x)) {}
来源：http://hz.haohaochexian.top/gtecvokhxs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hysaishi.cn/gtdfgaoywe.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gthyabbbfc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.ywan-chungtsiang.top/gtmukiysnt.html

Go:   if x == nil {}
来源：http://hz.smart0.xyz/gtppgfqnwr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.hfpthk.cn/gtrkuyndlq.html

C#:   if (x is null) {}
来源：http://hz.jyoumei.cn/gtdvwkiyun.html

[P07] 防抖与节流
来源：http://hz.chenlongwang.top/gtiecnluel.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.dianchejie.cn/gtdaqcwxkr.html

PHP:  // 手写时间戳比较
来源：http://hz.cheryme.top/gtqoqgwofk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtsxluppss.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtoczbkogt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.haohaochexian.top/gtoosknpws.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj202588.top/gttmtqdoij.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.sweek.top/gtfbswclnc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.chenzaomai.com/gtsokghznr.html

[P08] 处理浮点精度问题
来源：http://hz.jqgfzy.top/gtcptwtrym.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jlsjyb.cn/gtcvouccxt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yueranfly.top/gtohsayaau.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.aibaodan.cn/gtzrpcnzeu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zdqjudy.top/gtwtzqwloe.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.pengpengdd.cyou/gtyucueyis.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtatgezygu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daxiang520.top/gtwjgiextm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.ywan-chungtsiang.top/gtptnpdqau.html

================================================================================
来源：http://hz.aizwys.cn/gtqodbyxdm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.gotoacloud.top/gtcypfkyvb.html

================================================================================
来源：http://hz.xziqi.cn/gtdpzedrfx.html

[Q01] 创建表
来源：http://hz.ivvv.top/gtysgmztxo.html

CREATE TABLE users (
来源：http://hz.shzxlz.cn/gtcsohwvgr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yueranfly.top/gtgrcobdqj.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hfpthk.cn/gtqliannas.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jlsjyb.cn/gtvzkxdllq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.zdqjudy.top/gtewjgupxi.html

);
来源：http://hz.feifeiyinyue.top/gtgzykhaqm.html

[Q02] 创建带外键的表
来源：http://hz.shzxlz.cn/gtcupemnfw.html

CREATE TABLE orders (
来源：http://hz.zhaomingkeji.xyz/gtjyhxljnd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.vqdsnc.cn/gteapjbrjc.html

user_id INT NOT NULL,
来源：http://hz.52xcode.cn/gtinywcsxy.html

amount DECIMAL(10, 2),
来源：http://hz.ivvv.top/gtkhamgihr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jqgfzy.top/gtnskxsths.html

);
来源：http://hz.hnqzz.top/gtrzbtpsiz.html

[Q03] 增加列
来源：http://hz.jinqigfzy.top/gtatylnifr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shzxlz.cn/gtptxfujwn.html

[Q04] 修改列类型
来源：http://hz.9152youxi.cn/gtfdegstok.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.cucudq.cn/gtblutpcwu.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtdlnxfwyo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ywan-chungtsiang.top/gtxmjgepgv.html

[Q06] 删除列
来源：http://hz.sweek.top/gtyrdzzeed.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hnqzz.top/gtusllieqb.html

[Q07] 删除表
来源：http://hz.yuanzhike.top/gtbibfgxdr.html

DROP TABLE IF EXISTS orders;
来源：http://hz.sysykeji.top/gtvmyqcdmo.html

[Q08] 创建普通索引
来源：http://hz.vqdsnc.cn/gtcnzcpugp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.sweek.top/gtbsbgjxyr.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtkdsbqyfy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnqzz.top/gthckdbipw.html

[Q10] 插入单行
来源：http://hz.yongpay.top/gtsqbezmnk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cashguo.top/gtjxlwvvrv.html

[Q11] 一次插入多行
来源：http://hz.jinqigfzy.top/gtqcvdjbqo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shanyushiyangtech.top/gtipeeqzhe.html

[Q12] 插入后取自增 ID
来源：http://hz.zhiwuduotai.top/gtaqizsyef.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jyoumei.cn/gtfsrafvry.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.ydzc1.top/gtjinrkxiy.html

[Q13] 忽略重复插入
来源：http://hz.jinghuilouyu.cn/gtwwqcdgga.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.0kj1m.cn/gtnzpbfhih.html

[Q14] 存在则更新（upsert）
来源：http://hz.316326.xyz/gtvzvpmmgt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.gzhubu.top/gtovoauqzd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ivvv.top/gtokzscfuf.html

[Q15] 查询全部
来源：http://hz.ivvv.top/gteprottuw.html

SELECT * FROM users;
来源：http://hz.mhx1999.top/gtloxadcgm.html

[Q16] 查询指定列
来源：http://hz.tanke756.top/gtsioiulfu.html

SELECT id, name FROM users;
来源：http://hz.52xcode.cn/gtduiixspb.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtwjzwklwu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtplstybmc.html

[Q18] 模糊匹配
来源：http://hz.meibo888.top/gtnumjufkj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.daria6918.cn/gtepkwsuah.html

[Q19] 范围查询
来源：http://hz.aizwys.cn/gtgibcmonm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.birdmap.top/gtcinleisw.html

[Q20] IN 列表
来源：http://hz.zhaomingkeji.xyz/gtcdxwzhfm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhengqikj.top/gtxakumhho.html

[Q21] 空值判断
来源：http://hz.feifeiyinyue.top/gtwzhsuunm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtqmkonvgk.html

[Q22] 排序
来源：http://hz.ybcxt.top/gtgztgqldz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenzaomai.com/gtmvllvehk.html

[Q23] 分页
来源：http://hz.gaohongyu789.top/gtyvxmyijc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgfzy.top/gtjifzhomq.html

[Q24] 去重
来源：http://hz.ybcxt.top/gtyqoczqnk.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangkeji.top/gtdvlyubbd.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtqarjyary.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.fengsongda.top/gtnevjcsmw.html

[Q26] 计数
来源：http://hz.c1oappe.top/gtsylbexye.html

SELECT COUNT(*) FROM users;
来源：http://hz.vqdsnc.cn/gtrwpsaqbl.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtynbnhjrc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hysaishi.cn/gtwjvbywyp.html

[Q28] 求和与平均
来源：http://hz.zhixingplan.top/gtuureetay.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.havefunace.top/gtvrpnfiif.html

[Q29] 最大最小值
来源：http://hz.quarkkingdee.top/gtrwsgiltl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtwtrhqxlf.html

[Q30] 分组统计
来源：http://hz.xylfe.cn/gthxyrclpk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtpmxblyoa.html

[Q31] 分组后过滤
来源：http://hz.guowangkeji.top/gtgvzxgjqx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gtdwoueezo.html

[Q32] 分组拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtrpcldtyr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtnpimmotn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.52xcode.cn/gtsuwkztlo.html

[Q33] 多列分组
来源：http://hz.guannengcc.top/gtisesexqo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.aibaodan.cn/gtjmettmhp.html

[Q34] 每组取第一条
来源：http://hz.yuanzhike.top/gteucyvjdg.html

SELECT * FROM (
来源：http://hz.meibo888.top/gtvmsjkozb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.smart0.xyz/gtueuymlhv.html

) t WHERE rn = 1;
来源：http://hz.yvedp.cn/gtyktsumrv.html

[Q35] 内连接
来源：http://hz.gzhubu.top/gtoabvktmr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtcpjiqjxl.html

[Q36] 左连接
来源：http://hz.havefunace.top/gtmoefssnr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.52xcode.cn/gtcqkjunzh.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gtungtnwzc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tianlin.xyz/gtuuhsrkso.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hywenlv.cn/gtbcepvrfm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtgcwklyqi.html

[Q39] 自连接（查上下级）
来源：http://hz.cheryme.top/gtjwrdqwdi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xylfe.cn/gtnbymybbj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtlhgtvodt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.fengsongda.top/gtrmjixuyp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gotoacloud.top/gtbnckcjtm.html

[Q41] 多表连接
来源：http://hz.shzxlz.cn/gtdrdamzyo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenjidiqi.icu/gterlzhpcq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtxwczjslh.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yuxming.cn/gtazuqlvrc.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258.top/gtnxrzaxqw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.chenjidiqi.icu/gthrwblnyz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cucudq.cn/gtrjssswls.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gtkbidmryw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xuanzx.com/gtkdrrpttb.html

[Q44] IN 子查询
来源：http://hz.xuanzx.com/gtweqnxvzx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.snrcjt.cn/gtykwygrnv.html

[Q45] EXISTS 判断存在
来源：http://hz.chenzaomai.com/gthamyzmfx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pycfn.com/gtaemdefii.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxuanxn.top/gttrfqaokk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtkbkqmmhi.html

[Q47] 与平均值比较
来源：http://hz.zhoulong.xyz/gtjorqtnvv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinyuanbaomall.cn/gtanjwiuqb.html

[Q48] CTE 公用表表达式
来源：http://hz.c1oappe.top/gtegahgdxd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtmcbrbgey.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.tian-w.cn/gtiloypeae.html

[Q49] 更新单行
来源：http://hz.9152youxi.cn/gtdldulqfn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xziqi.cn/gtrmjcmucu.html

[Q50] 批量更新
来源：http://hz.svipenyu.cn/gtyhibbxyo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.nanxuanxn.top/gtzvtfzkzk.html

[Q51] 用子查询更新
来源：http://hz.ydjk.org.cn/gtgumemyam.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cqqwz.cn/gtznzgopzy.html

[Q52] 删除指定行
来源：http://hz.cheryme.top/gtwjbtzrrw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtgwwzrvev.html

[Q53] 按条件删除
来源：http://hz.chenjidiqi.icu/gtifhxnnnl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yonumen.top/gtfcpwzqmd.html

[Q54] 清空表
来源：http://hz.ydjk.org.cn/gtxqkudawr.html

TRUNCATE TABLE logs;
来源：http://hz.gaohongyu789.top/gtkocsodow.html

[Q55] 排名（并列占位）
来源：http://hz.jyoumei.cn/gtsxmvoatw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jlsjyb.cn/gtjogpwjqr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jqgufenzy.top/gtdetqjvhu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnxiangtu.top/gtxnxvdgtk.html

[Q57] 行号
来源：http://hz.9152youxi.cn/gtydkesjgh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yangfankeji.com/gthrunnhoo.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gthqacuuxg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtxfnijybz.html

[Q59] 分组内累计
来源：http://hz.chenzaomai.com/gtrxbnvpzl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtwhrjhyaw.html

[Q60] 取上一行 / 下一行
来源：http://hz.jyoumei.cn/gtbqixzcsx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jlsjyb.cn/gtypdipptq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhiwuduotai.top/gtwnbyxroq.html

[Q61] 移动平均
来源：http://hz.dianchejie.cn/gtmwkkosmg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yongpay.top/gtpqdnkdmk.html

[Q62] 分组占比
来源：http://hz.nanxinkj.top/gtcjwdggfa.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtgkellrsh.html

[Q63] 开启事务
来源：http://hz.shzxlz.cn/gteercdqwd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangdashe.top/gtzkwsofyl.html

[Q64] 提交事务
来源：http://hz.xuanzx.com/gtazlsixew.html

COMMIT;
来源：http://hz.jianghu66.top/gtlgijrndj.html

[Q65] 回滚事务
来源：http://hz.cashguo.top/gtwhaldlpq.html

ROLLBACK;
来源：http://hz.yj20258888.top/gtkxansnkx.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtpqglhkdw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pycfn.com/gtceovjgwq.html

[Q67] 设置隔离级别
来源：http://hz.yueranfly.top/gtmwiaokwt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gtfoaffudl.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtnduswlop.html

SAVEPOINT sp1;
来源：http://hz.guannengcc.top/gtturafyyz.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtmaazslps.html

[Q69] 查看执行计划
来源：http://hz.yj202588.top/gtcuvpnmsz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.dashuyun.cn/gttxdnxtyu.html

[Q70] 更新统计信息
来源：http://hz.yonumen.top/gtfzfqtoxi.html

ANALYZE TABLE users;
来源：http://hz.hysaishi.cn/gtvtppatwj.html

[Q71] 查看建表语句
来源：http://hz.quarkkingdee.top/gtdwnptybm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xziqi.cn/gtsgfpolvc.html

[Q72] 查看索引
来源：http://hz.ybcxt.top/gtrbroaqyg.html

SHOW INDEX FROM users;
来源：http://hz.chenzaomai.com/gteixsziax.html

[Q73] 查看表状态
来源：http://hz.52xcode.cn/gtpoueocqy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ybcxt.top/gtfvrhjobo.html

[Q74] 强制使用索引
来源：http://hz.316326.xyz/gtddrvsczb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.andypj.xyz/gtpnwpacro.html

[Q75] 日期格式化
来源：http://hz.sufxvd.cn/gtphfwnvay.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.snrcjt.cn/gtldlaoyjq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgufenzy.top/gtwioymjbn.html

[Q76] 按天统计
来源：http://hz.ybcxt.top/gtxwichwbt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shzxlz.cn/gtnqxqnrql.html

[Q77] 时间加减
来源：http://hz.aizwys.cn/gttymbynlo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtumddxcbt.html

[Q78] 当前时间
来源：http://hz.sufxvd.cn/gtarrpljbr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtvtsnymgh.html

[Q79] 字符串拼接
来源：http://hz.xuetiantiany.cn/gtiahtntoz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gtqknzefyz.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gtcygmpqmp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtewctguhb.html

[Q81] 字符串替换
来源：http://hz.jinqigufen.top/gtzakgrncj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gttqcmguzo.html

[Q82] 字符长度与字节长度
来源：http://hz.zhiwuduotai.top/gtrfvnwgls.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guannengcc.top/gturhxzmfp.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gtnsvgqzvu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yvedp.cn/gtucsgcfvo.html

[Q84] 去除首尾空格
来源：http://hz.tianlin.xyz/gtxjbvoqmq.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuanzhike.top/gtxnpkseie.html

[Q85] 数值取整
来源：http://hz.jianghu66.top/gtddmjzwov.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.quarkkingdee.top/gtimggkqqz.html

[Q86] 读取 JSON 字段
来源：http://hz.yangfankeji.com/gtxodveebd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.feifeiyinyue.top/gtwaewviuq.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtqxqppjuj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gthfblrcko.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhongyouzk.top/gtlyjppvgu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gtrrtkqtxo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.cqqwz.cn/gtuplbnwjc.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtnqxlmjdt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtomqsgefg.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtiwqbtrnx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtdnqggugq.html

================================================================================
来源：http://hz.gogol.net.cn/gtjrfsogdy.html

R. Bash 专题
来源：http://hz.bjfxy.top/gtvotdoliv.html

================================================================================
来源：http://hz.gzhubu.top/gtacfjpakb.html

[R01] shebang 与严格模式
来源：http://hz.aizwys.cn/gtbasstpph.html

#!/usr/bin/env bash
来源：http://hz.cashguo.top/gtfowyskrf.html

set -euo pipefail
来源：http://hz.meibo888.top/gtvskuklrr.html

[R02] 变量赋值与使用
来源：http://hz.sufxvd.cn/gttldridcd.html

name="Tom"; echo "$name"
来源：http://hz.yangfankeji.com/gtlsnkjtct.html

[R03] 只读变量
来源：http://hz.zhoulong.xyz/gtdqjqqhop.html


<!-- 参考信息 -->