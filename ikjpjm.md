代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xinyue.icu/gtkgaxzudp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtdxsdisdr.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtonhdnfzh.html

[O05] 并发执行并等待全部完成
来源：http://hz.xinyue.icu/gtklkheiwr.html

Py:   asyncio.gather(*tasks)
来源：http://hz.daxiang520.top/gttsxncjki.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenjidiqi.icu/gtrjiesblt.html

JS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtecfquryy.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtmwfaeoax.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj20258888.top/gtygsnsmuj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ehwqpu.com/gtakpxbscj.html

Ruby: threads.map(&:join)
来源：http://hz.shzxlz.cn/gthgwjzkem.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hnqzz.top/gtgdeqrzbq.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtplltxsjx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.feifeiyinyue.top/gtjouijntk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhongyouzk.top/gtlkkrotny.html

JS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtrgjnlbpd.html

TS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gtnixcmmvo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtbltirhko.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gtununnwyv.html

Ruby: // fork 块
来源：http://hz.zycfv.cn/gtrkarrrdg.html

C#:   Parallel.For
来源：http://hz.0kj1m.cn/gtbhbhhdmx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtghgqgttk.html

P. 常用工具函数
来源：http://hz.yangfankeji.com/gtydilvmrz.html

================================================================================
来源：http://hz.bjfxy.top/gtghommokr.html

[P01] 生成 UUID
来源：http://hz.jianghu66.top/gtizcrlivc.html

Py:   str(uuid.uuid4())
来源：http://hz.yonumen.top/gtitcbxxqj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.chenlongwang.top/gttjkvsyru.html

JS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtidfcdett.html

TS:   crypto.randomUUID()
来源：http://hz.zhoulong.xyz/gtcwhgleme.html

Java: UUID.randomUUID().toString()
来源：http://hz.ehwqpu.com/gttbinpsar.html

Go:   // 用 github.com/google/uuid
来源：http://hz.dianchejie.cn/gtujtrryqd.html

Ruby: SecureRandom.uuid
来源：http://hz.sxryk.cn/gtzwtrutqc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.sweek.top/gtqnprjtdj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sufxvd.cn/gtvfejuazv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.birdmap.top/gtwdrjqlci.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ppjwa.cn/gtoowujlun.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yueranfly.top/gtcqovhhse.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnxiangtu.top/gtgaaxdflj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jqgufenzy.top/gttqzrrfcx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jlsjyb.cn/gtbkobuayb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.xinyue.icu/gtsqgmddwd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.fengsongda.top/gtkjyrvnsu.html

[P03] 生成短随机字符串
来源：http://hz.yuxming.cn/gtkbdhwmnv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.wangshuangyany.cn/gturcehxiz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.hnxiangtu.top/gtfnsjoixd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jqgfzy.top/gtdnjztnnn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gaohongyu789.top/gtypyeccrx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gogol.net.cn/gtwhibgewj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.pengpengdd.cyou/gtdohlwpax.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.pengpengdd.cyou/gtklxuvkoi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jqgufenzy.top/gtroanrbpj.html

[P04] 求长度
来源：http://hz.fzhhl.top/gtinbxcgzg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.guannengcc.top/gtwgyjkuha.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtqutlnyip.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.mhx1999.top/gtzsshlsra.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gtznyfmycl.html

Java: list.size();  map.size();  s.length()
来源：http://hz.tianlin.xyz/gtvsggvear.html

Go:   len(arr);  len(m)
来源：http://hz.hongshengwenyu.top/gtaelcptzh.html

Ruby: x.length;  x.size
来源：http://hz.aizwys.cn/gtoyagtxfg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.shangyingyoupin.top/gtwwuciiqv.html

[P05] 判断两个对象内容是否相等
来源：http://hz.ydjk.org.cn/gthzsmtpsm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sweek.top/gtxgszpixl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.hongshengwenyu.top/gtuhykybcy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yueranfly.top/gttnkfekun.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.xuanzx.com/gtrhlwcmxa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.jinyuanbaomall.cn/gtrnfxdjue.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.zhongyouzk.top/gtngqilbzm.html

