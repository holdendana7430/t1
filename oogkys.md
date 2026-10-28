代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yvedp.cn/gtxohjfvgb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yongpay.top/gtiomspqfh.html

Ruby: threads.map(&:join)
来源：http://hz.haohaochexian.top/gtmshvgedv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tanke756.top/gtujmrlmfa.html

[O06] 使用进程池
来源：http://hz.vqdsnc.cn/gtlfbshicg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hongshengwenyu.top/gtwftkqnts.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangdashe.top/gtmsawztto.html

JS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtvmzfedio.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtxfflmvmz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gtorydtxdq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenjidiqi.icu/gtdgwwfzst.html

Ruby: // fork 块
来源：http://hz.jinghuilouyu.cn/gttzmxhnsl.html

C#:   Parallel.For
来源：http://hz.nwbrower.top/gtdjdmnuqg.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtlsaolunz.html

P. 常用工具函数
来源：http://hz.pengpengdd.cyou/gtwzmzooxm.html

================================================================================
来源：http://hz.smart0.xyz/gtzehjnzws.html

[P01] 生成 UUID
来源：http://hz.sxryk.cn/gtzfvgymye.html

Py:   str(uuid.uuid4())
来源：http://hz.havefunace.top/gtxhozocml.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.meibo888.top/gtdzlbaggz.html

JS:   crypto.randomUUID()
来源：http://hz.jlsjyb.cn/gtzxznsnut.html

TS:   crypto.randomUUID()
来源：http://hz.yvedp.cn/gtbiblrlun.html

Java: UUID.randomUUID().toString()
来源：http://hz.jlsjyb.cn/gtqpqazbij.html

Go:   // 用 github.com/google/uuid
来源：http://hz.c1oappe.top/gtftczxlpl.html

Ruby: SecureRandom.uuid
来源：http://hz.dianchejie.cn/gtygksarnt.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydzc1.top/gtisnrexjy.html

[P02] MD5 / SHA256 摘要
来源：http://hz.meibo888.top/gtyakweyem.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tianlin.xyz/gtgatuiqvr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.gaohongyu789.top/gtutphwpqj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtbujzyejh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yongpay.top/gtwidhpagw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yuxming.cn/gtyvtvkgvv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fengsongda.top/gtkzayrzpm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.wangshuangyany.cn/gthpzltbrp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.vqdsnc.cn/gttgwkcznt.html

[P03] 生成短随机字符串
来源：http://hz.meibo888.top/gtmficqxob.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtptnklpto.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.316326.xyz/gtetlltfdf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hfpthk.cn/gtjijrjtap.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.c1oappe.top/gtccfewzkz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xingfuxueyuan.xyz/gtvceykiof.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jinghuilouyu.cn/gtcgjopghd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zdqjudy.top/gtkmyhlsoz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.316326.xyz/gtdcxivbmu.html

[P04] 求长度
来源：http://hz.zycfv.cn/gtchkjwfed.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.nanxuanxn.top/gtdycmpuhd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtfulrilyf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.vqdsnc.cn/gthunduprv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ydjk.org.cn/gtgkqegspd.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtllszxgiw.html

Go:   len(arr);  len(m)
来源：http://hz.jinghuilouyu.cn/gtvtdcfjlb.html

Ruby: x.length;  x.size
来源：http://hz.jianghu66.top/gtnldbqvlo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hfpthk.cn/gtcosivfzj.html

[P05] 判断两个对象内容是否相等
来源：http://hz.kuanghao11.cn/gtrhszonrh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cheryme.top/gtggmvpria.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shuidangran.top/gtkisdicln.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gtlqyypkzf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgufenzy.top/gtrfcnfdvk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinqigufen.top/gtzbfzqcpp.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.gaohongyu789.top/gtjjxbcfmu.html

Ruby: a == b
来源：http://hz.ehwqpu.com/gthasoywwk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.gaohongyu789.top/gtlzkkgygc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.xylfe.cn/gtpnmjftsi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.haohaochexian.top/gtuffzpmsz.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtfqkuksvf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.havefunace.top/gtmrvhsgin.html

