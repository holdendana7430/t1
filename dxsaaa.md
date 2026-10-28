代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cqqwz.cn/gtofmjjvgn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.52xcode.cn/gtfnzheaaw.html

[P03] 生成短随机字符串
来源：http://hz.ppjwa.cn/gttjukrnbh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.shangyingyoupin.top/gtlfachzyw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jlsjyb.cn/gtijdsbnsy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.quarkkingdee.top/gtgdwppstz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxuanxn.top/gtobvbqdfh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuanzhike.top/gtkcflygvk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.ydzc1.top/gtdfonbhcp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.gogol.net.cn/gtonvkqbej.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xylfe.cn/gtfzgekquj.html

[P04] 求长度
来源：http://hz.shzxlz.cn/gtyivdnmoo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gtzeppczkj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtcevugwwz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xingfuxueyuan.xyz/gtjjzwzipi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yanxiufei.cn/gtalultlow.html

Java: list.size();  map.size();  s.length()
来源：http://hz.nanxinkj.top/gttjowervu.html

Go:   len(arr);  len(m)
来源：http://hz.cashguo.top/gtfppnlfjl.html

Ruby: x.length;  x.size
来源：http://hz.nanxuanxn.top/gtocyuwqqs.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.tanke756.top/gtxfgjfjry.html

[P05] 判断两个对象内容是否相等
来源：http://hz.shangyingyoupin.top/gtecjhnhyf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.cdnleiting.top/gtvbtjovyh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.gotoacloud.top/gtktqoccgd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.hysaishi.cn/gttgovtpmm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gthcdfhysv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.zhongyouzk.top/gtnxeklvns.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.jinghuilouyu.cn/gtevqmrvqo.html

Ruby: a == b
来源：http://hz.bjfxy.top/gtsblpeywr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.9152youxi.cn/gtskhdfdoy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.dianchejie.cn/gtodnurcdb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.sysykeji.top/gtuxduvqua.html

PHP:  if (empty($x)) {}
来源：http://hz.mhx1999.top/gttcswfweb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.aizwys.cn/gtcryzrccm.html

TS:   if (x == null) {}
来源：http://hz.chenzaomai.com/gthbwbhbcl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtqgpftfcc.html

Go:   if x == nil {}
来源：http://hz.wangshuangyany.cn/gttvijchpn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.fengsongda.top/gtjsmjzdvd.html

C#:   if (x is null) {}
来源：http://hz.tian-w.cn/gtknrlhrmh.html

[P07] 防抖与节流
来源：http://hz.zhengqikj.top/gtlfzopilu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.jiagoushi.top/gtzrfrhogi.html

PHP:  // 手写时间戳比较
来源：http://hz.zhengqikj.top/gtcnljlmbf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zhixingplan.top/gtdbzudvee.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gaohongyu789.top/gtonluoaae.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.fzhhl.top/gtylfeazco.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.guowangkeji.top/gtjqbbutlh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangdashe.top/gtufczfmiy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.cashguo.top/gthrhensml.html

[P08] 处理浮点精度问题
来源：http://hz.vqdsnc.cn/gtskeaykyr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shuidangran.top/gtsgbpmwus.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zdqjudy.top/gtlubskzbg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.xuanzx.com/gtlojxdpuf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xziqi.cn/gtzvjnjckf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.hywenlv.cn/gtgnqnxfec.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.jinghuilouyu.cn/gtnpauqjui.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.aibaodan.cn/gtbrezqbbr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.hywenlv.cn/gtdoluzjbs.html

================================================================================
来源：http://hz.jianghu66.top/gtkqegpboh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zdqjudy.top/gtwxwuhzmv.html

================================================================================
来源：http://hz.jqgfzy.top/gtorquckkx.html

[Q01] 创建表
来源：http://hz.316326.xyz/gtkqujvwis.html

CREATE TABLE users (
来源：http://hz.jiagoushi.top/gteizeunlp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.shzxlz.cn/gtpgsnjeyb.html

name VARCHAR(50) NOT NULL,
来源：http://hz.nanxinkj.top/gtpftiyszi.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gogol.net.cn/gtprseuqvm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.fzhhl.top/gtuvhyqema.html

);
来源：http://hz.mhx1999.top/gtasggmrpy.html

