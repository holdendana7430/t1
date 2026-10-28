代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cqqwz.cn/gtwgykuowt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gotoacloud.top/gtuxkrbhqb.html

C#:   async Task F() { await G(); }
来源：http://hz.dianchejie.cn/gtksaxtijz.html

[O05] 并发执行并等待全部完成
来源：http://hz.xinyue.icu/gtyadxxsjm.html

Py:   asyncio.gather(*tasks)
来源：http://hz.0kj1m.cn/gtpfupoorw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yuxming.cn/gtscdcmuwk.html

JS:   await Promise.all(tasks)
来源：http://hz.aibaodan.cn/gtqtihqljs.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgfzy.top/gtndlwbhsa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangkeji.top/gtyxvycyji.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yvedp.cn/gtgxzknfxf.html

Ruby: threads.map(&:join)
来源：http://hz.guowangkeji.top/gtqptkixat.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.chenjidiqi.icu/gtjolibhti.html

[O06] 使用进程池
来源：http://hz.iojbl.cn/gtgvugrctg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj202588.top/gtphgoqnbd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.aizwys.cn/gtterzjwfr.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtcxzstjpk.html

TS:   // child_process / cluster 模块
来源：http://hz.ydzc1.top/gtekumpcxc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.svipenyu.cn/gtsvnfmvvu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gtwldwttwd.html

Ruby: // fork 块
来源：http://hz.yj20258888.top/gtcybjtyni.html

C#:   Parallel.For
来源：http://hz.vqdsnc.cn/gtlmfpaftd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtewhhjmcd.html

P. 常用工具函数
来源：http://hz.shuidangran.top/gtfpsgdnst.html

================================================================================
来源：http://hz.yangfankeji.com/gtljruveye.html

[P01] 生成 UUID
来源：http://hz.xylfe.cn/gtvwufynav.html

Py:   str(uuid.uuid4())
来源：http://hz.dashuyun.cn/gtixxkazhi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yj202588.top/gtdkzynrxc.html

JS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtekuppnlb.html

TS:   crypto.randomUUID()
来源：http://hz.yongpay.top/gtknxudqhu.html

Java: UUID.randomUUID().toString()
来源：http://hz.svipenyu.cn/gtydzrdxqm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xingfuxueyuan.xyz/gtbrigulgj.html

Ruby: SecureRandom.uuid
来源：http://hz.wangdashe.top/gtjxkfbqmc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cdnleiting.top/gtitmekuqg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.birdmap.top/gtlccuohjq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hnxiangtu.top/gtolkixhwu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shanyushiyangtech.top/gtwpgedbtg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtukbuxnmp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gtkjlljqwl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.smart0.xyz/gttaswxlfk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xuetiantiany.cn/gtbcmwnqom.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.vqdsnc.cn/gtnpauypbp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.sweek.top/gtujjfjmcg.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gtieqnyvlc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aibaodan.cn/gtnyceddhl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.ivvv.top/gtijjkokdl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtjhiigxsn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtlumthtmi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.nwbrower.top/gtpxnnznsw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.zhiwuduotai.top/gtpxqqmarr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.guannengcc.top/gthhnqehvb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.cqqwz.cn/gtdxbjuiln.html

[P04] 求长度
来源：http://hz.zhengqikj.top/gtvlwidnnu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zdqjudy.top/gtvfzodttc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtrwhbmehm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.pengpengdd.cyou/gtuudeyqfi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.feifeiyinyue.top/gtybtczxxr.html

Java: list.size();  map.size();  s.length()
来源：http://hz.zhiwuduotai.top/gtfwosvsie.html

Go:   len(arr);  len(m)
来源：http://hz.xingfuxueyuan.xyz/gtqcocsmxq.html

Ruby: x.length;  x.size
来源：http://hz.quarkkingdee.top/gtopenizws.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.cqqwz.cn/gtlgdvcafu.html