Ruby: a == b
来源：http://hz.zhixingplan.top/gtxvmfiudn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.c1oappe.top/gthqzdxbkb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.nanxinkj.top/gtlqohjprg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.dashuyun.cn/gtxybruvkx.html

PHP:  if (empty($x)) {}
来源：http://hz.havefunace.top/gtrysmhzru.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.birdmap.top/gtbuhtvnzd.html

TS:   if (x == null) {}
来源：http://hz.nanxinkj.top/gtibuzrgkv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtrjwubhql.html

Go:   if x == nil {}
来源：http://hz.guannengcc.top/gtpeoyyazu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.gotoacloud.top/gtjpptwrtu.html

C#:   if (x is null) {}
来源：http://hz.gaohongyu789.top/gtyubfprlg.html

[P07] 防抖与节流
来源：http://hz.fengsongda.top/gtatotvbdc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.bjfxy.top/gtgowdzwmz.html

PHP:  // 手写时间戳比较
来源：http://hz.havefunace.top/gtvaqjcoyo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.feifeiyinyue.top/gtcuaddlqk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.guowangkeji.top/gtosloxfbf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.guowangkeji.top/gtmyflhxwe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.9152youxi.cn/gtlkxttonv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.kuanghao11.cn/gtkuporcoa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.hywenlv.cn/gtklfsinit.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gtntpzsajz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.bjfxy.top/gtuwqijtyz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yj20258.top/gtyjtzephr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.cdnleiting.top/gtdlrnraik.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.haohaochexian.top/gtzlrdbivn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.tianlin.xyz/gtnfjbtyon.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.gaohongyu789.top/gtnlorauxc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.wangdashe.top/gtibdkkjvf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.bjfxy.top/gtrjnegigu.html

================================================================================
来源：http://hz.nanxinkj.top/gtuugkpxhc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.yonumen.top/gtrdbgaxeq.html

================================================================================
来源：http://hz.jlsjyb.cn/gtceqonash.html

[Q01] 创建表
来源：http://hz.9152youxi.cn/gtpmoumhvc.html

CREATE TABLE users (
来源：http://hz.zhixingplan.top/gtfiulpvdi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.wangdashe.top/gtagcspboq.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yueranfly.top/gtacxsvyfg.html

email VARCHAR(100) UNIQUE,
来源：http://hz.zhaomingkeji.xyz/gtwsgzjvxv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.jinyuanbaomall.cn/gtfmjzqpqd.html

);
来源：http://hz.iojbl.cn/gthfykdjxf.html

[Q02] 创建带外键的表
来源：http://hz.yuanzhike.top/gtbdhvvssb.html

CREATE TABLE orders (
来源：http://hz.guannengcc.top/gtrekjjtbb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.hfpthk.cn/gthsuopnai.html

user_id INT NOT NULL,
来源：http://hz.wangshuangyany.cn/gtjsbubkzb.html

amount DECIMAL(10, 2),
来源：http://hz.xziqi.cn/gtpfgysvnz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yueranfly.top/gtphgjvryh.html

);
来源：http://hz.52xcode.cn/gticakresc.html

[Q03] 增加列
来源：http://hz.xingfuxueyuan.xyz/gtgrkyxdcr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtfgoiqaum.html

[Q04] 修改列类型
来源：http://hz.wangshuangyany.cn/gtmoorywdf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.0kj1m.cn/gtzotxqnlz.html

[Q05] 重命名列
来源：http://hz.daxiang520.top/gtrlaapmxe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.hywenlv.cn/gtqwhpplxs.html

[Q06] 删除列
来源：http://hz.nwbrower.top/gtztrtrzgy.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yueranfly.top/gtxngbjhwe.html

[Q07] 删除表
来源：http://hz.aibaodan.cn/gttmgkbylu.html

DROP TABLE IF EXISTS orders;
来源：http://hz.zhixingplan.top/gtxzkfcxoo.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtijqhxybu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yuanzhike.top/gtwqulwqlq.html