[Q02] 创建带外键的表
来源：http://hz.jqgfzy.top/gtlrcxattw.html

CREATE TABLE orders (
来源：http://hz.quarkkingdee.top/gtuhoxlihi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.dashuyun.cn/gttijuraza.html

user_id INT NOT NULL,
来源：http://hz.yj20258.top/gtepbjjged.html

amount DECIMAL(10, 2),
来源：http://hz.jinqigufen.top/gtpfptdgdg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.xylfe.cn/gttdqwlgjr.html

);
来源：http://hz.jiagoushi.top/gtdhgovoez.html

[Q03] 增加列
来源：http://hz.yanxiufei.cn/gtqcwhlxce.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.pycfn.com/gtnexbhbrj.html

[Q04] 修改列类型
来源：http://hz.zhijiandao.cn/gtbxozwvtl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hongshengwenyu.top/gtzqtedgpi.html

[Q05] 重命名列
来源：http://hz.yj202588.top/gtqhhovtsk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.nanxuanxn.top/gtpartgpvl.html

[Q06] 删除列
来源：http://hz.ppjwa.cn/gtjbjvmnmq.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.yj202588.top/gtqzxloasq.html

[Q07] 删除表
来源：http://hz.xingfuxueyuan.xyz/gtdzrjvbou.html

DROP TABLE IF EXISTS orders;
来源：http://hz.pycfn.com/gtiybkskbh.html

[Q08] 创建普通索引
来源：http://hz.havefunace.top/gtdeevlfdy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.hfpthk.cn/gtxeqhcdzz.html

[Q09] 创建唯一索引
来源：http://hz.zhongyouzk.top/gtldbkdlof.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.zhixingplan.top/gtaajcbdft.html

[Q10] 插入单行
来源：http://hz.xinyue.icu/gtueiipsml.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.hfpthk.cn/gtxaghrhrp.html

[Q11] 一次插入多行
来源：http://hz.jinqigufen.top/gtnblxkpun.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.zhixingplan.top/gtffjqwapq.html

[Q12] 插入后取自增 ID
来源：http://hz.yj202588.top/gtpvdcfyyp.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.nwbrower.top/gtlfjugcsj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.cdnleiting.top/gtgncwqimp.html

[Q13] 忽略重复插入
来源：http://hz.dashuyun.cn/gtzomgqscm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenlongwang.top/gtenqnefir.html

[Q14] 存在则更新（upsert）
来源：http://hz.bjfxy.top/gtroicaxrv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.dianchejie.cn/gtbyeogtnz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.tanke756.top/gtonjptbgi.html

[Q15] 查询全部
来源：http://hz.yuanzhike.top/gtewxfybnm.html

SELECT * FROM users;
来源：http://hz.cqqwz.cn/gtpreyuqwu.html

[Q16] 查询指定列
来源：http://hz.birdmap.top/gtqmzazbkt.html

SELECT id, name FROM users;
来源：http://hz.kuanghao11.cn/gtjlfhfmlj.html

[Q17] 条件查询
来源：http://hz.jlsjyb.cn/gtacpwyyqm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.iojbl.cn/gtobkrdffs.html

[Q18] 模糊匹配
来源：http://hz.xylfe.cn/gtlozusdls.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.guannengcc.top/gtozpefyci.html

[Q19] 范围查询
来源：http://hz.fzhhl.top/gtzsgsguwt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.daria6918.cn/gtmdnsnjcl.html

[Q20] IN 列表
来源：http://hz.yueranfly.top/gtabqipjaz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.smart0.xyz/gtrzffmqna.html

[Q21] 空值判断
来源：http://hz.mhx1999.top/gtebwaohji.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.cqqwz.cn/gtamgnadxy.html

[Q22] 排序
来源：http://hz.ppjwa.cn/gtfgtmytgi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.shanyushiyangtech.top/gtzyjrtfcb.html

[Q23] 分页
来源：http://hz.52xcode.cn/gtdxfatnyw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shangyingyoupin.top/gtvaapbsmt.html

[Q24] 去重
来源：http://hz.svipenyu.cn/gtngjsbdgh.html

