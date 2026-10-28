代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://hz.shzxlz.cn/gtqapqwjuw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.havefunace.top/gtnfuzeehf.html

JS:   await Promise.all(tasks)
来源：http://hz.yj202588.top/gttluyavtd.html

TS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtcaiwrhsy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cqqwz.cn/gtywqlstan.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.meibo888.top/gtfveihcfk.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gtiueemvkp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.bjfxy.top/gtcgrwywdn.html

[O06] 使用进程池
来源：http://hz.hysaishi.cn/gtrirkwotg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gthykyvncl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj20258888.top/gtvjfrngse.html

JS:   // child_process / cluster 模块
来源：http://hz.chenzaomai.com/gtftfvbwry.html

TS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtmysdldtk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yongpay.top/gtnpstzxbp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gtmwydpcbq.html

Ruby: // fork 块
来源：http://hz.zhongyouzk.top/gtaordvmpq.html

C#:   Parallel.For
来源：http://hz.xylfe.cn/gtokxupoft.html

================================================================================
来源：http://hz.tanke756.top/gteepzsxos.html

P. 常用工具函数
来源：http://hz.zdqjudy.top/gtfrsxsdre.html

================================================================================
来源：http://hz.pycfn.com/gtegrjimwc.html

[P01] 生成 UUID
来源：http://hz.hnxiangtu.top/gtevhdqxhm.html

Py:   str(uuid.uuid4())
来源：http://hz.shuidangran.top/gtykracuje.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.fengsongda.top/gtyguutpor.html

JS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtqrfxnqza.html

TS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtbeijyyta.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gtmgpvnhjd.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shangyingyoupin.top/gtfyxtywhk.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtsbwsmcpa.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ppjwa.cn/gtxctcqcej.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtslecwesc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.cdnleiting.top/gtjnwrxaaq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.snrcjt.cn/gtxgfavzbq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yuxming.cn/gtjkzruycl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.pengpengdd.cyou/gtoppbkukh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258.top/gtfglzehfv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.dianchejie.cn/gtfsphqaas.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.aizwys.cn/gtisvnkknh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj202588.top/gtsscyrcjr.html

[P03] 生成短随机字符串
来源：http://hz.yj20258888.top/gtzpxyuppx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.gzhubu.top/gtiakmjdmp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xylfe.cn/gtjsgwvmqn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.daria6918.cn/gtsqsyfenv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuanzhike.top/gtaidutrbx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.xinyue.icu/gtjfhigvfp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jiagoushi.top/gtmhqfzudh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.jlsjyb.cn/gtujwuwydg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.jinyuanbaomall.cn/gttqcjvrpk.html

[P04] 求长度
来源：http://hz.ivvv.top/gtvzpgllda.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.vqdsnc.cn/gtddemwodu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yongpay.top/gtcbpqswmu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.fzhhl.top/gtztcpsggx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sweek.top/gtzkqifjvg.html

Java: list.size();  map.size();  s.length()
来源：http://hz.smart0.xyz/gtzbwkqzgg.html

Go:   len(arr);  len(m)
来源：http://hz.jianghu66.top/gtbemrhvwn.html

Ruby: x.length;  x.size
来源：http://hz.tanke756.top/gtoysbaqew.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.ywan-chungtsiang.top/gtdgoogcja.html

[P05] 判断两个对象内容是否相等
来源：http://hz.iojbl.cn/gtdfarwibr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.c1oappe.top/gtlemircyc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.pengpengdd.cyou/gttfghlnxr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.c1oappe.top/gtocemtehm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.andypj.xyz/gtjscgdezh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.fzhhl.top/gtijxlmxwd.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.chenlongwang.top/gtbiakeenj.html

Ruby: a == b
来源：http://hz.ywan-chungtsiang.top/gteqzvoail.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.jlsjyb.cn/gtlojoxyre.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.jinyuanbaomall.cn/gtyuknndla.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.shangyingyoupin.top/gtbtbxzwjx.html