TS:   if (x == null) {}
来源：http://hz.zdqjudy.top/gtglwkjxkh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.daxiang520.top/gtuwoamlzg.html

Go:   if x == nil {}
来源：http://hz.chenlongwang.top/gtzghllebc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.feifeiyinyue.top/gtdzswqkxd.html

C#:   if (x is null) {}
来源：http://hz.yvedp.cn/gtnjvcczkj.html

[P07] 防抖与节流
来源：http://hz.yangfankeji.com/gtdlfzwyek.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ywan-chungtsiang.top/gtuejqdaii.html

PHP:  // 手写时间戳比较
来源：http://hz.ppjwa.cn/gtlwasvekc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtfmtkqvsd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.bjfxy.top/gtfvdqtzmc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.bjfxy.top/gturthbndv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.haohaochexian.top/gtzobvtdas.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.zhijiandao.cn/gthjfqdrkk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhongyouzk.top/gtqshwyvvv.html

[P08] 处理浮点精度问题
来源：http://hz.tanke756.top/gtszotkxvs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.zycfv.cn/gtefgzqbrt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ivvv.top/gtckcfvpbx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.jinqigufen.top/gtokgkzxuk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xziqi.cn/gtnfzonmyc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.jinqigfzy.top/gtmvairgjl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.guowangkeji.top/gtypyqegae.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.shanyushiyangtech.top/gtejgpapfv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.pycfn.com/gtclelbgam.html

================================================================================
来源：http://hz.tanke756.top/gtdnbagois.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.fengsongda.top/gtzytkcuid.html

================================================================================
来源：http://hz.jqgufenzy.top/gtskmvdgrg.html

[Q01] 创建表
来源：http://hz.chenzaomai.com/gtqqmnlufc.html

CREATE TABLE users (
来源：http://hz.hywenlv.cn/gtclsyovmw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.meibo888.top/gtwhmjqjqw.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yanxiufei.cn/gtcarvdwul.html

email VARCHAR(100) UNIQUE,
来源：http://hz.hnqzz.top/gtvxgckxpi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.aizwys.cn/gtgprdgepw.html

);
来源：http://hz.chenjidiqi.icu/gtjplkqbir.html

[Q02] 创建带外键的表
来源：http://hz.hammf.cn/gtcbwqeduo.html

CREATE TABLE orders (
来源：http://hz.zhongyouzk.top/gtshbfevkc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nwbrower.top/gtxcdysbxp.html

user_id INT NOT NULL,
来源：http://hz.nanxinkj.top/gtqaqvdhns.html

amount DECIMAL(10, 2),
来源：http://hz.quarkkingdee.top/gtjmxoxuog.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.c1oappe.top/gtkbdddorv.html

);
来源：http://hz.hywenlv.cn/gtdlqzuolu.html

[Q03] 增加列
来源：http://hz.smart0.xyz/gttaodvjdc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.jqgfzy.top/gtdkkjoqtj.html

[Q04] 修改列类型
来源：http://hz.cdnleiting.top/gtsbplicfv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.jinyuanbaomall.cn/gtgglyrmbf.html

[Q05] 重命名列
来源：http://hz.316326.xyz/gtexeensov.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daria6918.cn/gtttfexnyo.html

[Q06] 删除列
来源：http://hz.nwbrower.top/gtbcfvoaet.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.sweek.top/gtusluyydk.html

[Q07] 删除表
来源：http://hz.cdnleiting.top/gtbzssvqbe.html

DROP TABLE IF EXISTS orders;
来源：http://hz.tianlin.xyz/gtvrdhvmgf.html

[Q08] 创建普通索引
来源：http://hz.fengsongda.top/gtwsxzcqhz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtyknywowq.html

[Q09] 创建唯一索引
来源：http://hz.sxryk.cn/gtrrnsewxf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cqqwz.cn/gtdhkkuraa.html

[Q10] 插入单行
来源：http://hz.chenzaomai.com/gtmiqtdshq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.ppjwa.cn/gtehahdclt.html

[Q11] 一次插入多行
来源：http://hz.xylfe.cn/gtsyfhzdwp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ybcxt.top/gtmnesxgyg.html

