代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.daria6918.cn/gtdchydhsx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yangfankeji.com/gtleezdbse.html

Ruby: threads.map(&:join)
来源：http://hz.zhixingplan.top/gtswbhpxgv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hywenlv.cn/gtixyofgov.html

[O06] 使用进程池
来源：http://hz.zhoulong.xyz/gtqlkbnjyy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hongshengwenyu.top/gtdynesfaa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ppjwa.cn/gtwaoazxia.html

JS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtuvhfopid.html

TS:   // child_process / cluster 模块
来源：http://hz.zhiwuduotai.top/gtobapdxlc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.wangshuangyany.cn/gtzhhrusua.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhoulong.xyz/gtalxevnjy.html

Ruby: // fork 块
来源：http://hz.kuanghao11.cn/gtgnzkmrdb.html

C#:   Parallel.For
来源：http://hz.hysaishi.cn/gtaqeqvolz.html

================================================================================
来源：http://hz.jiagoushi.top/gtoysesdbg.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtskldblia.html

================================================================================
来源：http://hz.mhx1999.top/gtrtkvvyoj.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtqnmfzdba.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangkeji.top/gttngzhrow.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ywan-chungtsiang.top/gtvpbbhqcu.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtyumyyjyk.html

TS:   crypto.randomUUID()
来源：http://hz.havefunace.top/gtkxdtruwh.html

Java: UUID.randomUUID().toString()
来源：http://hz.cqqwz.cn/gttbqtdnjs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhaomingkeji.xyz/gtgrezgbax.html

Ruby: SecureRandom.uuid
来源：http://hz.mhx1999.top/gtnkqkbfbv.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtdkunrnsh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.shanyushiyangtech.top/gtxpliratr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xziqi.cn/gtuwmmdczu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.iojbl.cn/gtvimycpzm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj20258.top/gtbxvaztdz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.sufxvd.cn/gtwwrzhtpu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.birdmap.top/gtvcsalpqo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.fzhhl.top/gtijjzbrvp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.smart0.xyz/gticxxyisg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.redwolf501.top/gtexuvunxl.html

[P03] 生成短随机字符串
来源：http://hz.cqqwz.cn/gtpvokqzmj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.meibo888.top/gtxopfpakw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hammf.cn/gtzbabicax.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.feifeiyinyue.top/gtmixqtgyv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cucudq.cn/gtlfqptaps.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.haohaochexian.top/gtoeqrxkba.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gtusmhxwrt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxuanxn.top/gtfbuxvmqd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yuxming.cn/gtlqhbdyos.html

[P04] 求长度
来源：http://hz.yuxming.cn/gtffljsyjk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hysaishi.cn/gtihnxjrdb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtrlgyjauu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hnxiangtu.top/gtqsdajhng.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtsualyuem.html

Java: list.size();  map.size();  s.length()
来源：http://hz.jinqigufen.top/gttjbmhzfi.html

Go:   len(arr);  len(m)
来源：http://hz.shanyushiyangkeji.top/gthjkauiyu.html

Ruby: x.length;  x.size
来源：http://hz.hongshengwenyu.top/gtcfzfmwwo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shanyushiyangtech.top/gtrvmymfct.html

[P05] 判断两个对象内容是否相等
来源：http://hz.c1oappe.top/gtcdbujinb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.jianghu66.top/gtwihjungu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zhijiandao.cn/gtopfeqvqm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.ybcxt.top/gtgzsxwejt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtuhljnefp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cucudq.cn/gtcpohtudd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jiagoushi.top/gtzfsnnjfo.html

Ruby: a == b
来源：http://hz.xingfuxueyuan.xyz/gtsjnmxain.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.daxiang520.top/gtyazwvycr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.c1oappe.top/gtghcehlry.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.mhx1999.top/gtuirbveaq.html

PHP:  if (empty($x)) {}
来源：http://hz.birdmap.top/gtkikvpdgg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.guowangkeji.top/gtysncdwzq.html

TS:   if (x == null) {}
来源：http://hz.haohaochexian.top/gtrjgmqapt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtlyvuteti.html