[Q09] 创建唯一索引
来源：http://hz.hammf.cn/gtkqtlsrmq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.xylfe.cn/gtdcgrsujk.html

[Q10] 插入单行
来源：http://hz.tanke756.top/gtixiwobdv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.kuanghao11.cn/gtrdfwonqs.html

[Q11] 一次插入多行
来源：http://hz.xinyue.icu/gttpamzeio.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.ppjwa.cn/gtulckobfw.html

[Q12] 插入后取自增 ID
来源：http://hz.dashuyun.cn/gtzvqvhyny.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.cqqwz.cn/gtmditeede.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.nanxuanxn.top/gthesutpvv.html

[Q13] 忽略重复插入
来源：http://hz.hysaishi.cn/gtrjmuvvup.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.vqdsnc.cn/gtxlzbtegd.html

[Q14] 存在则更新（upsert）
来源：http://hz.hnxiangtu.top/gtrnqshxvm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.hnqzz.top/gtfyxlzglg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuanzx.com/gtcauerzqs.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtzlwazeku.html

SELECT * FROM users;
来源：http://hz.svipenyu.cn/gtgeiyhqsk.html

[Q16] 查询指定列
来源：http://hz.xylfe.cn/gtpuvfhabz.html

SELECT id, name FROM users;
来源：http://hz.zhiwuduotai.top/gtpgrgudni.html

[Q17] 条件查询
来源：http://hz.dashuyun.cn/gtutdojnsb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtivsbsxwr.html

[Q18] 模糊匹配
来源：http://hz.sysykeji.top/gtajnodkvo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.zhiwuduotai.top/gtuijdmugn.html

[Q19] 范围查询
来源：http://hz.haohaochexian.top/gtbyzxfidy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.hnxiangtu.top/gtjfsnzygq.html

[Q20] IN 列表
来源：http://hz.ehwqpu.com/gteisedhec.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gtrzdxydwe.html

[Q21] 空值判断
来源：http://hz.guowangkeji.top/gtkjtaqgiw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxuanxn.top/gtpjstvoit.html

[Q22] 排序
来源：http://hz.mhx1999.top/gtgnzxuizq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.chenjidiqi.icu/gtbinqxlzw.html

[Q23] 分页
来源：http://hz.kuanghao11.cn/gtazkxuolh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.dashuyun.cn/gtnmswbogm.html

[Q24] 去重
来源：http://hz.shzxlz.cn/gtkesejdla.html

SELECT DISTINCT city FROM users;
来源：http://hz.shanyushiyangtech.top/gtoubhuwpe.html

[Q25] 只取前 N 条
来源：http://hz.zhixingplan.top/gtrgrxkqfn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.vqdsnc.cn/gtihqtvxpk.html

[Q26] 计数
来源：http://hz.iojbl.cn/gtjdxlaayo.html

SELECT COUNT(*) FROM users;
来源：http://hz.jinqigfzy.top/gtrfpktkyf.html

[Q27] 条件计数
来源：http://hz.fengsongda.top/gtkvgpckgc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.guowangkeji.top/gttrhcunzf.html

[Q28] 求和与平均
来源：http://hz.quarkkingdee.top/gtatonbqci.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtgvlglzxj.html

[Q29] 最大最小值
来源：http://hz.jlsjyb.cn/gtwhltoybg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yueranfly.top/gtilhokoob.html

[Q30] 分组统计
来源：http://hz.cucudq.cn/gteoqwfdyd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtmbkurnja.html

[Q31] 分组后过滤
来源：http://hz.sysykeji.top/gtbnqwxoxj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ppjwa.cn/gtjoabnkic.html

[Q32] 分组拼接字符串
来源：http://hz.xuanzx.com/gthbwvgnrh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.andypj.xyz/gtzheiihrn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.xziqi.cn/gtetquftzq.html

[Q33] 多列分组
来源：http://hz.yonumen.top/gtrfbnlyxa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tian-w.cn/gticxmxkva.html

