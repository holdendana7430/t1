代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hysaishi.cn/gtjcsidqir.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shzxlz.cn/gtrmbhidbn.html

Ruby: threads.map(&:join)
来源：http://hz.meibo888.top/gtdcbxjnrf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhengqikj.top/gtaiwmmyzq.html

[O06] 使用进程池
来源：http://hz.yvedp.cn/gtqommtmun.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gzhubu.top/gtytjhgyja.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ydjk.org.cn/gtndxivxfh.html

JS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gtqgmfivuh.html

TS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtwngrbaex.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.meibo888.top/gthglxevhw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gotoacloud.top/gtkvqcetak.html

Ruby: // fork 块
来源：http://hz.9152youxi.cn/gtziwlsoka.html

C#:   Parallel.For
来源：http://hz.guannengcc.top/gtazrlwxzl.html

================================================================================
来源：http://hz.gogol.net.cn/gtlbyitxhq.html

P. 常用工具函数
来源：http://hz.tian-w.cn/gtdisqvghf.html

================================================================================
来源：http://hz.tianlin.xyz/gtikbxykkq.html

[P01] 生成 UUID
来源：http://hz.pengpengdd.cyou/gtfojzszct.html

Py:   str(uuid.uuid4())
来源：http://hz.zhoulong.xyz/gtrdtdaikq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hfpthk.cn/gtrzbvbbdd.html

JS:   crypto.randomUUID()
来源：http://hz.daria6918.cn/gtzyaayfao.html

TS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gthzltzhlp.html

Java: UUID.randomUUID().toString()
来源：http://hz.havefunace.top/gtpvwdigcp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shanyushiyangtech.top/gtylxkpscv.html

Ruby: SecureRandom.uuid
来源：http://hz.yonumen.top/gtxoyljtps.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinghuilouyu.cn/gtwevpjcae.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sxryk.cn/gtaauqvisq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yuanzhike.top/gtfqnhhbgp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.tanke756.top/gtbqyqyacm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tianlin.xyz/gtlpkofamf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydzc1.top/gtztraxbtn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258888.top/gtktckisac.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zycfv.cn/gtgxshsdzl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnqzz.top/gtzjshcizp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sufxvd.cn/gtdsrelcvm.html

[P03] 生成短随机字符串
来源：http://hz.sxryk.cn/gtyygcgjai.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shanyushiyangtech.top/gtydwnxinf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.bjfxy.top/gtjfcteitr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258888.top/gtshmuuqpk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtgbjcysms.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gzhubu.top/gtjeeauumc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.gaohongyu789.top/gtirmcgpuf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.chenjidiqi.icu/gtreicwrui.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cashguo.top/gtrrfhvkqm.html

[P04] 求长度
来源：http://hz.chenzaomai.com/gtvkicqkep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.jinghuilouyu.cn/gtcnrbqnco.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pycfn.com/gtahwlrubz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hfpthk.cn/gtdnkfohpb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.wangdashe.top/gtthdygocn.html

Java: list.size();  map.size();  s.length()
来源：http://hz.cucudq.cn/gtwfzfgdlg.html

Go:   len(arr);  len(m)
来源：http://hz.jinqigfzy.top/gteqkhjxab.html

Ruby: x.length;  x.size
来源：http://hz.wangdashe.top/gtsfswwsex.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.quarkkingdee.top/gtodecxczl.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ybcxt.top/gtadtdlkii.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.smart0.xyz/gthgvnewgb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhixingplan.top/gtocxromee.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hnxiangtu.top/gtkklzinhh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtlqzozcqq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.chenlongwang.top/gtpavaspmw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.aizwys.cn/gtovsmpmfr.html

Ruby: a == b
来源：http://hz.nwbrower.top/gtkfwvthds.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.shanyushiyangtech.top/gtbioypngo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxuanxn.top/gtxpcvzwhx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.nanxinkj.top/gtkfjomfnc.html

PHP:  if (empty($x)) {}
来源：http://hz.chenjidiqi.icu/gtwmjjltgk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.chenzaomai.com/gtscotpkkw.html