PHP:  if (empty($x)) {}
来源：http://hz.vqdsnc.cn/gtzswztwyk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gotoacloud.top/gtkauhgxcl.html

TS:   if (x == null) {}
来源：http://hz.snrcjt.cn/gtqlvnzmdk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.redwolf501.top/gtdbmlckfw.html

Go:   if x == nil {}
来源：http://hz.quarkkingdee.top/gthpjxnhig.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.shanyushiyangtech.top/gtsanwzqhv.html

C#:   if (x is null) {}
来源：http://hz.shanyushiyangtech.top/gthiuuabin.html

[P07] 防抖与节流
来源：http://hz.fzhhl.top/gtylmbppbr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jlsjyb.cn/gtpjdqvlno.html

PHP:  // 手写时间戳比较
来源：http://hz.hongshengwenyu.top/gtrobjqqyi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.nwbrower.top/gtdundkgqy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtkgkexkdm.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.yj20258888.top/gtiyeacrby.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guannengcc.top/gtpnzeeexl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yj20258.top/gtbkuqrhhb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.jinqigfzy.top/gtmifucawo.html

[P08] 处理浮点精度问题
来源：http://hz.redwolf501.top/gttusyksor.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtrikeuaot.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.daxiang520.top/gtjjbwrnlm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zhoulong.xyz/gtjhpteyaz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ydjk.org.cn/gtlpyosjig.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.yj20258888.top/gtdjkfsxrr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinqigfzy.top/gtnzvaqccw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.snrcjt.cn/gtgdlppepv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.zhixingplan.top/gtvuawvaam.html

================================================================================
来源：http://hz.tian-w.cn/gtscncbxeg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.nanxuanxn.top/gtxpfzesvo.html

================================================================================
来源：http://hz.hammf.cn/gtasphluqx.html

[Q01] 创建表
来源：http://hz.svipenyu.cn/gtctnsebpb.html

CREATE TABLE users (
来源：http://hz.meibo888.top/gtszjnucep.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shuidangran.top/gtolvmursv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.xingfuxueyuan.xyz/gtmithfica.html

email VARCHAR(100) UNIQUE,
来源：http://hz.yongpay.top/gtpanttloj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.yuxming.cn/gtbzhojwhj.html

);
来源：http://hz.pengpengdd.cyou/gtiffxzowx.html

[Q02] 创建带外键的表
来源：http://hz.pycfn.com/gtxmueinrk.html

CREATE TABLE orders (
来源：http://hz.hammf.cn/gtslsdaagi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.nanxinkj.top/gtzjqtbszr.html

user_id INT NOT NULL,
来源：http://hz.52xcode.cn/gttztugvza.html

amount DECIMAL(10, 2),
来源：http://hz.nanxuanxn.top/gttfshvfoy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yj202588.top/gteddwkclj.html

);
来源：http://hz.wangdashe.top/gtodjkjfah.html

[Q03] 增加列
来源：http://hz.jianghu66.top/gtrgimjzrf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangshuangyany.cn/gtvevjlafl.html

[Q04] 修改列类型
来源：http://hz.yonumen.top/gtdeznnlcu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.pengpengdd.cyou/gtqncglyzz.html

[Q05] 重命名列
来源：http://hz.sysykeji.top/gtdxiicauf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.xziqi.cn/gtmncxvkur.html

[Q06] 删除列
来源：http://hz.yangfankeji.com/gteoynvbsu.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jiagoushi.top/gtqvfpjiio.html

[Q07] 删除表
来源：http://hz.zhaomingkeji.xyz/gtbprtiyek.html

DROP TABLE IF EXISTS orders;
来源：http://hz.quarkkingdee.top/gtqjcbdmze.html

[Q08] 创建普通索引
来源：http://hz.yuxming.cn/gtvxoucxel.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.shuidangran.top/gtvoarvikf.html

[Q09] 创建唯一索引
来源：http://hz.wangshuangyany.cn/gtvlubfmyd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtcpacpjit.html