[Q12] 插入后取自增 ID
来源：http://hz.yanxiufei.cn/gtwgrwiyri.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.daria6918.cn/gtkgyhwtli.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.xuanzx.com/gtcmpxavsa.html

[Q13] 忽略重复插入
来源：http://hz.xingfuxueyuan.xyz/gternchekb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gtlaidlguc.html

[Q14] 存在则更新（upsert）
来源：http://hz.xinyue.icu/gtjklamyrg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.smart0.xyz/gtgybgncar.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.kuanghao11.cn/gtyccxqlif.html

[Q15] 查询全部
来源：http://hz.nwbrower.top/gtjmpjwmmn.html

SELECT * FROM users;
来源：http://hz.nanxinkj.top/gtgcmgtbof.html

[Q16] 查询指定列
来源：http://hz.yj20258888.top/gtntjtgfbd.html

SELECT id, name FROM users;
来源：http://hz.xylfe.cn/gtobinjvak.html

[Q17] 条件查询
来源：http://hz.yuxming.cn/gttwdyyxxf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jiagoushi.top/gtqkozmxfx.html

[Q18] 模糊匹配
来源：http://hz.zhijiandao.cn/gtmfrydohx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jqgfzy.top/gtgwtpvbms.html

[Q19] 范围查询
来源：http://hz.yj202588.top/gtxdwmhsbk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtgeuwoghr.html

[Q20] IN 列表
来源：http://hz.52xcode.cn/gtpvrqqzzc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.andypj.xyz/gtuzqzkmjw.html

[Q21] 空值判断
来源：http://hz.cashguo.top/gttfvrgutv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gotoacloud.top/gtdhmekisu.html

[Q22] 排序
来源：http://hz.zhixingplan.top/gtevwpkdxu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.fzhhl.top/gtruiyqqpp.html

[Q23] 分页
来源：http://hz.chenzaomai.com/gtumudgoyv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.aibaodan.cn/gthsplnxjl.html

[Q24] 去重
来源：http://hz.aibaodan.cn/gtxyisaszw.html

SELECT DISTINCT city FROM users;
来源：http://hz.nanxinkj.top/gtdnvnjsci.html

[Q25] 只取前 N 条
来源：http://hz.xuetiantiany.cn/gtsstczwgg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dashuyun.cn/gtyoailzvf.html

[Q26] 计数
来源：http://hz.shanyushiyangtech.top/gtauvqxkci.html

SELECT COUNT(*) FROM users;
来源：http://hz.daria6918.cn/gtykttwtdd.html

[Q27] 条件计数
来源：http://hz.jinqigufen.top/gtdbcboqsu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hnxiangtu.top/gtxegpomjj.html

[Q28] 求和与平均
来源：http://hz.kuanghao11.cn/gttkxkzjku.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dashuyun.cn/gteuzsxgol.html

[Q29] 最大最小值
来源：http://hz.chenjidiqi.icu/gtfbfnvotg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtqpcmbdqb.html

[Q30] 分组统计
来源：http://hz.hnqzz.top/gtrvycdiit.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtqwdenpbd.html

[Q31] 分组后过滤
来源：http://hz.fzhhl.top/gtypinnbev.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.fengsongda.top/gtthfnsuru.html

[Q32] 分组拼接字符串
来源：http://hz.guannengcc.top/gtxaplsyff.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtebonrmbe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.fzhhl.top/gtlkzqbwmu.html

[Q33] 多列分组
来源：http://hz.hywenlv.cn/gtjaodenst.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cheryme.top/gtnnnnphxi.html

[Q34] 每组取第一条
来源：http://hz.svipenyu.cn/gtodbymtko.html

SELECT * FROM (
来源：http://hz.redwolf501.top/gteekcyrnn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guannengcc.top/gtguxpxele.html

) t WHERE rn = 1;
来源：http://hz.snrcjt.cn/gtxhglvbtd.html

[Q35] 内连接
来源：http://hz.daxiang520.top/gtfrdlqqtq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtvedaants.html

[Q36] 左连接
来源：http://hz.bjfxy.top/gtpggluxfp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gttuhdufyb.html

[Q37] 右连接
来源：http://hz.gogol.net.cn/gtvawmivhd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gtzovmewln.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtdkrdxoco.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtbqdsoevh.html