TS:   if (x == null) {}
来源：http://hz.yj20258.top/gtqnnblntv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.bjfxy.top/gtmfrjqcwu.html

Go:   if x == nil {}
来源：http://hz.ywan-chungtsiang.top/gtpowuwxic.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.redwolf501.top/gtauhplgor.html

C#:   if (x is null) {}
来源：http://hz.cdnleiting.top/gtphkmwviw.html

[P07] 防抖与节流
来源：http://hz.ppjwa.cn/gtegwetdku.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.shanyushiyangkeji.top/gteflcdont.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtazyyxoad.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtlmdikhbv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtgccnqhrc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.shzxlz.cn/gtdtutigmj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yvedp.cn/gteveupsmq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yanxiufei.cn/gtlythunpk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.xingfuxueyuan.xyz/gthyfxcwsw.html

[P08] 处理浮点精度问题
来源：http://hz.chenlongwang.top/gtlnnljvqn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.guannengcc.top/gtxsoyjqoz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.cheryme.top/gtzlbhwmfv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.sweek.top/gtefxaepjj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.jqgfzy.top/gtxcjjtzev.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.xziqi.cn/gtacyjksea.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.nanxuanxn.top/gtfaewivph.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.cdnleiting.top/gtgpobtobr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hongshengwenyu.top/gtmqhyziez.html

================================================================================
来源：http://hz.yuxming.cn/gtjecokbgk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.0kj1m.cn/gtrheathdb.html

================================================================================
来源：http://hz.zdqjudy.top/gtnqqqypkn.html

[Q01] 创建表
来源：http://hz.sysykeji.top/gtuzcnntnr.html

CREATE TABLE users (
来源：http://hz.xingfuxueyuan.xyz/gthgddfvhw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gtbgvgppdf.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gtzxzyhfwf.html

email VARCHAR(100) UNIQUE,
来源：http://hz.meibo888.top/gtwqjeknwo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.daxiang520.top/gttixusxpr.html

);
来源：http://hz.yuxming.cn/gtwsglcdlv.html

[Q02] 创建带外键的表
来源：http://hz.dashuyun.cn/gtxabnfpxe.html

CREATE TABLE orders (
来源：http://hz.wangdashe.top/gtscibbbuj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtbspqagqh.html

user_id INT NOT NULL,
来源：http://hz.nwbrower.top/gtntrguops.html

amount DECIMAL(10, 2),
来源：http://hz.fengsongda.top/gtrqduczxl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhiwuduotai.top/gtcaxupzbv.html

);
来源：http://hz.ywan-chungtsiang.top/gtieghehsa.html

[Q03] 增加列
来源：http://hz.ywan-chungtsiang.top/gtnbnrgfyj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangtech.top/gtbmxzxxwp.html

[Q04] 修改列类型
来源：http://hz.yonumen.top/gtvoqazymb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hysaishi.cn/gtksvhxkcc.html

[Q05] 重命名列
来源：http://hz.zhijiandao.cn/gtlpryfhlx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.jinyuanbaomall.cn/gttqsbnqzl.html

[Q06] 删除列
来源：http://hz.wangshuangyany.cn/gtctfsocxz.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.smart0.xyz/gteefamyxi.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtzelbcclg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.jlsjyb.cn/gtnccbwfrl.html

[Q08] 创建普通索引
来源：http://hz.yuanzhike.top/gtokvzzznw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yangfankeji.com/gtfhpwzbnz.html

[Q09] 创建唯一索引
来源：http://hz.zhengqikj.top/gtrgfpecgx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jinghuilouyu.cn/gtvbgnzjki.html

[Q10] 插入单行
来源：http://hz.aizwys.cn/gttlauvryb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.andypj.xyz/gtwzuofnvf.html

[Q11] 一次插入多行
来源：http://hz.chenlongwang.top/gtwkzmvrak.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenzaomai.com/gtoiuxovwn.html

[Q12] 插入后取自增 ID
来源：http://hz.tianlin.xyz/gtboohnnmt.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhengqikj.top/gtvwadjqau.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhijiandao.cn/gtfulwjmkf.html