[Q10] 插入单行
来源：http://hz.sufxvd.cn/gtjpcsypbz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xingfuxueyuan.xyz/gtkgidfwwj.html

[Q11] 一次插入多行
来源：http://hz.guannengcc.top/gttbearflo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.0kj1m.cn/gtkdzgpxrc.html

[Q12] 插入后取自增 ID
来源：http://hz.shanyushiyangtech.top/gtekrxjbqg.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.mhx1999.top/gtsgmqqlvo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.yonumen.top/gthreotfnb.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gtpotivipe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.jinqigufen.top/gtemnmuzel.html

[Q14] 存在则更新（upsert）
来源：http://hz.hfpthk.cn/gthhzmctdw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhaomingkeji.xyz/gttwfbmkud.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cheryme.top/gtrqdhvmdn.html

[Q15] 查询全部
来源：http://hz.chenjidiqi.icu/gtldihrksd.html

SELECT * FROM users;
来源：http://hz.mhx1999.top/gtnytdvzvv.html

[Q16] 查询指定列
来源：http://hz.xuetiantiany.cn/gtaaeybsly.html

SELECT id, name FROM users;
来源：http://hz.zhoulong.xyz/gtpfyuozho.html

[Q17] 条件查询
来源：http://hz.pengpengdd.cyou/gtzucsbtud.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.dianchejie.cn/gtmapjmlxz.html

[Q18] 模糊匹配
来源：http://hz.zhaomingkeji.xyz/gtodcqfxpy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yj202588.top/gtqqwbdxtg.html

[Q19] 范围查询
来源：http://hz.gogol.net.cn/gttofzxtcz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.bjfxy.top/gthqzxallj.html

[Q20] IN 列表
来源：http://hz.shanyushiyangkeji.top/gtygfyesoz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gtocwcqbmq.html

[Q21] 空值判断
来源：http://hz.yongpay.top/gtzxkmggsa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.chenjidiqi.icu/gtfwowbqes.html

[Q22] 排序
来源：http://hz.jinghuilouyu.cn/gttjkpfhmb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.9152youxi.cn/gtuikqsbaw.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gthldpyvgf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tianlin.xyz/gttwfwegup.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtmqdakwrd.html

SELECT DISTINCT city FROM users;
来源：http://hz.guowangkeji.top/gtrsrutuji.html

[Q25] 只取前 N 条
来源：http://hz.andypj.xyz/gthhqebhpi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.sysykeji.top/gtasjdmseh.html

[Q26] 计数
来源：http://hz.tian-w.cn/gtvjsoizoj.html

SELECT COUNT(*) FROM users;
来源：http://hz.tanke756.top/gtdjveexqn.html

[Q27] 条件计数
来源：http://hz.smart0.xyz/gtjstpvinn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.chenlongwang.top/gtoqbsyxyl.html

[Q28] 求和与平均
来源：http://hz.dashuyun.cn/gtqpnqmzkg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtnywydjht.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gtkdafsrzs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.snrcjt.cn/gtzqqiuymq.html

[Q30] 分组统计
来源：http://hz.c1oappe.top/gtuvnkzwch.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.fengsongda.top/gtgqocqpwc.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gtvioxtimu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ehwqpu.com/gtanigommc.html

[Q32] 分组拼接字符串
来源：http://hz.wangshuangyany.cn/gtkyricxlq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jqgfzy.top/gtkjjaedqo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.dashuyun.cn/gtdkywgmbd.html

[Q33] 多列分组
来源：http://hz.gogol.net.cn/gtmjalsfwg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gzhubu.top/gthgjxqajg.html

[Q34] 每组取第一条
来源：http://hz.pycfn.com/gtbxgdldwv.html

SELECT * FROM (
来源：http://hz.cheryme.top/gtgzozmcmn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.meibo888.top/gtrbjxvrdt.html

) t WHERE rn = 1;
来源：http://hz.bjfxy.top/gtvalctkth.html