Go:   if x == nil {}
来源：http://hz.zhiwuduotai.top/gtmwbdylbx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtgpqgienq.html

C#:   if (x is null) {}
来源：http://hz.sysykeji.top/gttjrmeqlw.html

[P07] 防抖与节流
来源：http://hz.nwbrower.top/gtubcqnczz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.yuxming.cn/gtnvkkosmx.html

PHP:  // 手写时间戳比较
来源：http://hz.yuxming.cn/gtydrgjefx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtaayfluol.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ivvv.top/gttfeglsey.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.ivvv.top/gtprprtyqx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.jiagoushi.top/gtuvylxeoi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.c1oappe.top/gtwkrjsrvd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.yuanzhike.top/gtxvjwbulz.html

[P08] 处理浮点精度问题
来源：http://hz.zhijiandao.cn/gtwrgicneq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jyoumei.cn/gtmjdelmnt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258888.top/gtcyfavlmv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.redwolf501.top/gtagtuitqq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.mhx1999.top/gtyzmyjlxh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.ydjk.org.cn/gthoeolcxq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.wangdashe.top/gtdyieahie.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.yj20258888.top/gtnwmqptfh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hywenlv.cn/gtncgiifye.html

================================================================================
来源：http://hz.aibaodan.cn/gthbmvwmlb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.ydzc1.top/gtzpongeiy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtaoxpkjag.html

[Q01] 创建表
来源：http://hz.ybcxt.top/gtrkdiyvna.html

CREATE TABLE users (
来源：http://hz.jinghuilouyu.cn/gtswmffxme.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.jiagoushi.top/gtcclzywec.html

name VARCHAR(50) NOT NULL,
来源：http://hz.hysaishi.cn/gtkqigwmir.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yuxming.cn/gtjeupcyjm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.shzxlz.cn/gtvdrztmkq.html

);
来源：http://hz.fzhhl.top/gtkakgtdzb.html

[Q02] 创建带外键的表
来源：http://hz.yuanzhike.top/gtjqkkooxo.html

CREATE TABLE orders (
来源：http://hz.aibaodan.cn/gtrhqcxpgc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.haohaochexian.top/gtvclsxsuk.html

user_id INT NOT NULL,
来源：http://hz.xuetiantiany.cn/gtfcozbrxg.html

amount DECIMAL(10, 2),
来源：http://hz.cucudq.cn/gtshnvmfrp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.fzhhl.top/gttmtpmilm.html

);
来源：http://hz.shanyushiyangkeji.top/gthwvzvqjs.html

[Q03] 增加列
来源：http://hz.hywenlv.cn/gtlxxtrtvo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yueranfly.top/gthovrbzzn.html

[Q04] 修改列类型
来源：http://hz.ivvv.top/gttspsplbc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gthsmqtibo.html

[Q05] 重命名列
来源：http://hz.ppjwa.cn/gtmzkogqug.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.wangshuangyany.cn/gtvcnevuwk.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtskaxduti.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.cqqwz.cn/gtayesbwyp.html

[Q07] 删除表
来源：http://hz.zhijiandao.cn/gtyaowcfwt.html

DROP TABLE IF EXISTS orders;
来源：http://hz.xziqi.cn/gtqammtgwr.html

[Q08] 创建普通索引
来源：http://hz.shangyingyoupin.top/gtkdfwyjdf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.52xcode.cn/gtsrrcawqx.html

[Q09] 创建唯一索引
来源：http://hz.jinyuanbaomall.cn/gtppzjoelc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yj20258888.top/gtwjnrjbxe.html

[Q10] 插入单行
来源：http://hz.ppjwa.cn/gtigoziyeb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.jqgufenzy.top/gtzeclzqrn.html

[Q11] 一次插入多行
来源：http://hz.yuxming.cn/gteiudkfby.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.nanxinkj.top/gtgstdrddb.html

[Q12] 插入后取自增 ID
来源：http://hz.andypj.xyz/gttzibkios.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cheryme.top/gtdexxfwsd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yongpay.top/gtsfqsnuex.html