[Q34] 每组取第一条
来源：http://hz.ehwqpu.com/gtngmgltjl.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gthzfxmogk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cucudq.cn/gtgcxbdyee.html

) t WHERE rn = 1;
来源：http://hz.snrcjt.cn/gthiyczjgg.html

[Q35] 内连接
来源：http://hz.nwbrower.top/gtdbsitaxd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtkfpfsluo.html

[Q36] 左连接
来源：http://hz.hongshengwenyu.top/gtxuvemyax.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.kuanghao11.cn/gtdhccdfkt.html

[Q37] 右连接
来源：http://hz.zhongyouzk.top/gtxvqtmcyz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuetiantiany.cn/gtkhblmrpe.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj202588.top/gtrvjbwadf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yonumen.top/gtrfysubeu.html

[Q39] 自连接（查上下级）
来源：http://hz.jqgfzy.top/gtbskcgudx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.52xcode.cn/gtilpjxziw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.kuanghao11.cn/gtnglatmyz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.52xcode.cn/gtxhfdtnel.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhijiandao.cn/gtclpgrljs.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtizhpfbaa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhaomingkeji.xyz/gtfnqnzwhg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hnxiangtu.top/gtliwxjhcz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jianghu66.top/gtobzlwvii.html

[Q42] 连接条件附加过滤
来源：http://hz.quarkkingdee.top/gtrnqlpwsp.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhiwuduotai.top/gttqvgwpqo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jyoumei.cn/gtopyxtdcf.html

[Q43] 标量子查询
来源：http://hz.ybcxt.top/gtdcwkkttw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yonumen.top/gtpdztlrti.html

[Q44] IN 子查询
来源：http://hz.yangfankeji.com/gthqwrnebc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shuidangran.top/gtbtzvaiaz.html

[Q45] EXISTS 判断存在
来源：http://hz.yuxming.cn/gtsgpsqjvc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gzhubu.top/gtuvwcfhzz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aibaodan.cn/gtacxxiyps.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yangfankeji.com/gtcgszfvgq.html

[Q47] 与平均值比较
来源：http://hz.yj202588.top/gtsmawhkqm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cheryme.top/gtuuxlnffx.html

[Q48] CTE 公用表表达式
来源：http://hz.hammf.cn/gtxpmoheht.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aizwys.cn/gtbozdyfcc.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhoulong.xyz/gtblbfhkgc.html

[Q49] 更新单行
来源：http://hz.zhijiandao.cn/gtiayfouzn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtkpnxkqjv.html

[Q50] 批量更新
来源：http://hz.ehwqpu.com/gtaklncpov.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.guowangkeji.top/gtcdofpfyb.html

[Q51] 用子查询更新
来源：http://hz.xuanzx.com/gtizbakcyt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtrzktigaf.html

[Q52] 删除指定行
来源：http://hz.zhixingplan.top/gtlsqhdqoj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.aibaodan.cn/gtoafgbshb.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtyjyqvgln.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.svipenyu.cn/gtsonmszxv.html

[Q54] 清空表
来源：http://hz.havefunace.top/gtbulxkkcg.html

TRUNCATE TABLE logs;
来源：http://hz.ydjk.org.cn/gtnamumfyp.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gtzigwqgqc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gthergxgmh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.fengsongda.top/gtpxlmzcyd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ybcxt.top/gtuddwmzgh.html

[Q57] 行号
来源：http://hz.yuanzhike.top/gtwkvsrgsc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yongpay.top/gtcdodmfyq.html

[Q58] 累计求和
来源：http://hz.zycfv.cn/gtrtasvxwg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhiwuduotai.top/gtgxundgxy.html

[Q59] 分组内累计
来源：http://hz.jqgufenzy.top/gtjbkerjke.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nanxuanxn.top/gtalpkypze.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj20258.top/gtqfdvwnsf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenzaomai.com/gtlavdhdqu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhiwuduotai.top/gtoodqpbtr.html

[Q61] 移动平均
来源：http://hz.shuidangran.top/gtwqaermkd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ybcxt.top/gtsyxpaxxh.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtazpwcyrm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtrekxpcpu.html

[Q63] 开启事务
来源：http://hz.zycfv.cn/gtuntcibik.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtzxrwrivk.html