[Q35] 内连接
来源：http://hz.jinyuanbaomall.cn/gtxfqkrzto.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtswlzevro.html

[Q36] 左连接
来源：http://hz.tianlin.xyz/gtzbvjyicw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtrpjvoflr.html

[Q37] 右连接
来源：http://hz.shangyingyoupin.top/gtwstsyjwc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yonumen.top/gtvcrhnesp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtsnhenpnp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhijiandao.cn/gtqmsuszrr.html

[Q39] 自连接（查上下级）
来源：http://hz.sweek.top/gtoybrsqqx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgufenzy.top/gtfwafybyn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.shzxlz.cn/gtrtleykbn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sxryk.cn/gtsyrdmddk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ydzc1.top/gtxacprssn.html

[Q41] 多表连接
来源：http://hz.gaohongyu789.top/gtjvzculpf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gthwcyjwwz.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hfpthk.cn/gtktmqtvce.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yj202588.top/gtydwhbein.html

[Q42] 连接条件附加过滤
来源：http://hz.chenjidiqi.icu/gtmazzefrk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigfzy.top/gtrkfmucct.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jlsjyb.cn/gtdbnjywbf.html

[Q43] 标量子查询
来源：http://hz.9152youxi.cn/gtjdvszdrw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xziqi.cn/gtuculkrld.html

[Q44] IN 子查询
来源：http://hz.chenlongwang.top/gtavxmrkmv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhiwuduotai.top/gtvdtuiohj.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gtloiajhwf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.quarkkingdee.top/gtitzzzsls.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ivvv.top/gttufnhtsh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cucudq.cn/gttzavingq.html

[Q47] 与平均值比较
来源：http://hz.tian-w.cn/gtyvoxhkjp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtbnqwuqax.html

[Q48] CTE 公用表表达式
来源：http://hz.pengpengdd.cyou/gttstpvnal.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.smart0.xyz/gtnniaeitp.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daxiang520.top/gtjrzmhiop.html

[Q49] 更新单行
来源：http://hz.xylfe.cn/gtneeeoidh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtghszzfud.html

[Q50] 批量更新
来源：http://hz.xylfe.cn/gtvmxrsild.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.c1oappe.top/gtdkklzdxb.html

[Q51] 用子查询更新
来源：http://hz.birdmap.top/gtnkbgklix.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.dianchejie.cn/gtwxotuypk.html

[Q52] 删除指定行
来源：http://hz.hfpthk.cn/gtehageynd.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sysykeji.top/gtulpibnqz.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtkspbgbyw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgufenzy.top/gtnyxslufx.html

[Q54] 清空表
来源：http://hz.52xcode.cn/gtbihufyxu.html

TRUNCATE TABLE logs;
来源：http://hz.jinghuilouyu.cn/gtxihjlbky.html

[Q55] 排名（并列占位）
来源：http://hz.0kj1m.cn/gtlbjcecls.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gttgcptkle.html

[Q56] 密集排名（并列不占位）
来源：http://hz.haohaochexian.top/gtwgltdrfz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.dashuyun.cn/gtsjsataxy.html

[Q57] 行号
来源：http://hz.cheryme.top/gtgdqmviwi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.redwolf501.top/gtfjydkuux.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtpampadjx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hammf.cn/gtbnxxckdt.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gtkpuacuip.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.andypj.xyz/gtoolvvnrz.html

[Q60] 取上一行 / 下一行
来源：http://hz.ivvv.top/gtlqxrszkn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gtyrgknbnx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.aizwys.cn/gtcwlchcny.html

[Q61] 移动平均
来源：http://hz.yuanzhike.top/gtqbvwwuqv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jiagoushi.top/gtmkgiechr.html

[Q62] 分组占比
来源：http://hz.nanxuanxn.top/gtvoxfbecd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtmpdvzghc.html

[Q63] 开启事务
来源：http://hz.chenlongwang.top/gtdbjtnaku.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtjtimmuea.html