[Q13] 忽略重复插入
来源：http://hz.bjfxy.top/gtwqudbgwx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.sufxvd.cn/gtlyldbwog.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhongyouzk.top/gtyiapjiul.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jyoumei.cn/gtevtajint.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.feifeiyinyue.top/gtzkubzlem.html

[Q15] 查询全部
来源：http://hz.hywenlv.cn/gtlvhizrnt.html

SELECT * FROM users;
来源：http://hz.yongpay.top/gtvweinsvb.html

[Q16] 查询指定列
来源：http://hz.yangfankeji.com/gtapynomih.html

SELECT id, name FROM users;
来源：http://hz.shangyingyoupin.top/gtszafswwt.html

[Q17] 条件查询
来源：http://hz.guowangkeji.top/gtoceypwqk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xziqi.cn/gtskfjwyuu.html

[Q18] 模糊匹配
来源：http://hz.9152youxi.cn/gtzodrubwd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cheryme.top/gtjgaaeqsw.html

[Q19] 范围查询
来源：http://hz.bjfxy.top/gtrgwagpyp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.chenzaomai.com/gtoqawpmed.html

[Q20] IN 列表
来源：http://hz.shanyushiyangtech.top/gthgjtsibv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hongshengwenyu.top/gttrsaseol.html

[Q21] 空值判断
来源：http://hz.sufxvd.cn/gtxlpupbyr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinqigufen.top/gtalyvzhbs.html

[Q22] 排序
来源：http://hz.gotoacloud.top/gtiwadbrxq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.quarkkingdee.top/gtamvxzcjp.html

[Q23] 分页
来源：http://hz.gaohongyu789.top/gtgevatnvb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gteiudrdcs.html

[Q24] 去重
来源：http://hz.52xcode.cn/gtzybtekjz.html

SELECT DISTINCT city FROM users;
来源：http://hz.hysaishi.cn/gtnzqxhbuz.html

[Q25] 只取前 N 条
来源：http://hz.9152youxi.cn/gtpnaprtmc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jlsjyb.cn/gtpdqvubuy.html

[Q26] 计数
来源：http://hz.hywenlv.cn/gtlkgexyev.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtpmhicpnh.html

[Q27] 条件计数
来源：http://hz.sxryk.cn/gttxdnxeyc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.bjfxy.top/gtefxejfem.html

[Q28] 求和与平均
来源：http://hz.mhx1999.top/gttesblqsm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jqgufenzy.top/gtpyoachbw.html

[Q29] 最大最小值
来源：http://hz.jinghuilouyu.cn/gtmwrgtrjx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.birdmap.top/gtgnlpchfr.html

[Q30] 分组统计
来源：http://hz.xziqi.cn/gtvnpppgko.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtgncdfgbg.html

[Q31] 分组后过滤
来源：http://hz.zhijiandao.cn/gtgpedgktl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.316326.xyz/gtsrypueoe.html

[Q32] 分组拼接字符串
来源：http://hz.shangyingyoupin.top/gtgxklihyd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtvqvzvbzk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangtech.top/gtwkiulpuf.html

[Q33] 多列分组
来源：http://hz.bjfxy.top/gtgjhrllac.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtgmdkqvpa.html

[Q34] 每组取第一条
来源：http://hz.zdqjudy.top/gtxbstbjdb.html

SELECT * FROM (
来源：http://hz.jinqigufen.top/gtdpjaxjrl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xylfe.cn/gtldejkenw.html

) t WHERE rn = 1;
来源：http://hz.chenlongwang.top/gtrkqqioii.html

[Q35] 内连接
来源：http://hz.yanxiufei.cn/gtmkulrymk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.fengsongda.top/gtxpesknjp.html

[Q36] 左连接
来源：http://hz.feifeiyinyue.top/gtskwgbjqw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtbqezawrn.html

[Q37] 右连接
来源：http://hz.ydzc1.top/gtsxmqkoaw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gaohongyu789.top/gtvepjguze.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.redwolf501.top/gttomxyzrp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtazeslqix.html

