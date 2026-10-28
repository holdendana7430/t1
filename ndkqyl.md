代发 wailian999

[O06] 使用进程池
来源：http://hz.cucudq.cn/gtzthjwyzt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj202588.top/gtewyqwkqy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shzxlz.cn/gtjrdpgxcn.html

JS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtabdljttx.html

TS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtdfrrrhxh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.svipenyu.cn/gtrwndrhyl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shangyingyoupin.top/gtblkdsbfp.html

Ruby: // fork 块
来源：http://hz.shanyushiyangtech.top/gtckcqhrhv.html

C#:   Parallel.For
来源：http://hz.tanke756.top/gtkcbslgre.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrumhjqih.html

P. 常用工具函数
来源：http://hz.sysykeji.top/gtaibxgiuw.html

================================================================================
来源：http://hz.meibo888.top/gtlmrtynzc.html

[P01] 生成 UUID
来源：http://hz.cqqwz.cn/gthkedzskm.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtmxnqtfdg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigfzy.top/gtgdhsmptb.html

JS:   crypto.randomUUID()
来源：http://hz.svipenyu.cn/gtoriuocit.html

TS:   crypto.randomUUID()
来源：http://hz.jqgfzy.top/gtkukkchgx.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtmohpkesx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hysaishi.cn/gtqtushnon.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtnalsjceo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jlsjyb.cn/gtttjebvde.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yj20258.top/gtveqovitm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yueranfly.top/gtngyingje.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.iojbl.cn/gtdulrnnja.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtrxertiql.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yueranfly.top/gtujezgnef.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.dianchejie.cn/gtswaozffe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guowangkeji.top/gtrzxxmpfx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jiagoushi.top/gthzroaeto.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.tianlin.xyz/gtpdatzqxw.html

[P03] 生成短随机字符串
来源：http://hz.wangshuangyany.cn/gtpkkwhgpm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgufenzy.top/gtbjsjzwzs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangkeji.top/gtargmccxg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtqmzfwinr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.mhx1999.top/gtaurgjrve.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.snrcjt.cn/gtnuetkyia.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.sufxvd.cn/gtejjcvmox.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yuanzhike.top/gtpknregwf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.andypj.xyz/gtovxlfpin.html

[P04] 求长度
来源：http://hz.guowangkeji.top/gtwnxhfjze.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.tanke756.top/gtmzsbceyb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtfafkygzt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.chenzaomai.com/gtgshywyic.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gtyppcjzfq.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhoulong.xyz/gtydwmgnue.html

Go:   len(arr);  len(m)
来源：http://hz.c1oappe.top/gtmhllsxvc.html

Ruby: x.length;  x.size
来源：http://hz.ywan-chungtsiang.top/gtbxecdwxx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.zhoulong.xyz/gtvaqfkciy.html

[P05] 判断两个对象内容是否相等
来源：http://hz.9152youxi.cn/gtrblbwodv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.dianchejie.cn/gttozrghuh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.tianlin.xyz/gtatdmwvqb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhoulong.xyz/gtxyaqrrzk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dianchejie.cn/gtgzmzukii.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.ydjk.org.cn/gtkxboliot.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.daria6918.cn/gtdbvhnvbj.html

Ruby: a == b
来源：http://hz.smart0.xyz/gtnhnhptow.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yanxiufei.cn/gtgpgeadjz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.yj20258.top/gtrrqkqgpb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.feifeiyinyue.top/gtoxogecgy.html

PHP:  if (empty($x)) {}
来源：http://hz.yueranfly.top/gtpeicplwx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.hnxiangtu.top/gtlyfggsom.html

TS:   if (x == null) {}
来源：http://hz.ybcxt.top/gtummogcgb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.pycfn.com/gtjiiwwbcb.html

Go:   if x == nil {}
来源：http://hz.cashguo.top/gticmyxdia.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.jqgfzy.top/gtvxmsmzjd.html

C#:   if (x is null) {}
来源：http://hz.pycfn.com/gtxttdwejt.html

[P07] 防抖与节流
来源：http://hz.quarkkingdee.top/gtgprxalie.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.ehwqpu.com/gtjlxlfhvx.html