[Q64] 提交事务
来源：http://hz.ehwqpu.com/gtqgowxtuu.html

COMMIT;
来源：http://hz.zhijiandao.cn/gtadjtvjyx.html

[Q65] 回滚事务
来源：http://hz.feifeiyinyue.top/gtvtlauzjl.html

ROLLBACK;
来源：http://hz.sysykeji.top/gtezuhgbya.html

[Q66] 行锁查询
来源：http://hz.ydzc1.top/gtalnrnjav.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenzaomai.com/gteqsghiqm.html

[Q67] 设置隔离级别
来源：http://hz.hywenlv.cn/gttqsoixko.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.andypj.xyz/gtxubiiezd.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtavosyman.html

SAVEPOINT sp1;
来源：http://hz.fzhhl.top/gtbbpknpyw.html

ROLLBACK TO sp1;
来源：http://hz.chenjidiqi.icu/gtspvzzqqn.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gtcamqhshj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangkeji.top/gtcldrucow.html

[Q70] 更新统计信息
来源：http://hz.zhijiandao.cn/gtdffgejqe.html

ANALYZE TABLE users;
来源：http://hz.guowangkeji.top/gtybyxmrmb.html

[Q71] 查看建表语句
来源：http://hz.pycfn.com/gtcyntnbzm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nwbrower.top/gtcxpyqmai.html

[Q72] 查看索引
来源：http://hz.iojbl.cn/gttupxwkru.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtmwmijtyh.html

[Q73] 查看表状态
来源：http://hz.snrcjt.cn/gtuknxdprf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtrgijhobp.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtoiwnpwrf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhijiandao.cn/gtnpsbfzih.html

[Q75] 日期格式化
来源：http://hz.xuanzx.com/gtrmthzikx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cqqwz.cn/gtpyvswguc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxuanxn.top/gtoiuwcjab.html

[Q76] 按天统计
来源：http://hz.dianchejie.cn/gtxtdhcffv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daria6918.cn/gtetivnkvm.html

[Q77] 时间加减
来源：http://hz.shanyushiyangtech.top/gtksuyirou.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gotoacloud.top/gtzyatbblw.html

[Q78] 当前时间
来源：http://hz.chenzaomai.com/gtxjgqymgn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtqtulkkiz.html

[Q79] 字符串拼接
来源：http://hz.yueranfly.top/gtyfcqvhen.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.52xcode.cn/gtpnermoaj.html

[Q80] 字符串截取
来源：http://hz.hnxiangtu.top/gtwatysgkk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhengqikj.top/gtqwmudxmn.html

[Q81] 字符串替换
来源：http://hz.ybcxt.top/gtkudabqky.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtsnqpdyjy.html

[Q82] 字符长度与字节长度
来源：http://hz.ppjwa.cn/gtrqnbxbge.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtocudnfwj.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gtihruloni.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtewogtcoz.html

[Q84] 去除首尾空格
来源：http://hz.haohaochexian.top/gtyrzkeynw.html

SELECT TRIM(name) FROM users;
来源：http://hz.sufxvd.cn/gtcmlyshnb.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtoutckomf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.316326.xyz/gtefitmurn.html

[Q86] 读取 JSON 字段
来源：http://hz.fengsongda.top/gtbvjoouhd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtwxzbdnlz.html

[Q87] JSON 字段做条件
来源：http://hz.fengsongda.top/gttwvayadd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigfzy.top/gtoxvjpvrs.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258888.top/gtrroumpzd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtbavaqrqa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangshuangyany.cn/gtyfduvofe.html

[Q89] 判断表是否存在
来源：http://hz.hywenlv.cn/gtxgvcwqhe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shangyingyoupin.top/gtqurtjxrz.html

[Q90] 生成序号列
来源：http://hz.gzhubu.top/gtlnjlrmxn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.mhx1999.top/gtbiqvcvxt.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtgzstsaaz.html


<!-- 参考信息 -->