[Q39] 自连接（查上下级）
来源：http://hz.fzhhl.top/gtqlmfytnq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hywenlv.cn/gtdjlfmyvk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gteikaeuoe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tanke756.top/gtobcutghb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jlsjyb.cn/gtugduslle.html

[Q41] 多表连接
来源：http://hz.zhongyouzk.top/gtqfbavgim.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hammf.cn/gtfdjdigdc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jyoumei.cn/gtpkmzmxht.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.chenjidiqi.icu/gtapmbcudb.html

[Q42] 连接条件附加过滤
来源：http://hz.jinghuilouyu.cn/gtmixhtgwn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.tianlin.xyz/gthwsjouqz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.wangshuangyany.cn/gtnefvppoj.html

[Q43] 标量子查询
来源：http://hz.daxiang520.top/gteikkkxju.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xziqi.cn/gteuhfalsy.html

[Q44] IN 子查询
来源：http://hz.redwolf501.top/gtkmnaazww.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj202588.top/gtodfeehgr.html

[Q45] EXISTS 判断存在
来源：http://hz.birdmap.top/gtuogahcwj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangkeji.top/gtahmaupzj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ywan-chungtsiang.top/gtalkhtpbs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtaatnhksx.html

[Q47] 与平均值比较
来源：http://hz.wangdashe.top/gtkviufejn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hnxiangtu.top/gtmiftmvxp.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gtwumqygun.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtsmrezfjs.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydzc1.top/gtwebmtboh.html

[Q49] 更新单行
来源：http://hz.shzxlz.cn/gtatmdraxu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hysaishi.cn/gtuatwdglv.html

[Q50] 批量更新
来源：http://hz.zhongyouzk.top/gtkukcejnw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ppjwa.cn/gtfiblhtck.html

[Q51] 用子查询更新
来源：http://hz.gotoacloud.top/gtbvfbtqga.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.mhx1999.top/gtxybetfat.html

[Q52] 删除指定行
来源：http://hz.guowangkeji.top/gtlwlammjc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtvomzbequ.html

[Q53] 按条件删除
来源：http://hz.dianchejie.cn/gtrulanwuj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgufenzy.top/gtpjrpcfyl.html

[Q54] 清空表
来源：http://hz.shanyushiyangtech.top/gtjojblceg.html

TRUNCATE TABLE logs;
来源：http://hz.ivvv.top/gtesuyvwjc.html

[Q55] 排名（并列占位）
来源：http://hz.sysykeji.top/gtbubsgcve.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuxming.cn/gtcezldzvc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hongshengwenyu.top/gtbkymwcvd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.bjfxy.top/gtrrvzqnvq.html

[Q57] 行号
来源：http://hz.jiagoushi.top/gtjiuzfumu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ybcxt.top/gtfhwujwqo.html

[Q58] 累计求和
来源：http://hz.zhoulong.xyz/gtuprjsohj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenzaomai.com/gtlqtgnsxr.html

[Q59] 分组内累计
来源：http://hz.yanxiufei.cn/gtirvirgdg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gtajtzllbo.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinyuanbaomall.cn/gtsueaprez.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhongyouzk.top/gtwhpeuuby.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.chenzaomai.com/gtdutvufcg.html

[Q61] 移动平均
来源：http://hz.hysaishi.cn/gtzjqnmmxv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.316326.xyz/gtkkdptdgo.html

[Q62] 分组占比
来源：http://hz.zhixingplan.top/gtebfqlgdn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tian-w.cn/gtgfzvpjqz.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtzrlllfhi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtpkrvxgzv.html

[Q64] 提交事务
来源：http://hz.hfpthk.cn/gtvezvmoby.html

COMMIT;
来源：http://hz.jinyuanbaomall.cn/gtmqfeomer.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtkrgiuqlq.html

ROLLBACK;
来源：http://hz.quarkkingdee.top/gtceyrcncv.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtyeozoukg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhoulong.xyz/gtvddofzxj.html