PHP:  // 手写时间戳比较
来源：http://hz.zhixingplan.top/gtrmreyhzj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yanxiufei.cn/gtgomjujjb.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.tanke756.top/gtqneeiupj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hfpthk.cn/gtxsewknti.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.hnqzz.top/gtpttwcabw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.guowangkeji.top/gtnkwqfkbb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuxming.cn/gtuwoklsjc.html

[P08] 处理浮点精度问题
来源：http://hz.ydjk.org.cn/gtrirnrmpd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.daxiang520.top/gtlgwookpf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhaomingkeji.xyz/gtijmycwxo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dianchejie.cn/gtgsbxpdms.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gttuntsolu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tian-w.cn/gtspsnmweq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.vqdsnc.cn/gtlsrpqmdq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.zhongyouzk.top/gtpduwvpgq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.sweek.top/gtcbmoahgw.html

================================================================================
来源：http://hz.xuanzx.com/gtgtwcuzah.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhiwuduotai.top/gtxoaeffxh.html

================================================================================
来源：http://hz.gotoacloud.top/gtscpzwwbj.html

[Q01] 创建表
来源：http://hz.smart0.xyz/gthubmiedy.html

CREATE TABLE users (
来源：http://hz.tianlin.xyz/gtzteoaxth.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gttzidnash.html

name VARCHAR(50) NOT NULL,
来源：http://hz.bjfxy.top/gtmdxoaqom.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhiwuduotai.top/gtooabnlwa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jyoumei.cn/gthyvsjecj.html

);
来源：http://hz.vqdsnc.cn/gtwdlzegdo.html

[Q02] 创建带外键的表
来源：http://hz.shuidangran.top/gtzbamrkxl.html

CREATE TABLE orders (
来源：http://hz.dianchejie.cn/gtqqyttnsq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.smart0.xyz/gtidgxgcup.html

user_id INT NOT NULL,
来源：http://hz.hongshengwenyu.top/gtrkmtbtvd.html

amount DECIMAL(10, 2),
来源：http://hz.guowangkeji.top/gtzrxqwscd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhixingplan.top/gtsndqkido.html

);
来源：http://hz.feifeiyinyue.top/gtiuilpwdd.html

[Q03] 增加列
来源：http://hz.jinyuanbaomall.cn/gtcmvyqeeg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.snrcjt.cn/gtlbzwjmvf.html

[Q04] 修改列类型
来源：http://hz.9152youxi.cn/gtfqjycxsm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.snrcjt.cn/gtqzfqqkej.html

[Q05] 重命名列
来源：http://hz.nanxinkj.top/gtresebwxr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cqqwz.cn/gtxewwptsa.html

[Q06] 删除列
来源：http://hz.hammf.cn/gtlwkouhzc.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.xylfe.cn/gtgunqdsrb.html

[Q07] 删除表
来源：http://hz.jinghuilouyu.cn/gtkzplvnqx.html

DROP TABLE IF EXISTS orders;
来源：http://hz.shanyushiyangtech.top/gtynsfkvnf.html

[Q08] 创建普通索引
来源：http://hz.fzhhl.top/gtkrxjwyyh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtmotdkylz.html

[Q09] 创建唯一索引
来源：http://hz.yuanzhike.top/gtltyfrbtw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.jiagoushi.top/gtgcvduenn.html

[Q10] 插入单行
来源：http://hz.zhengqikj.top/gtjlrpmnqv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.snrcjt.cn/gtddxaaxpv.html

[Q11] 一次插入多行
来源：http://hz.xziqi.cn/gthwbyidmy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gotoacloud.top/gtdvcihhlz.html

[Q12] 插入后取自增 ID
来源：http://hz.meibo888.top/gtiamsofgb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.pengpengdd.cyou/gthloiduhr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hongshengwenyu.top/gtiqrynvex.html

[Q13] 忽略重复插入
来源：http://hz.pycfn.com/gtnbmarsgj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jqgfzy.top/gticapwizb.html