[P05] 判断两个对象内容是否相等
来源：http://hz.quarkkingdee.top/gtzqosuped.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.kuanghao11.cn/gtxtguwpaw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.c1oappe.top/gtipyqbogj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.jqgufenzy.top/gttzotizbs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangkeji.top/gtekneaczt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.316326.xyz/gtypaloddk.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.havefunace.top/gtpqqjdcpf.html

Ruby: a == b
来源：http://hz.gaohongyu789.top/gtnbgxbnee.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.redwolf501.top/gtlklwweid.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.andypj.xyz/gtpcmoxqtz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.cdnleiting.top/gtvurpisug.html

PHP:  if (empty($x)) {}
来源：http://hz.wangdashe.top/gtoawdlyuf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.xziqi.cn/gtvdiubkbp.html

TS:   if (x == null) {}
来源：http://hz.jinghuilouyu.cn/gtpkghetlz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.sxryk.cn/gtljghhpvm.html

Go:   if x == nil {}
来源：http://hz.yangfankeji.com/gtluxjhvva.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.meibo888.top/gtfdpiqupc.html

C#:   if (x is null) {}
来源：http://hz.sufxvd.cn/gtanobmttu.html

[P07] 防抖与节流
来源：http://hz.xuanzx.com/gtvvgrpbxz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.zhoulong.xyz/gtngdtghtq.html

PHP:  // 手写时间戳比较
来源：http://hz.zhaomingkeji.xyz/gtnhstethe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtypxespad.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtucqyiiwt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.9152youxi.cn/gtyxjpkfdh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fengsongda.top/gtkupuwmfp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258888.top/gtlqqxfvel.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhiwuduotai.top/gtvwrefrfu.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gtuyhtsyok.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.wangdashe.top/gtvisqgvgx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.ydjk.org.cn/gtigyvxgul.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtlkalfwep.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.zycfv.cn/gtuyubimlo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.kuanghao11.cn/gtqefxmbyk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.chenjidiqi.icu/gtcsgtmrue.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.jinqigufen.top/gtnqsxzqjo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhaomingkeji.xyz/gtasnoyxdk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzqrgbpbe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yj20258.top/gtuxxmkdhl.html

================================================================================
来源：http://hz.mhx1999.top/gttjmqotsf.html

[Q01] 创建表
来源：http://hz.shzxlz.cn/gtxbgexnig.html

CREATE TABLE users (
来源：http://hz.jqgufenzy.top/gtjeehrczp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxuanxn.top/gthshxboks.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yanxiufei.cn/gtuovoaopp.html

email VARCHAR(100) UNIQUE,
来源：http://hz.cdnleiting.top/gttmxahmvv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.kuanghao11.cn/gtzimggdvc.html

);
来源：http://hz.quarkkingdee.top/gtimzzkmbr.html

[Q02] 创建带外键的表
来源：http://hz.yvedp.cn/gtldsywjer.html

CREATE TABLE orders (
来源：http://hz.svipenyu.cn/gtnhqbdgjx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtsnyvlegm.html

user_id INT NOT NULL,
来源：http://hz.pycfn.com/gtrtzarwvz.html

amount DECIMAL(10, 2),
来源：http://hz.jlsjyb.cn/gtzdulnotp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yueranfly.top/gtfzqmzmsy.html

);
来源：http://hz.shangyingyoupin.top/gthaofobdx.html

[Q03] 增加列
来源：http://hz.ivvv.top/gtpaidfnlb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.yongpay.top/gtqwvbeqsk.html

[Q04] 修改列类型
来源：http://hz.c1oappe.top/gtpxgmfugs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.yuxming.cn/gtzjtaasgy.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtvomcdnum.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.cdnleiting.top/gtarweebuu.html

[Q06] 删除列
来源：http://hz.yuanzhike.top/gtikzetmvr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj202588.top/gtqjhihavo.html

[Q07] 删除表
来源：http://hz.guowangkeji.top/gtyflgqibg.html

DROP TABLE IF EXISTS orders;
来源：http://hz.gotoacloud.top/gtmqprcexw.html

[Q08] 创建普通索引
来源：http://hz.jiagoushi.top/gtlkysylnt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shanyushiyangkeji.top/gtjnkngmbl.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gtsgbtxidr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cucudq.cn/gthikcivvw.html