[Q67] 设置隔离级别
来源：http://hz.fzhhl.top/gtzqyvjrml.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gogol.net.cn/gtjpuqtdcy.html

[Q68] 保存点
来源：http://hz.shanyushiyangtech.top/gteojjvdpo.html

SAVEPOINT sp1;
来源：http://hz.bjfxy.top/gtclmfvjqv.html

ROLLBACK TO sp1;
来源：http://hz.yongpay.top/gtolbtabtn.html

[Q69] 查看执行计划
来源：http://hz.gogol.net.cn/gtaupjwhxt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.redwolf501.top/gtigrvyvzx.html

[Q70] 更新统计信息
来源：http://hz.xinyue.icu/gtbvrywzqo.html

ANALYZE TABLE users;
来源：http://hz.haohaochexian.top/gtetweezkw.html

[Q71] 查看建表语句
来源：http://hz.zhongyouzk.top/gtosvxjuib.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtgdbrfckf.html

[Q72] 查看索引
来源：http://hz.ybcxt.top/gthleomcbq.html

SHOW INDEX FROM users;
来源：http://hz.jqgfzy.top/gtabrdkilo.html

[Q73] 查看表状态
来源：http://hz.tanke756.top/gtnngmndmj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pengpengdd.cyou/gtyvojjnan.html

[Q74] 强制使用索引
来源：http://hz.redwolf501.top/gttikmojrl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.bjfxy.top/gtnshepwyx.html

[Q75] 日期格式化
来源：http://hz.cdnleiting.top/gtbnwpcryf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj202588.top/gtnkddtpvg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sxryk.cn/gtypdmiwpo.html

[Q76] 按天统计
来源：http://hz.zhengqikj.top/gthjqcozqo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigufen.top/gtnqmbojta.html

[Q77] 时间加减
来源：http://hz.hnqzz.top/gtpyvquyfk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.wangshuangyany.cn/gtkffhlnvz.html

[Q78] 当前时间
来源：http://hz.sysykeji.top/gttigzwuzd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gttovhzmeo.html

[Q79] 字符串拼接
来源：http://hz.birdmap.top/gtqvinzide.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.snrcjt.cn/gthijefqfp.html

[Q80] 字符串截取
来源：http://hz.feifeiyinyue.top/gtruoasspi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gogol.net.cn/gtfoctcwhb.html

[Q81] 字符串替换
来源：http://hz.xingfuxueyuan.xyz/gtlkxcuqmi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinyuanbaomall.cn/gtavnhlqzp.html

[Q82] 字符长度与字节长度
来源：http://hz.cashguo.top/gtbagzumdd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.daria6918.cn/gtmcijatjr.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtcffrxntu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydzc1.top/gtegfwitbd.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtbicgeyuz.html

SELECT TRIM(name) FROM users;
来源：http://hz.sufxvd.cn/gtncdvanxi.html

[Q85] 数值取整
来源：http://hz.sxryk.cn/gtrfcqsbnl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.smart0.xyz/gtduhyuefp.html

[Q86] 读取 JSON 字段
来源：http://hz.52xcode.cn/gtqnfxdeir.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.havefunace.top/gtkqaaidtc.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangtech.top/gtakwcjqhx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xylfe.cn/gtgsqydvax.html

[Q88] 行转列（条件聚合）
来源：http://hz.shangyingyoupin.top/gtfnpxuabq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.c1oappe.top/gtmmdwuqtc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenzaomai.com/gtwrwvaofn.html

[Q89] 判断表是否存在
来源：http://hz.fzhhl.top/gtxxahzzhh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj202588.top/gtvhsnyfsv.html

[Q90] 生成序号列
来源：http://hz.shzxlz.cn/gttyebmcdf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtagveznlj.html

================================================================================
来源：http://hz.daxiang520.top/gtzbuvrfxc.html

R. Bash 专题
来源：http://hz.yj202588.top/gtfmayjluv.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjanuzlee.html

[R01] shebang 与严格模式
来源：http://hz.jiagoushi.top/gtarhpttqe.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gttiiiztnb.html


<!-- 参考信息 -->