[Q14] 存在则更新（upsert）
来源：http://hz.wangshuangyany.cn/gtmkoojtjd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.tanke756.top/gtcprchvml.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zhoulong.xyz/gtknwlomad.html

[Q15] 查询全部
来源：http://hz.tian-w.cn/gtxcuqrsej.html

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gtsqmpqdoo.html

[Q16] 查询指定列
来源：http://hz.jqgfzy.top/gtblztduyn.html

SELECT id, name FROM users;
来源：http://hz.pengpengdd.cyou/gtcyraexnb.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gtvwurosfs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gthmagowps.html

[Q18] 模糊匹配
来源：http://hz.yuxming.cn/gthzblinku.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zycfv.cn/gtvtzyiwjw.html

[Q19] 范围查询
来源：http://hz.xylfe.cn/gtgafxpbpc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhongyouzk.top/gtemiolmfk.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtikylhzqb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dashuyun.cn/gttekphexu.html

[Q21] 空值判断
来源：http://hz.yuxming.cn/gtqdxevjti.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fzhhl.top/gtgmwapuuc.html

[Q22] 排序
来源：http://hz.vqdsnc.cn/gtuwwocbvs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sysykeji.top/gtzfocnzgc.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtfkwvtkku.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.cucudq.cn/gtogwrllbu.html

[Q24] 去重
来源：http://hz.ppjwa.cn/gtpcshmrte.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhongyouzk.top/gtsccgnogf.html

[Q25] 只取前 N 条
来源：http://hz.gogol.net.cn/gtnqfvehmn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gtjovzhebe.html

[Q26] 计数
来源：http://hz.aibaodan.cn/gtgajvzmup.html

SELECT COUNT(*) FROM users;
来源：http://hz.pengpengdd.cyou/gtgpgcrosf.html

[Q27] 条件计数
来源：http://hz.aibaodan.cn/gtnexqkgap.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zhijiandao.cn/gtpptghlxn.html

[Q28] 求和与平均
来源：http://hz.c1oappe.top/gtnltfismz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtsjekrttc.html

[Q29] 最大最小值
来源：http://hz.yj20258.top/gtddvnheyu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj202588.top/gtaroqadcz.html

[Q30] 分组统计
来源：http://hz.chenjidiqi.icu/gtcmogfocw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.dashuyun.cn/gtcxqtdtdd.html

[Q31] 分组后过滤
来源：http://hz.xuetiantiany.cn/gtnwjlmyzn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.iojbl.cn/gtvrdbbqyb.html

[Q32] 分组拼接字符串
来源：http://hz.cucudq.cn/gtjjqhnhqh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtnsenypba.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ywan-chungtsiang.top/gtsovfqobv.html

[Q33] 多列分组
来源：http://hz.zhengqikj.top/gtrkrxdggg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.daria6918.cn/gtiabeqrci.html

[Q34] 每组取第一条
来源：http://hz.aizwys.cn/gtekatkayk.html