[Q39] 自连接（查上下级）
来源：http://hz.jinqigufen.top/gtryruacms.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hammf.cn/gtzrhhnpei.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.birdmap.top/gtznuiqhzh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yuanzhike.top/gtwjqtmure.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhengqikj.top/gtxdmvznkc.html

[Q41] 多表连接
来源：http://hz.yvedp.cn/gtnezdqftv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.316326.xyz/gtlvkidhys.html

JOIN users u ON u.id = o.user_id
来源：http://hz.iojbl.cn/gtpfdojkyg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj202588.top/gtnzaqezkl.html

[Q42] 连接条件附加过滤
来源：http://hz.ydzc1.top/gtmrjttfhh.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gtdbmrwhcx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gotoacloud.top/gtrpywnkff.html

[Q43] 标量子查询
来源：http://hz.jianghu66.top/gtcwkcrrvl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.smart0.xyz/gttqcyrjjh.html

[Q44] IN 子查询
来源：http://hz.chenzaomai.com/gtajeoojrh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yueranfly.top/gtmeywrvad.html

[Q45] EXISTS 判断存在
来源：http://hz.ydzc1.top/gtxglryxvv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xingfuxueyuan.xyz/gtxwklmkvd.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.andypj.xyz/gtvfkjiajv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fzhhl.top/gtofiefdnm.html

[Q47] 与平均值比较
来源：http://hz.yj20258.top/gtldlyieqn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gotoacloud.top/gtkskkeaxb.html

[Q48] CTE 公用表表达式
来源：http://hz.xuetiantiany.cn/gtgiibozcl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.daria6918.cn/gtlwkldigu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shzxlz.cn/gtdxunffon.html

[Q49] 更新单行
来源：http://hz.jyoumei.cn/gtzcsxdbvx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xinyue.icu/gtvlnwcpfv.html

[Q50] 批量更新
来源：http://hz.birdmap.top/gtbaofxnvv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yangfankeji.com/gttoerammm.html

[Q51] 用子查询更新
来源：http://hz.feifeiyinyue.top/gtlwwhlgwd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gttvnodhkb.html

[Q52] 删除指定行
来源：http://hz.yonumen.top/gtbtcmwszv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tian-w.cn/gtvgdnkvcx.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gtemcowoag.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xinyue.icu/gtbwvilecv.html

[Q54] 清空表
来源：http://hz.redwolf501.top/gtpicyycqb.html

TRUNCATE TABLE logs;
来源：http://hz.bjfxy.top/gtbzmrwbyu.html

[Q55] 排名（并列占位）
来源：http://hz.sxryk.cn/gtwzavibrd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangtech.top/gttjfeyvek.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shangyingyoupin.top/gtxowdvmfq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhengqikj.top/gtzicwmzcb.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gtoyhuymdf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yueranfly.top/gthjuitnta.html

[Q58] 累计求和
来源：http://hz.yj20258.top/gtofyuyipy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jinghuilouyu.cn/gtvgllingn.html

[Q59] 分组内累计
来源：http://hz.zhijiandao.cn/gtcbibfcsg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.wangshuangyany.cn/gtcgtivrhy.html

[Q60] 取上一行 / 下一行
来源：http://hz.fengsongda.top/gtplsygdbo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.aizwys.cn/gtietmhwum.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.daria6918.cn/gtdpxzxxdn.html

[Q61] 移动平均
来源：http://hz.iojbl.cn/gtknrrliax.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.9152youxi.cn/gtfctirwpa.html

[Q62] 分组占比
来源：http://hz.feifeiyinyue.top/gtffiwopyn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtjwfsujob.html

[Q63] 开启事务
来源：http://hz.daria6918.cn/gtsagalxue.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xziqi.cn/gtxtbcoslk.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtdlkauqaa.html

COMMIT;
来源：http://hz.aibaodan.cn/gtckkpdwkr.html

[Q65] 回滚事务
来源：http://hz.fzhhl.top/gtbxrznyuz.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gtmiyrqixm.html