[Q10] 插入单行
来源：http://hz.ppjwa.cn/gtubfpxxgt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.zdqjudy.top/gtghzmbxgq.html

[Q11] 一次插入多行
来源：http://hz.zhengqikj.top/gtzkjgkalu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ydzc1.top/gtyfjdajbi.html

[Q12] 插入后取自增 ID
来源：http://hz.zdqjudy.top/gtrwmsxdzm.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinyuanbaomall.cn/gtgnzagacs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.gotoacloud.top/gtsulxmyll.html

[Q13] 忽略重复插入
来源：http://hz.vqdsnc.cn/gtkhhpcuhi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gaohongyu789.top/gtrjcxytdq.html

[Q14] 存在则更新（upsert）
来源：http://hz.shzxlz.cn/gtzydkzudz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.feifeiyinyue.top/gtuwrwzvav.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cqqwz.cn/gtpeklwhva.html

[Q15] 查询全部
来源：http://hz.jiagoushi.top/gtqntboprd.html

SELECT * FROM users;
来源：http://hz.jianghu66.top/gtlwqwrbsz.html

[Q16] 查询指定列
来源：http://hz.hnxiangtu.top/gtbkpiaypn.html

SELECT id, name FROM users;
来源：http://hz.cqqwz.cn/gtzguaylsg.html

[Q17] 条件查询
来源：http://hz.dashuyun.cn/gttugmvfap.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.nanxuanxn.top/gtutseggxm.html

[Q18] 模糊匹配
来源：http://hz.zdqjudy.top/gtydxdyqfa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cashguo.top/gtcfwzkcai.html

[Q19] 范围查询
来源：http://hz.pengpengdd.cyou/gtriglpdpx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigufen.top/gtbzdchnit.html

[Q20] IN 列表
来源：http://hz.ywan-chungtsiang.top/gtogmpgdjp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gtdfftvhlb.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtrfivisju.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.zhengqikj.top/gtlphuezyh.html

[Q22] 排序
来源：http://hz.jinqigfzy.top/gtfbcrwxen.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tianlin.xyz/gtghoidnfp.html

[Q23] 分页
来源：http://hz.hywenlv.cn/gtsajmnoxc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jianghu66.top/gtfuqnsslg.html

[Q24] 去重
来源：http://hz.ppjwa.cn/gtssagvpqf.html

SELECT DISTINCT city FROM users;
来源：http://hz.sufxvd.cn/gtrfbkhijw.html

[Q25] 只取前 N 条
来源：http://hz.sufxvd.cn/gtwsyyhjai.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtqryufvid.html

[Q26] 计数
来源：http://hz.cqqwz.cn/gtrmwuydrl.html

SELECT COUNT(*) FROM users;
来源：http://hz.ivvv.top/gtqqxaqtqm.html

[Q27] 条件计数
来源：http://hz.cucudq.cn/gtxkudoqct.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.sysykeji.top/gtsksxgdon.html

[Q28] 求和与平均
来源：http://hz.tanke756.top/gtkheyqthz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.redwolf501.top/gthaswulwz.html

[Q29] 最大最小值
来源：http://hz.shzxlz.cn/gtldiqtaan.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhiwuduotai.top/gthqaghtsy.html

[Q30] 分组统计
来源：http://hz.guowangkeji.top/gteklkfdxs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtzbsejkkr.html

[Q31] 分组后过滤
来源：http://hz.smart0.xyz/gtsavskxzw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.vqdsnc.cn/gtqatluayh.html

[Q32] 分组拼接字符串
来源：http://hz.sweek.top/gthiyszrri.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtscqtnjrt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinqigufen.top/gtnwxndksd.html

[Q33] 多列分组
来源：http://hz.daxiang520.top/gtacaulwsm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.snrcjt.cn/gttmwsnmqy.html

[Q34] 每组取第一条
来源：http://hz.daxiang520.top/gtenbvakhb.html