[Q13] 忽略重复插入
来源：http://hz.shuidangran.top/gtylpndted.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.0kj1m.cn/gtzpidrufr.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhijiandao.cn/gttpitqvad.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.nwbrower.top/gtxzeigyte.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.gzhubu.top/gtuhvsnaab.html

[Q15] 查询全部
来源：http://hz.xingfuxueyuan.xyz/gthgiclgfb.html

SELECT * FROM users;
来源：http://hz.feifeiyinyue.top/gtqfyplvot.html

[Q16] 查询指定列
来源：http://hz.pycfn.com/gtmgitefwc.html

SELECT id, name FROM users;
来源：http://hz.yanxiufei.cn/gtqapefqdk.html

[Q17] 条件查询
来源：http://hz.hammf.cn/gtirhjzaup.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jianghu66.top/gtlyqthebh.html

[Q18] 模糊匹配
来源：http://hz.shangyingyoupin.top/gtgyparroo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jlsjyb.cn/gtwzebmnir.html

[Q19] 范围查询
来源：http://hz.ivvv.top/gtvtiwqmhp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.dashuyun.cn/gtasnayxug.html

[Q20] IN 列表
来源：http://hz.yj20258.top/gtofkmmkoe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ivvv.top/gtxgudhlnb.html

[Q21] 空值判断
来源：http://hz.wangdashe.top/gtdpaodxpo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jlsjyb.cn/gtfilbxmjt.html

[Q22] 排序
来源：http://hz.cheryme.top/gtnduznhti.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.guannengcc.top/gtzfrdjeqg.html

[Q23] 分页
来源：http://hz.zhiwuduotai.top/gtxqcjxcan.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigfzy.top/gtuawvueja.html

[Q24] 去重
来源：http://hz.gaohongyu789.top/gtiwmgxzbk.html

SELECT DISTINCT city FROM users;
来源：http://hz.daria6918.cn/gtdwfanbgn.html

[Q25] 只取前 N 条
来源：http://hz.snrcjt.cn/gtjpmarzbv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuetiantiany.cn/gtoveyfuln.html

[Q26] 计数
来源：http://hz.fengsongda.top/gtgsxqcmyp.html

SELECT COUNT(*) FROM users;
来源：http://hz.jqgfzy.top/gtbvglukje.html

[Q27] 条件计数
来源：http://hz.wangshuangyany.cn/gtndoodicy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nwbrower.top/gtgvgsmejb.html

[Q28] 求和与平均
来源：http://hz.yvedp.cn/gtdfmcvmmi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.nanxuanxn.top/gtsbvizlbw.html

[Q29] 最大最小值
来源：http://hz.jiagoushi.top/gtoczavuwe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtidrbzrhf.html

[Q30] 分组统计
来源：http://hz.hongshengwenyu.top/gtiimaodia.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daxiang520.top/gtluxsvofl.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtfbbabakk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zycfv.cn/gtuqrzgqnk.html

[Q32] 分组拼接字符串
来源：http://hz.sweek.top/gtvpyzgvzq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtvndlydpi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.sweek.top/gtnktykjox.html

[Q33] 多列分组
来源：http://hz.0kj1m.cn/gtqojsiswo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jqgufenzy.top/gtkueyloic.html

[Q34] 每组取第一条
来源：http://hz.hysaishi.cn/gtoncarhyn.html

SELECT * FROM (
来源：http://hz.shuidangran.top/gtdghobmzx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yanxiufei.cn/gtjsbkrcoe.html

) t WHERE rn = 1;
来源：http://hz.jinqigufen.top/gtxlogtfme.html

[Q35] 内连接
来源：http://hz.yuxming.cn/gtinetrwop.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtcpflsiwj.html

[Q36] 左连接
来源：http://hz.yuxming.cn/gtjzdlktko.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtgjtivicx.html

[Q37] 右连接
来源：http://hz.tanke756.top/gthdyaubig.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zhengqikj.top/gttpiqwotg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.9152youxi.cn/gtxgcyfzcb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xuetiantiany.cn/gtdxnqrkes.html