SELECT DISTINCT city FROM users;
来源：http://hz.aibaodan.cn/gtejaavrfp.html

[Q25] 只取前 N 条
来源：http://hz.yanxiufei.cn/gtntxlymcd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.cqqwz.cn/gtmcdzanoz.html

[Q26] 计数
来源：http://hz.ppjwa.cn/gtonyjtxhk.html

SELECT COUNT(*) FROM users;
来源：http://hz.jlsjyb.cn/gtmsdxomqc.html

[Q27] 条件计数
来源：http://hz.quarkkingdee.top/gtizomhxnd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xylfe.cn/gtyxorbkpf.html

[Q28] 求和与平均
来源：http://hz.aibaodan.cn/gtlbshcwdk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.birdmap.top/gtozqoqhzj.html

[Q29] 最大最小值
来源：http://hz.tianlin.xyz/gtvmcmuleo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhijiandao.cn/gtcczvtelx.html

[Q30] 分组统计
来源：http://hz.tanke756.top/gtecwsouco.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtjkzpkqbd.html

[Q31] 分组后过滤
来源：http://hz.pengpengdd.cyou/gtmkchizka.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gtyjskdymv.html

[Q32] 分组拼接字符串
来源：http://hz.sxryk.cn/gtefwvhzai.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hysaishi.cn/gtkpbkegdp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.aibaodan.cn/gtsfeidsnb.html

[Q33] 多列分组
来源：http://hz.shzxlz.cn/gtzzxkwcgr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zycfv.cn/gtxhgcmwmv.html

[Q34] 每组取第一条
来源：http://hz.gzhubu.top/gtfeiqfeud.html

SELECT * FROM (
来源：http://hz.yj20258.top/gtnmjlywsp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.sxryk.cn/gtuauaxhbv.html

) t WHERE rn = 1;
来源：http://hz.jinghuilouyu.cn/gtudyifycf.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gtecoooblf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj202588.top/gtgnxflllc.html

[Q36] 左连接
来源：http://hz.dashuyun.cn/gtvoyshhcp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtlyhiocrw.html

[Q37] 右连接
来源：http://hz.yuxming.cn/gttmkmcswc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dashuyun.cn/gthvxsajbz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zycfv.cn/gtlbuoschr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnxiangtu.top/gtiinqvkji.html

[Q39] 自连接（查上下级）
来源：http://hz.aibaodan.cn/gtvpitqcca.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhaomingkeji.xyz/gtdjkypbgr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jianghu66.top/gtiggsqvee.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ydzc1.top/gtqlsdpeit.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.ywan-chungtsiang.top/gtgnuepwhr.html

[Q41] 多表连接
来源：http://hz.vqdsnc.cn/gtknnctbus.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gtfymoojks.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yuxming.cn/gtrbzxvftj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gthpcylpln.html

[Q42] 连接条件附加过滤
来源：http://hz.jinqigufen.top/gtjbyapeul.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xinyue.icu/gtzgozbbrv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cashguo.top/gtxkogvchh.html

[Q43] 标量子查询
来源：http://hz.yj20258.top/gtcjukdglu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtcanmkwch.html

[Q44] IN 子查询
来源：http://hz.xziqi.cn/gtnqdpiexa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hysaishi.cn/gtszgzefqi.html

[Q45] EXISTS 判断存在
来源：http://hz.daxiang520.top/gtgdtkwcnw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtlwsitnhy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sxryk.cn/gtffjolajh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtkywgszuy.html

[Q47] 与平均值比较
来源：http://hz.mhx1999.top/gtdpnjxffp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jlsjyb.cn/gtlhnpbnqx.html

[Q48] CTE 公用表表达式
来源：http://hz.smart0.xyz/gtecusnmfi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zycfv.cn/gtrpfejyyr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258.top/gtpfmaivjz.html

[Q49] 更新单行
来源：http://hz.ybcxt.top/gtzmfcwxzk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yuanzhike.top/gtiegvwjfc.html

[Q50] 批量更新
来源：http://hz.shangyingyoupin.top/gthagwgxdt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.feifeiyinyue.top/gtykhctshm.html