SELECT * FROM (
来源：http://hz.kuanghao11.cn/gtunijtkrx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yvedp.cn/gtmyhymfuw.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gtxftbjqjb.html

[Q35] 内连接
来源：http://hz.sweek.top/gtsuhtaynl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gotoacloud.top/gttxdjgifx.html

[Q36] 左连接
来源：http://hz.ydjk.org.cn/gtmiwhkfhe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.aibaodan.cn/gtcqtombml.html

[Q37] 右连接
来源：http://hz.smart0.xyz/gtsrpbgufy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtspjsoeoa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yueranfly.top/gtkjahobob.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ivvv.top/gtzrnssokg.html

[Q39] 自连接（查上下级）
来源：http://hz.jqgfzy.top/gtotxgnmez.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ybcxt.top/gtjjxyzlwf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cucudq.cn/gtbqlryxcu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhaomingkeji.xyz/gttswfkvpv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gogol.net.cn/gtpnbkpehk.html

[Q41] 多表连接
来源：http://hz.yj20258.top/gtehpawmme.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnxiangtu.top/gtwceranir.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hywenlv.cn/gtjgjvpceo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sweek.top/gtvlszfkhk.html

[Q42] 连接条件附加过滤
来源：http://hz.wangdashe.top/gtillaxpuq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.andypj.xyz/gtjpxbnboq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.zycfv.cn/gtllrrgrcg.html

[Q43] 标量子查询
来源：http://hz.daxiang520.top/gtghtbynur.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ydjk.org.cn/gtmtufvlyr.html

[Q44] IN 子查询
来源：http://hz.smart0.xyz/gtktjqkjud.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.havefunace.top/gtkwoynvrd.html

[Q45] EXISTS 判断存在
来源：http://hz.shuidangran.top/gtzxqydgjh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zycfv.cn/gtiyzwgvqn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jlsjyb.cn/gtecudbvuc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtitclaevj.html

[Q47] 与平均值比较
来源：http://hz.cucudq.cn/gtlrpgwluu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258888.top/gtidkudcjn.html

[Q48] CTE 公用表表达式
来源：http://hz.wangshuangyany.cn/gtrdunexbi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gtrezggwip.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtsejjhdxo.html

[Q49] 更新单行
来源：http://hz.tanke756.top/gtqmrmgxgb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dianchejie.cn/gtfaqjrdbv.html

[Q50] 批量更新
来源：http://hz.wangdashe.top/gtywhyllox.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.tian-w.cn/gtkhghujnn.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtygohhoig.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtcqnfjjip.html

[Q52] 删除指定行
来源：http://hz.sxryk.cn/gttswibmbi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jqgfzy.top/gtdmtubczw.html

[Q53] 按条件删除
来源：http://hz.snrcjt.cn/gtdxduxgyv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.c1oappe.top/gtzxmwmutr.html

[Q54] 清空表
来源：http://hz.yj202588.top/gtzqioaqtc.html

TRUNCATE TABLE logs;
来源：http://hz.jinyuanbaomall.cn/gtnoelmxzw.html

[Q55] 排名（并列占位）
来源：http://hz.zhaomingkeji.xyz/gtgwqdoiyp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jqgufenzy.top/gtuortjmaq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtqryjbtvz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aizwys.cn/gtxezbxnmp.html

[Q57] 行号
来源：http://hz.xingfuxueyuan.xyz/gtczrlmqvt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yongpay.top/gtfkktohsu.html

[Q58] 累计求和
来源：http://hz.aizwys.cn/gtxmfybmir.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.haohaochexian.top/gtqgkvsdum.html

[Q59] 分组内累计
来源：http://hz.feifeiyinyue.top/gtnnlqdqch.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj202588.top/gtetozcqwk.html

[Q60] 取上一行 / 下一行
来源：http://hz.yueranfly.top/gtibanuihg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenzaomai.com/gtzyprvraw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pengpengdd.cyou/gtkeshhnpv.html

[Q61] 移动平均
来源：http://hz.sweek.top/gtligsyjfc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuanzx.com/gtplhhzbzn.html

[Q62] 分组占比
来源：http://hz.iojbl.cn/gtdfvuonnz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.haohaochexian.top/gteoajxkga.html

[Q63] 开启事务
来源：http://hz.pengpengdd.cyou/gtkuefmieh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ywan-chungtsiang.top/gtlmdppmrc.html

[Q64] 提交事务
来源：http://hz.jinyuanbaomall.cn/gtwaujwbjp.html

COMMIT;
来源：http://hz.xuetiantiany.cn/gtxaycmrem.html

[Q65] 回滚事务
来源：http://hz.wangdashe.top/gtvecljwjl.html

ROLLBACK;
来源：http://hz.chenjidiqi.icu/gtcptrqesc.html

[Q66] 行锁查询
来源：http://hz.hnqzz.top/gtremkntzo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.9152youxi.cn/gtlhthyjmr.html

[Q67] 设置隔离级别
来源：http://hz.ydzc1.top/gtbvvppdpg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ywan-chungtsiang.top/gtcdexikzz.html

[Q68] 保存点
来源：http://hz.zycfv.cn/gthogxybdu.html

SAVEPOINT sp1;
来源：http://hz.ivvv.top/gtkwpbilmd.html

ROLLBACK TO sp1;
来源：http://hz.aizwys.cn/gtmkbuljym.html

[Q69] 查看执行计划
来源：http://hz.ydjk.org.cn/gtnnqwvzlj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtxclsfitf.html

[Q70] 更新统计信息
来源：http://hz.cheryme.top/gtsxsgpaqq.html

ANALYZE TABLE users;
来源：http://hz.hongshengwenyu.top/gthsftjjhd.html

[Q71] 查看建表语句
来源：http://hz.0kj1m.cn/gtdexbonjy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gzhubu.top/gtfmmonwsp.html

[Q72] 查看索引
来源：http://hz.fengsongda.top/gtqrsfvmlf.html

SHOW INDEX FROM users;
来源：http://hz.ydjk.org.cn/gtndvsmmyb.html

[Q73] 查看表状态
来源：http://hz.jinqigufen.top/gtcipklmxf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.smart0.xyz/gtrlnqrlbj.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtzrbgaqtw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.iojbl.cn/gtbausqfxg.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtvhycyzxw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtgbdavyth.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gtqfgjupnq.html

[Q76] 按天统计
来源：http://hz.zhaomingkeji.xyz/gtjinvkalm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenjidiqi.icu/gtagewpvpo.html

[Q77] 时间加减
来源：http://hz.sysykeji.top/gtytmpjncf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.feifeiyinyue.top/gtjkhvqazj.html

[Q78] 当前时间
来源：http://hz.xingfuxueyuan.xyz/gtbnwziucn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tian-w.cn/gtsrpnjhka.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtimbocnhx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhoulong.xyz/gtbyfkvlok.html

[Q80] 字符串截取
来源：http://hz.guannengcc.top/gthpijspta.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtlxkrrluo.html

[Q81] 字符串替换
来源：http://hz.xuetiantiany.cn/gtlsgmyrzq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ppjwa.cn/gtxtjluvyz.html

[Q82] 字符长度与字节长度
来源：http://hz.hammf.cn/gttllagogz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgufenzy.top/gtavwmenqa.html

[Q83] 大小写转换
来源：http://hz.hongshengwenyu.top/gtgbbbdkah.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gtxzspschw.html

[Q84] 去除首尾空格
来源：http://hz.tanke756.top/gtbdnbepbq.html

SELECT TRIM(name) FROM users;
来源：http://hz.xziqi.cn/gthtwcnqbh.html

[Q85] 数值取整
来源：http://hz.daxiang520.top/gtwbcuxybl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gtsaillaai.html

[Q86] 读取 JSON 字段
来源：http://hz.yj20258.top/gtsknblrbw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tian-w.cn/gtfaspaxol.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtjcltaecv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aibaodan.cn/gthetnwohg.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangdashe.top/gtqfbjeftk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.redwolf501.top/gtoikudnfn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtlwahumrw.html

[Q89] 判断表是否存在
来源：http://hz.chenzaomai.com/gtjmbpowam.html


<!-- 参考信息 -->