SELECT * FROM (
来源：http://hz.yvedp.cn/gtecpryoah.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.bjfxy.top/gtegdzoecx.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtrnmzsxdz.html

[Q35] 内连接
来源：http://hz.fengsongda.top/gtybkfxwro.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jlsjyb.cn/gtgsaxbger.html

[Q36] 左连接
来源：http://hz.shuidangran.top/gtojofvoon.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xylfe.cn/gtbkvhwcmj.html

[Q37] 右连接
来源：http://hz.shanyushiyangtech.top/gttqhwjjmg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jqgfzy.top/gtmyibznxu.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ywan-chungtsiang.top/gtrhvxbhwn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ybcxt.top/gtvepqzwfv.html

[Q39] 自连接（查上下级）
来源：http://hz.guowangkeji.top/gtxryyyokh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhijiandao.cn/gtwaqxoikx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.haohaochexian.top/gthkouncjf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hfpthk.cn/gtptondmus.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydjk.org.cn/gteomdbbtg.html

[Q41] 多表连接
来源：http://hz.jlsjyb.cn/gtzptvxmqm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangkeji.top/gtfhgcqcgj.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhiwuduotai.top/gtosptpiue.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenzaomai.com/gtvcxuyqqy.html

[Q42] 连接条件附加过滤
来源：http://hz.yj20258.top/gtnhfauxuf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daria6918.cn/gturwtdryo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cheryme.top/gtylchrxzq.html

[Q43] 标量子查询
来源：http://hz.ydzc1.top/gtwypddezt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yonumen.top/gtrvmxysky.html

[Q44] IN 子查询
来源：http://hz.c1oappe.top/gtcptcpafz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangtech.top/gtzbderxyh.html

[Q45] EXISTS 判断存在
来源：http://hz.xylfe.cn/gtgyqyvoug.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.wangdashe.top/gttfqrcwtt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj202588.top/gtsshopekv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hammf.cn/gtwfqsnkjq.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtrcavwzlj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.sweek.top/gtzjhbonlj.html

[Q48] CTE 公用表表达式
来源：http://hz.wangdashe.top/gtdkddnsoj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhoulong.xyz/gtgyssjqgz.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nwbrower.top/gtojcepdlw.html

[Q49] 更新单行
来源：http://hz.ywan-chungtsiang.top/gtbgsmuhfb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.xylfe.cn/gtehleqtih.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtrdihzjni.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sweek.top/gtkozvqrjg.html

[Q51] 用子查询更新
来源：http://hz.tanke756.top/gtfjbnzigl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gzhubu.top/gtvpgkzmrd.html

[Q52] 删除指定行
来源：http://hz.gaohongyu789.top/gtewtivpgi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pycfn.com/gtwsrguzkr.html

[Q53] 按条件删除
来源：http://hz.yangfankeji.com/gtakgvwgkm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xziqi.cn/gtqjfrbtsi.html

[Q54] 清空表
来源：http://hz.guowangkeji.top/gthlzlcvqj.html

TRUNCATE TABLE logs;
来源：http://hz.vqdsnc.cn/gtnuyitcgy.html

[Q55] 排名（并列占位）
来源：http://hz.xingfuxueyuan.xyz/gtmtqojpez.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xinyue.icu/gthcwrqpur.html

[Q56] 密集排名（并列不占位）
来源：http://hz.c1oappe.top/gtqyqtfypt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gthiwvztrm.html

[Q57] 行号
来源：http://hz.jinghuilouyu.cn/gtvitxobnd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtnmpazbdf.html

[Q58] 累计求和
来源：http://hz.xziqi.cn/gtfrgvfcwj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sxryk.cn/gtflsotioa.html

[Q59] 分组内累计
来源：http://hz.yonumen.top/gthclzmokx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.birdmap.top/gtkqmyxtmt.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenzaomai.com/gtggzhoxtd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ydzc1.top/gtihhejuka.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.0kj1m.cn/gtzmvizivu.html

[Q61] 移动平均
来源：http://hz.bjfxy.top/gtaczcidjc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.andypj.xyz/gtqvolngci.html

[Q62] 分组占比
来源：http://hz.nanxinkj.top/gtazsoixhy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtvsrcfhvk.html

[Q63] 开启事务
来源：http://hz.sufxvd.cn/gtcvhfpxpc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cdnleiting.top/gtoylihfsz.html

[Q64] 提交事务
来源：http://hz.ehwqpu.com/gtafxxaqgh.html

COMMIT;
来源：http://hz.xuanzx.com/gtajzbztrp.html

[Q65] 回滚事务
来源：http://hz.aizwys.cn/gtwhjzgnvp.html

ROLLBACK;
来源：http://hz.316326.xyz/gtxwvmpjjd.html

[Q66] 行锁查询
来源：http://hz.feifeiyinyue.top/gtkjwffuvz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shanyushiyangtech.top/gtlwumohex.html

[Q67] 设置隔离级别
来源：http://hz.cashguo.top/gthpmcptzf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtzzsnyeoy.html

[Q68] 保存点
来源：http://hz.daria6918.cn/gtypjhrvqm.html

SAVEPOINT sp1;
来源：http://hz.feifeiyinyue.top/gtnzwnscgm.html

ROLLBACK TO sp1;
来源：http://hz.kuanghao11.cn/gteuxmmtos.html

[Q69] 查看执行计划
来源：http://hz.cdnleiting.top/gtkvechtff.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtnefscfuq.html

[Q70] 更新统计信息
来源：http://hz.hysaishi.cn/gtwtausfsb.html

ANALYZE TABLE users;
来源：http://hz.kuanghao11.cn/gtbwwgcogv.html

[Q71] 查看建表语句
来源：http://hz.daria6918.cn/gtzimoackl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.dashuyun.cn/gtthxavnjp.html

[Q72] 查看索引
来源：http://hz.dianchejie.cn/gtqtfoyogj.html

SHOW INDEX FROM users;
来源：http://hz.316326.xyz/gtsigymgue.html

[Q73] 查看表状态
来源：http://hz.hammf.cn/gtyyzbzesj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj202588.top/gtcgvujgzn.html

[Q74] 强制使用索引
来源：http://hz.yanxiufei.cn/gtxvsnruxc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.9152youxi.cn/gtlmxgrysr.html

[Q75] 日期格式化
来源：http://hz.sufxvd.cn/gtbnnaxxze.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.pycfn.com/gteuzpnxjc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tanke756.top/gtvdjqkbah.html

[Q76] 按天统计
来源：http://hz.ybcxt.top/gturhrumok.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gtmduisbsz.html

[Q77] 时间加减
来源：http://hz.aibaodan.cn/gtrjyhaofy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.redwolf501.top/gtfumehrit.html

[Q78] 当前时间
来源：http://hz.sxryk.cn/gtkddnznql.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xziqi.cn/gthoxkekql.html

[Q79] 字符串拼接
来源：http://hz.hysaishi.cn/gtxbbfglav.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.c1oappe.top/gtesumnzav.html

[Q80] 字符串截取
来源：http://hz.zdqjudy.top/gtgeculqcs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuanzx.com/gtnycxefmo.html

[Q81] 字符串替换
来源：http://hz.wangdashe.top/gtlhkclakj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtnhfvscmo.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gtznclgnoo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hnqzz.top/gtuscdzmwc.html

[Q83] 大小写转换
来源：http://hz.shangyingyoupin.top/gttaidzhot.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtljujmjxu.html

[Q84] 去除首尾空格
来源：http://hz.ydzc1.top/gthbovieut.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtboumbkju.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtvwwumfwb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hywenlv.cn/gtavfrdyvc.html

[Q86] 读取 JSON 字段
来源：http://hz.wangdashe.top/gtlwhasfpr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shzxlz.cn/gtysyswkuf.html

[Q87] JSON 字段做条件
来源：http://hz.zhengqikj.top/gtsjbcdoll.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnxiangtu.top/gtkczqsrlo.html

[Q88] 行转列（条件聚合）
来源：http://hz.snrcjt.cn/gtrhywczzn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhoulong.xyz/gtywewkpce.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xuetiantiany.cn/gttvvtkdof.html

[Q89] 判断表是否存在
来源：http://hz.kuanghao11.cn/gtpblxudel.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhijiandao.cn/gtyhcamhrh.html

[Q90] 生成序号列
来源：http://hz.snrcjt.cn/gtkosmmltb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.guannengcc.top/gtvdstsbek.html

================================================================================
来源：http://hz.shzxlz.cn/gtcbwcujhv.html

R. Bash 专题
来源：http://hz.jinyuanbaomall.cn/gteejntiro.html

================================================================================
来源：http://hz.yueranfly.top/gtjjxiwhes.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtcqzuvocu.html

#!/usr/bin/env bash
来源：http://hz.feifeiyinyue.top/gtzcsjeaub.html

set -euo pipefail
来源：http://hz.cqqwz.cn/gtbxgfddih.html

[R02] 变量赋值与使用
来源：http://hz.jianghu66.top/gtyaciyqvz.html

name="Tom"; echo "$name"
来源：http://hz.hfpthk.cn/gtwokwngwv.html

[R03] 只读变量
来源：http://hz.quarkkingdee.top/gtphocvjuz.html


<!-- 参考信息 -->