[Q51] 用子查询更新
来源：http://hz.wangdashe.top/gttdafqnpa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtfddvoxok.html

[Q52] 删除指定行
来源：http://hz.xylfe.cn/gtsckdzcrx.html

DELETE FROM users WHERE id = 10;
来源：http://hz.smart0.xyz/gtleddyaoj.html

[Q53] 按条件删除
来源：http://hz.chenlongwang.top/gtlgyoosnq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtcwgyntdl.html

[Q54] 清空表
来源：http://hz.yanxiufei.cn/gtrkfttmue.html

TRUNCATE TABLE logs;
来源：http://hz.tanke756.top/gtmihryqvy.html

[Q55] 排名（并列占位）
来源：http://hz.xylfe.cn/gtbqiyjghw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guowangkeji.top/gtssyzlhxg.html

[Q56] 密集排名（并列不占位）
来源：http://hz.aizwys.cn/gtbqglusnx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jinqigufen.top/gtxgotolpk.html

[Q57] 行号
来源：http://hz.guannengcc.top/gtfwunbhdr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shuidangran.top/gtriowtvqe.html

[Q58] 累计求和
来源：http://hz.jinqigufen.top/gtybeqrhdn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhoulong.xyz/gtvadevwpt.html

[Q59] 分组内累计
来源：http://hz.c1oappe.top/gtjhpjoacn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtnevsvzkm.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtgyqyxbhw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnqzz.top/gtdnuoonxu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jlsjyb.cn/gtiwzbnllh.html

[Q61] 移动平均
来源：http://hz.zhongyouzk.top/gtaxbksttt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258888.top/gtjaltuxvt.html

[Q62] 分组占比
来源：http://hz.guannengcc.top/gtvguvwszu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtojebjymt.html

[Q63] 开启事务
来源：http://hz.gotoacloud.top/gtktddueoz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.haohaochexian.top/gttxqzlilf.html

[Q64] 提交事务
来源：http://hz.chenlongwang.top/gtbcfsbirr.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtaelnovrl.html

[Q65] 回滚事务
来源：http://hz.hnqzz.top/gteepnroxn.html

ROLLBACK;
来源：http://hz.52xcode.cn/gteiqstkvm.html

[Q66] 行锁查询
来源：http://hz.iojbl.cn/gtisacizos.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtbbcbvdfi.html

[Q67] 设置隔离级别
来源：http://hz.yangfankeji.com/gtutnigljs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jiagoushi.top/gtgllwjkav.html

[Q68] 保存点
来源：http://hz.hongshengwenyu.top/gthhnkyaoo.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtjdwzfgxt.html

ROLLBACK TO sp1;
来源：http://hz.jinyuanbaomall.cn/gtqhucgptz.html

[Q69] 查看执行计划
来源：http://hz.ywan-chungtsiang.top/gtlgpdnajx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xinyue.icu/gtznqmwlqh.html

[Q70] 更新统计信息
来源：http://hz.fzhhl.top/gtbcdnspay.html

ANALYZE TABLE users;
来源：http://hz.vqdsnc.cn/gtynfpnsmk.html

[Q71] 查看建表语句
来源：http://hz.52xcode.cn/gtltgkxfel.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.9152youxi.cn/gtpvybxxxg.html

[Q72] 查看索引
来源：http://hz.havefunace.top/gtbmxcvqkv.html

SHOW INDEX FROM users;
来源：http://hz.svipenyu.cn/gtodhgcnez.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gthwimgugv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinghuilouyu.cn/gtyzqwqxrv.html

[Q74] 强制使用索引
来源：http://hz.nanxuanxn.top/gtdhoaqbfd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cucudq.cn/gtqbxqmjsw.html

[Q75] 日期格式化
来源：http://hz.aizwys.cn/gtlnigdkcf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ivvv.top/gtsuicywce.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ydzc1.top/gtnmiryodk.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtnjfybdfa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhaomingkeji.xyz/gtwqhtrhfc.html

[Q77] 时间加减
来源：http://hz.yj202588.top/gtpokiahch.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yanxiufei.cn/gtbpuobztr.html

[Q78] 当前时间
来源：http://hz.zhixingplan.top/gteieftcwb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cashguo.top/gtvoiyecux.html