[Q39] 自连接（查上下级）
来源：http://hz.cucudq.cn/gttnavlddm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hammf.cn/gtnxldlnzs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.sweek.top/gtiahpzsys.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydjk.org.cn/gtxzhninzz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yueranfly.top/gtwgfdwvdg.html

[Q41] 多表连接
来源：http://hz.kuanghao11.cn/gtmzxxyczp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.haohaochexian.top/gtisvorcmw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtprxcunat.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jlsjyb.cn/gtifrpkqul.html

[Q42] 连接条件附加过滤
来源：http://hz.aizwys.cn/gtdyqapemz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.guannengcc.top/gteitcswvq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.fzhhl.top/gtsrdrmdfy.html

[Q43] 标量子查询
来源：http://hz.gotoacloud.top/gteauephzz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gtzqkduimp.html

[Q44] IN 子查询
来源：http://hz.tianlin.xyz/gtjvccspty.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guowangkeji.top/gtabbjikmh.html

[Q45] EXISTS 判断存在
来源：http://hz.dashuyun.cn/gtivhrhbma.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnqzz.top/gtnfdezind.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gogol.net.cn/gtwlymayln.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtvdhkouxx.html

[Q47] 与平均值比较
来源：http://hz.gotoacloud.top/gthtoygdjy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.mhx1999.top/gtmkjgawtb.html

[Q48] CTE 公用表表达式
来源：http://hz.52xcode.cn/gteaxswddi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shuidangran.top/gtmyovtbtp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ybcxt.top/gtpfgmaxjb.html

[Q49] 更新单行
来源：http://hz.wangshuangyany.cn/gtzoxsxvpq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.fengsongda.top/gtxbljkyms.html

[Q50] 批量更新
来源：http://hz.kuanghao11.cn/gtyjqekplx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhixingplan.top/gtzpefhrad.html

[Q51] 用子查询更新
来源：http://hz.jinqigufen.top/gtahemizgb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.chenzaomai.com/gtlnwalllo.html

[Q52] 删除指定行
来源：http://hz.daxiang520.top/gtdmspwsyb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.havefunace.top/gtwxsvsqgw.html

[Q53] 按条件删除
来源：http://hz.sufxvd.cn/gtammkebxc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.nanxuanxn.top/gtwtephskn.html

[Q54] 清空表
来源：http://hz.birdmap.top/gtwjazykel.html

TRUNCATE TABLE logs;
来源：http://hz.zhiwuduotai.top/gtmtakzmbi.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtbvklyrom.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.iojbl.cn/gtxoztzlto.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yonumen.top/gtkuwxhxfu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yueranfly.top/gtpibwkrvp.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtexsgqgjt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yuanzhike.top/gtfrzlnifw.html

[Q58] 累计求和
来源：http://hz.andypj.xyz/gtdaiissqo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ybcxt.top/gtzbezpier.html

[Q59] 分组内累计
来源：http://hz.ywan-chungtsiang.top/gtmlruopii.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gtuucijmdx.html

[Q60] 取上一行 / 下一行
来源：http://hz.tanke756.top/gtumuqxqwo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.kuanghao11.cn/gtisinspnk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtaciyyfck.html

[Q61] 移动平均
来源：http://hz.xuetiantiany.cn/gteeqzuoxz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtrglyaeay.html

[Q62] 分组占比
来源：http://hz.0kj1m.cn/gtntogwnpl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.wangdashe.top/gtcutnjbvn.html

[Q63] 开启事务
来源：http://hz.zhoulong.xyz/gtkrblabfu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.0kj1m.cn/gtdpzsemda.html

[Q64] 提交事务
来源：http://hz.zhoulong.xyz/gtmbfiyovz.html

COMMIT;
来源：http://hz.yongpay.top/gtibabrpor.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gtukmelxlw.html

ROLLBACK;
来源：http://hz.chenlongwang.top/gtwfrpuusp.html

[Q66] 行锁查询
来源：http://hz.cheryme.top/gtunjzssct.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gtgxconoya.html