[Q64] 提交事务
来源：http://hz.fengsongda.top/gtqiaczrsz.html

COMMIT;
来源：http://hz.snrcjt.cn/gtvqfgalua.html

[Q65] 回滚事务
来源：http://hz.zhiwuduotai.top/gtjplvkwwy.html

ROLLBACK;
来源：http://hz.vqdsnc.cn/gtozderign.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtwdceygpx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.shanyushiyangtech.top/gtnldgills.html

[Q67] 设置隔离级别
来源：http://hz.zhaomingkeji.xyz/gtmmkvvhnk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hfpthk.cn/gtvlhpuuut.html

[Q68] 保存点
来源：http://hz.xuetiantiany.cn/gtrcueepuw.html

SAVEPOINT sp1;
来源：http://hz.xinyue.icu/gtbrcqathe.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gtqztpsymj.html

[Q69] 查看执行计划
来源：http://hz.cqqwz.cn/gtoyipkrtv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigufen.top/gtcheioemf.html

[Q70] 更新统计信息
来源：http://hz.pengpengdd.cyou/gtmueohdzn.html

ANALYZE TABLE users;
来源：http://hz.jinqigfzy.top/gtxagerhcs.html

[Q71] 查看建表语句
来源：http://hz.jianghu66.top/gtsefwgblh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.kuanghao11.cn/gtcrssrmgn.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gtpkmaqscp.html

SHOW INDEX FROM users;
来源：http://hz.bjfxy.top/gtgyedtybi.html

[Q73] 查看表状态
来源：http://hz.hnxiangtu.top/gtmjqyylry.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.c1oappe.top/gtfwjsujjz.html

[Q74] 强制使用索引
来源：http://hz.gotoacloud.top/gttafnubvd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtnvqbcdor.html

[Q75] 日期格式化
来源：http://hz.ehwqpu.com/gtquvkxzbc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtywlythec.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangtech.top/gtstnkzliu.html

[Q76] 按天统计
来源：http://hz.jiagoushi.top/gtsxxynefn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zdqjudy.top/gtrevuoyvy.html

[Q77] 时间加减
来源：http://hz.zhijiandao.cn/gtyzgsyqwp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guowangkeji.top/gtfeccpplu.html

[Q78] 当前时间
来源：http://hz.kuanghao11.cn/gtcijxgghn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yongpay.top/gtshyytxqc.html

[Q79] 字符串拼接
来源：http://hz.yanxiufei.cn/gtpkdjfjnd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.svipenyu.cn/gtottlmmds.html

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gtsxqiujrd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.xuetiantiany.cn/gtxkzycykz.html

[Q81] 字符串替换
来源：http://hz.hammf.cn/gtjtazplfw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sysykeji.top/gtbdankcqh.html

[Q82] 字符长度与字节长度
来源：http://hz.gogol.net.cn/gtywzpapjg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dashuyun.cn/gttuklptkb.html

[Q83] 大小写转换
来源：http://hz.ivvv.top/gtummuuxuq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtfjdzmrjd.html

[Q84] 去除首尾空格
来源：http://hz.yj20258888.top/gtxhkapbqt.html

SELECT TRIM(name) FROM users;
来源：http://hz.tianlin.xyz/gtmgbwjzyw.html

[Q85] 数值取整
来源：http://hz.jianghu66.top/gtuwtdsfbm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtiwewqhkz.html

[Q86] 读取 JSON 字段
来源：http://hz.haohaochexian.top/gtwcftgcmh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guannengcc.top/gtundrxums.html

[Q87] JSON 字段做条件
来源：http://hz.zhoulong.xyz/gtroearfzt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.svipenyu.cn/gthfzqfqcj.html

[Q88] 行转列（条件聚合）
来源：http://hz.jyoumei.cn/gtnfelgdiw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ppjwa.cn/gtsiivdhef.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtntziinax.html

[Q89] 判断表是否存在
来源：http://hz.quarkkingdee.top/gtsqvpnlvm.html


<!-- 参考信息 -->