[Q79] 字符串拼接
来源：http://hz.hywenlv.cn/gtbvistzxv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cashguo.top/gtedmmomtm.html

[Q80] 字符串截取
来源：http://hz.c1oappe.top/gttiujjufh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.meibo888.top/gtepcixioi.html

[Q81] 字符串替换
来源：http://hz.cheryme.top/gtewpbygao.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangkeji.top/gtjubmyoww.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gtolmskqkz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtpyfcjkah.html

[Q83] 大小写转换
来源：http://hz.hongshengwenyu.top/gtqenalnnl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigfzy.top/gtwcajjwiu.html

[Q84] 去除首尾空格
来源：http://hz.ybcxt.top/gtgetpqlyw.html

SELECT TRIM(name) FROM users;
来源：http://hz.yanxiufei.cn/gtmxxtumwl.html

[Q85] 数值取整
来源：http://hz.nanxinkj.top/gtzirkpwjj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ehwqpu.com/gtlbxkeuyx.html

[Q86] 读取 JSON 字段
来源：http://hz.zdqjudy.top/gtmijffnxr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sufxvd.cn/gtjyaykbob.html

[Q87] JSON 字段做条件
来源：http://hz.zhijiandao.cn/gtjksocrky.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gttujatinw.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxinkj.top/gtjzdjehyd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinghuilouyu.cn/gtugtphyds.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnxiangtu.top/gtlyekwmlz.html

[Q89] 判断表是否存在
来源：http://hz.chenjidiqi.icu/gtwcnymxoh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtgaphelqt.html

[Q90] 生成序号列
来源：http://hz.shzxlz.cn/gtviiqocco.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gtbhrcuxot.html

================================================================================
来源：http://hz.vqdsnc.cn/gtyxmwbize.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtmqhptbdz.html

================================================================================
来源：http://hz.cashguo.top/gtbgnmsadl.html

[R01] shebang 与严格模式
来源：http://hz.cashguo.top/gtetloqzjs.html

#!/usr/bin/env bash
来源：http://hz.jianghu66.top/gtbojjtspu.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtzbehlotz.html

[R02] 变量赋值与使用
来源：http://hz.guannengcc.top/gtkbowikia.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtpojxgehd.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gtuucvmjmo.html

readonly PI=3.14
来源：http://hz.zhiwuduotai.top/gtdjaolvmo.html

[R04] 位置参数
来源：http://hz.sweek.top/gttvnnjyzu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ydzc1.top/gtoywpvmeo.html

[R05] 参数默认值
来源：http://hz.jinqigufen.top/gtyyjhqbna.html

name="${1:-default}"
来源：http://hz.yangfankeji.com/gthctwpfhl.html

[R06] 判断命令是否存在
来源：http://hz.zdqjudy.top/gtvxiatpeo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yongpay.top/gtsnpnyllh.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtanxnrhft.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cashguo.top/gtqfohcrdt.html

[R08] 数值比较
来源：http://hz.haohaochexian.top/gttjtijbve.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtqnnshtsi.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gtvqbzjjtt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtfsufpflq.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtvflhanzn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.52xcode.cn/gtcqgqmyoa.html

[R11] case 多分支
来源：http://hz.xinyue.icu/gteceypcov.html

case "$1" in
来源：http://hz.andypj.xyz/gtpzaezygv.html

start) echo "启动" ;;
来源：http://hz.ivvv.top/gtshxpfchp.html

stop)  echo "停止" ;;
来源：http://hz.aizwys.cn/gtnkvqoyeo.html

*)     echo "未知命令" ;;
来源：http://hz.tian-w.cn/gtiykfandk.html

esac
来源：http://hz.ybcxt.top/gtnzkhkgjx.html

[R12] for 遍历文件
来源：http://hz.yj20258888.top/gtpooikxgv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258888.top/gtztuvthvz.html

[R13] for 计数循环
来源：http://hz.nanxuanxn.top/gtxmukpjuh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtrknnvvkq.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gtlpfxhtyh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtuumfiewn.html

[R15] while 逐行读文件
来源：http://hz.aibaodan.cn/gtzpwjtfek.html


<!-- 参考信息 -->