[Q66] 行锁查询
来源：http://hz.tian-w.cn/gtjviccest.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtqtlebnvo.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtafmczeqm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xingfuxueyuan.xyz/gtrealnpvs.html

[Q68] 保存点
来源：http://hz.jiagoushi.top/gtcaxbupqr.html

SAVEPOINT sp1;
来源：http://hz.xingfuxueyuan.xyz/gtgwwlpdcx.html

ROLLBACK TO sp1;
来源：http://hz.wangshuangyany.cn/gtscwckygx.html

[Q69] 查看执行计划
来源：http://hz.jyoumei.cn/gtrzvgcqec.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jlsjyb.cn/gtutkeamvp.html

[Q70] 更新统计信息
来源：http://hz.sysykeji.top/gthvckgnqt.html

ANALYZE TABLE users;
来源：http://hz.zhixingplan.top/gtfvenwoix.html

[Q71] 查看建表语句
来源：http://hz.pycfn.com/gtorzmdwpr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.andypj.xyz/gtzrbyjman.html

[Q72] 查看索引
来源：http://hz.tianlin.xyz/gtwwpqqjzo.html

SHOW INDEX FROM users;
来源：http://hz.tianlin.xyz/gtwwjkcwei.html

[Q73] 查看表状态
来源：http://hz.zhixingplan.top/gtupcstapz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.redwolf501.top/gtsczzrwbj.html

[Q74] 强制使用索引
来源：http://hz.dashuyun.cn/gtakzvbgoo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gaohongyu789.top/gtdkxpxdex.html

[Q75] 日期格式化
来源：http://hz.zhongyouzk.top/gtpsmkazpp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jianghu66.top/gtzvsxdddt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guannengcc.top/gtxoysyvqu.html

[Q76] 按天统计
来源：http://hz.hfpthk.cn/gtnjjogoar.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tianlin.xyz/gtubksoojf.html

[Q77] 时间加减
来源：http://hz.hywenlv.cn/gtjygfjhgo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fzhhl.top/gtuhroeyrq.html

[Q78] 当前时间
来源：http://hz.bjfxy.top/gtkbvvhsjn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj202588.top/gtyomsfrmk.html

[Q79] 字符串拼接
来源：http://hz.jinghuilouyu.cn/gtbeeqnaak.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hysaishi.cn/gtycfsdvmm.html

[Q80] 字符串截取
来源：http://hz.ydzc1.top/gtdxuuuwzw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenlongwang.top/gtdfxaxgkp.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtempunidu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtrzezofyy.html

[Q82] 字符长度与字节长度
来源：http://hz.hywenlv.cn/gtwrlldayj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhijiandao.cn/gtwqlopwgc.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtjdrxgpcm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gtitnoeprg.html

[Q84] 去除首尾空格
来源：http://hz.daria6918.cn/gtclyjagwt.html

SELECT TRIM(name) FROM users;
来源：http://hz.svipenyu.cn/gtqcpudrut.html

[Q85] 数值取整
来源：http://hz.ppjwa.cn/gtvhaorbyd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ywan-chungtsiang.top/gtzfakkedf.html

[Q86] 读取 JSON 字段
来源：http://hz.chenlongwang.top/gthgfujwbd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tian-w.cn/gtdcbfxjfc.html

[Q87] JSON 字段做条件
来源：http://hz.yuanzhike.top/gtyxgldqqn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtzaesuhze.html

[Q88] 行转列（条件聚合）
来源：http://hz.cheryme.top/gtpacolvnt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.fengsongda.top/gtldaevwrw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yuxming.cn/gtdvtruwkg.html

[Q89] 判断表是否存在
来源：http://hz.zhixingplan.top/gtfboqwfer.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtqmnalili.html

[Q90] 生成序号列
来源：http://hz.hysaishi.cn/gtpegdfwdm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.gzhubu.top/gtwkjzunlk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtzoefobgi.html

R. Bash 专题
来源：http://hz.316326.xyz/gttiylnroz.html

================================================================================
来源：http://hz.birdmap.top/gtiqpujcnx.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtjkfywqut.html

#!/usr/bin/env bash
来源：http://hz.dianchejie.cn/gtvonbwfkk.html


<!-- 参考信息 -->