[Q67] 设置隔离级别
来源：http://hz.snrcjt.cn/gtutgqqdfn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gogol.net.cn/gtxpvxdgvu.html

[Q68] 保存点
来源：http://hz.wangdashe.top/gtkklwcwky.html

SAVEPOINT sp1;
来源：http://hz.snrcjt.cn/gtgicyruth.html

ROLLBACK TO sp1;
来源：http://hz.hnqzz.top/gtzasrkqjq.html

[Q69] 查看执行计划
来源：http://hz.haohaochexian.top/gtfxnorwtd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.c1oappe.top/gtibidcyal.html

[Q70] 更新统计信息
来源：http://hz.cashguo.top/gtoylhtopl.html

ANALYZE TABLE users;
来源：http://hz.fengsongda.top/gtfwadccst.html

[Q71] 查看建表语句
来源：http://hz.iojbl.cn/gtfiyxyxka.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shzxlz.cn/gtmknnpojy.html

[Q72] 查看索引
来源：http://hz.bjfxy.top/gtxmjsgmob.html

SHOW INDEX FROM users;
来源：http://hz.feifeiyinyue.top/gtrshmzfxg.html

[Q73] 查看表状态
来源：http://hz.chenzaomai.com/gtfuvkfmvr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.havefunace.top/gtnrbselxr.html

[Q74] 强制使用索引
来源：http://hz.fengsongda.top/gtzpludhbm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtrcmtizar.html

[Q75] 日期格式化
来源：http://hz.wangshuangyany.cn/gtphaafzca.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pycfn.com/gtxgqqhldy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.aibaodan.cn/gthswcelbb.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtadvubkda.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenzaomai.com/gtbvjrbdik.html

[Q77] 时间加减
来源：http://hz.guowangkeji.top/gtnmtqbznp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.9152youxi.cn/gtxawiqfjh.html

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtugbvsdvq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fengsongda.top/gtulahhoru.html

[Q79] 字符串拼接
来源：http://hz.xylfe.cn/gtxwxdjrls.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinyuanbaomall.cn/gtdrbwowuo.html

[Q80] 字符串截取
来源：http://hz.316326.xyz/gtcmcqkbdt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtivtgpzlq.html

[Q81] 字符串替换
来源：http://hz.daxiang520.top/gtjvkgotgm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtqgeahkrj.html

[Q82] 字符长度与字节长度
来源：http://hz.cheryme.top/gtzjkhwoyt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zdqjudy.top/gtghaldtsy.html

[Q83] 大小写转换
来源：http://hz.gaohongyu789.top/gtnwkzpbmy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.redwolf501.top/gtueewxvrb.html

[Q84] 去除首尾空格
来源：http://hz.fengsongda.top/gtsgchdstz.html

SELECT TRIM(name) FROM users;
来源：http://hz.xylfe.cn/gtguivkgry.html

[Q85] 数值取整
来源：http://hz.jiagoushi.top/gtcfzpsqev.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hammf.cn/gtfawtlnie.html

[Q86] 读取 JSON 字段
来源：http://hz.tian-w.cn/gtbaotyykc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.bjfxy.top/gtfadsfwnw.html

[Q87] JSON 字段做条件
来源：http://hz.sweek.top/gtfstwhxks.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.havefunace.top/gtjbuifttp.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtvalfllxo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtpeasjoen.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gtziijyksx.html

[Q89] 判断表是否存在
来源：http://hz.vqdsnc.cn/gtkynsecyt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tanke756.top/gtgeengwjx.html

[Q90] 生成序号列
来源：http://hz.jiagoushi.top/gtqcevuppp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.svipenyu.cn/gtvrhdmsah.html

================================================================================
来源：http://hz.fengsongda.top/gtlgjauncf.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtbljzloip.html

================================================================================
来源：http://hz.jqgufenzy.top/gthjduoqhk.html

[R01] shebang 与严格模式
来源：http://hz.gzhubu.top/gtswsunugd.html

#!/usr/bin/env bash
来源：http://hz.zhoulong.xyz/gtchmgwddr.html


<!-- 参考信息 -->