代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.dashuyun.cn/gtshjhxeoo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenlongwang.top/gtyjxpgjra.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.feifeiyinyue.top/gtqpfjqbhg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yvedp.cn/gtjyjpiyff.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hywenlv.cn/gtmhcbbdfg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gotoacloud.top/gtttbwnquu.html

[P03] 生成短随机字符串
来源：http://hz.yj202588.top/gtnrznrwaz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.zhongyouzk.top/gtjkxbwthi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.gotoacloud.top/gtjzlfzber.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtqhimcjdm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinqigfzy.top/gtmtudiptd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.pycfn.com/gtjvmcikgw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.smart0.xyz/gtfivjkaxm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxinkj.top/gtdnnuebur.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.ybcxt.top/gtoizmuavt.html

[P04] 求长度
来源：http://hz.gaohongyu789.top/gttteeqkpa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.xuanzx.com/gtpwtlnbsb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtoaemjylq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.hywenlv.cn/gtamdgckpz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.jinyuanbaomall.cn/gtjkyqjtgh.html

Java: list.size();  map.size();  s.length()
来源：http://hz.guowangkeji.top/gtcnmeljej.html

Go:   len(arr);  len(m)
来源：http://hz.fengsongda.top/gtrkzzmwpt.html

Ruby: x.length;  x.size
来源：http://hz.aibaodan.cn/gtsgxdubpb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.meibo888.top/gtkqpxtvyf.html

[P05] 判断两个对象内容是否相等
来源：http://hz.jianghu66.top/gtndhugwvf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.nanxuanxn.top/gtpoknwltf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.vqdsnc.cn/gtuxawvtdz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.daxiang520.top/gtiomhmpmp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.bjfxy.top/gtxbnaloue.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.yonumen.top/gtjkexpedw.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.hfpthk.cn/gtycjppqtu.html

Ruby: a == b
来源：http://hz.yj202588.top/gtivjahjvv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.vqdsnc.cn/gtmodyvwvx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhaomingkeji.xyz/gtbpukgtxp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.ivvv.top/gtzqerkiqp.html

PHP:  if (empty($x)) {}
来源：http://hz.gaohongyu789.top/gtcmpgziwt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.ywan-chungtsiang.top/gtefzlgekd.html

TS:   if (x == null) {}
来源：http://hz.hywenlv.cn/gtejsegslm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.svipenyu.cn/gtalpwxtvf.html

Go:   if x == nil {}
来源：http://hz.52xcode.cn/gtattrlexl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.chenjidiqi.icu/gtlsqtjeak.html

C#:   if (x is null) {}
来源：http://hz.guannengcc.top/gtwasoedos.html

[P07] 防抖与节流
来源：http://hz.jqgufenzy.top/gtxonxvpvu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.tanke756.top/gtjsjdnwco.html

PHP:  // 手写时间戳比较
来源：http://hz.aizwys.cn/gtxbzrlzfh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtaipohrks.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydzc1.top/gtxlrgbgun.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.zdqjudy.top/gttluuuvay.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.chenlongwang.top/gtthnqrvcq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.wangshuangyany.cn/gtxaqwjvmu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.shzxlz.cn/gtkbywgnjf.html

[P08] 处理浮点精度问题
来源：http://hz.gzhubu.top/gtoiqlxucp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.jianghu66.top/gtlwvjduiy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.yonumen.top/gtzhzfqreg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.nanxinkj.top/gtmhigkyxr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.cashguo.top/gtakuisxky.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.haohaochexian.top/gtkilfxecx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.redwolf501.top/gtozjeyhyv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.meibo888.top/gtgdiwrzxc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.yvedp.cn/gtkdarhkff.html

================================================================================
来源：http://hz.zhixingplan.top/gtkrcclste.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.snrcjt.cn/gtlreirztu.html

================================================================================
来源：http://hz.cashguo.top/gtocsqfsui.html

[Q01] 创建表
来源：http://hz.xziqi.cn/gtesgpwfew.html

CREATE TABLE users (
来源：http://hz.c1oappe.top/gtzwtodwqw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.guowangkeji.top/gtmvjiokrc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.iojbl.cn/gtwmiiwxws.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jqgufenzy.top/gtaxoquyqs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.xziqi.cn/gttlvpljai.html

);
来源：http://hz.zhijiandao.cn/gtsliaievp.html

[Q02] 创建带外键的表
来源：http://hz.jinyuanbaomall.cn/gtzfzpujse.html

CREATE TABLE orders (
来源：http://hz.jinyuanbaomall.cn/gtnplsxjbn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cashguo.top/gtrscyiexf.html

user_id INT NOT NULL,
来源：http://hz.yueranfly.top/gtedgxpxeb.html

amount DECIMAL(10, 2),
来源：http://hz.shanyushiyangkeji.top/gtbixjqczj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jyoumei.cn/gtowbnhjdn.html

);
来源：http://hz.yangfankeji.com/gtyaiaxlay.html

[Q03] 增加列
来源：http://hz.tianlin.xyz/gtgptudgbs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.shanyushiyangkeji.top/gtpcljoyqc.html

[Q04] 修改列类型
来源：http://hz.jianghu66.top/gtydarnuns.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.gzhubu.top/gtmyzdfobx.html

[Q05] 重命名列
来源：http://hz.cqqwz.cn/gtlnqoylpz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.zhaomingkeji.xyz/gtflafljfr.html

[Q06] 删除列
来源：http://hz.pycfn.com/gtsildymrj.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.tianlin.xyz/gtbwyxwfwd.html

[Q07] 删除表
来源：http://hz.wangdashe.top/gtobyykwil.html

DROP TABLE IF EXISTS orders;
来源：http://hz.ehwqpu.com/gtfvnlwtkb.html

[Q08] 创建普通索引
来源：http://hz.ydzc1.top/gtwnhskpbl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.iojbl.cn/gthlexqugf.html

[Q09] 创建唯一索引
来源：http://hz.jqgfzy.top/gtlraitkim.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.chenlongwang.top/gtkpitlwsb.html

[Q10] 插入单行
来源：http://hz.jinyuanbaomall.cn/gtmvehkhai.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.fengsongda.top/gtkoqimgsa.html

[Q11] 一次插入多行
来源：http://hz.zhoulong.xyz/gtklnwaggz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.wangdashe.top/gtvdqkjcnb.html

[Q12] 插入后取自增 ID
来源：http://hz.gaohongyu789.top/gtgxmzssdj.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.jinqigfzy.top/gtvnnphfvz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.c1oappe.top/gtsqajqxtp.html

[Q13] 忽略重复插入
来源：http://hz.tanke756.top/gtypnnxgjl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.chenjidiqi.icu/gtgrphydsh.html

[Q14] 存在则更新（upsert）
来源：http://hz.jlsjyb.cn/gthrefochr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ivvv.top/gteamiizvi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.chenlongwang.top/gtwxbckjnl.html

[Q15] 查询全部
来源：http://hz.iojbl.cn/gtaauijssz.html

SELECT * FROM users;
来源：http://hz.yvedp.cn/gtzbmjsbht.html

[Q16] 查询指定列
来源：http://hz.wangshuangyany.cn/gtgdfsdcrl.html

SELECT id, name FROM users;
来源：http://hz.zhixingplan.top/gtmdraspse.html

[Q17] 条件查询
来源：http://hz.yuanzhike.top/gttzvemhdr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ybcxt.top/gtixaszajh.html

[Q18] 模糊匹配
来源：http://hz.chenjidiqi.icu/gtyoiwjxpx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.316326.xyz/gtxgqtrurj.html

[Q19] 范围查询
来源：http://hz.smart0.xyz/gthxlpzaic.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhengqikj.top/gtylqdxrpl.html

[Q20] IN 列表
来源：http://hz.hnxiangtu.top/gtslyjymuw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhixingplan.top/gteymnfrgt.html

[Q21] 空值判断
来源：http://hz.shangyingyoupin.top/gtkmtwlvsg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gogol.net.cn/gthirlsdhb.html

[Q22] 排序
来源：http://hz.zdqjudy.top/gtlgojkqon.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xingfuxueyuan.xyz/gtbpsiqxys.html

[Q23] 分页
来源：http://hz.iojbl.cn/gtzjdjzzmg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.hnqzz.top/gtvahcaaoe.html

[Q24] 去重
来源：http://hz.daria6918.cn/gtlzhehnhx.html

SELECT DISTINCT city FROM users;
来源：http://hz.hnxiangtu.top/gtvrzkfjbb.html

[Q25] 只取前 N 条
来源：http://hz.nanxuanxn.top/gtwdiheecv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.hammf.cn/gtpquurwvi.html

[Q26] 计数
来源：http://hz.zhaomingkeji.xyz/gtvoatdkac.html

SELECT COUNT(*) FROM users;
来源：http://hz.gotoacloud.top/gtkktfoemi.html

[Q27] 条件计数
来源：http://hz.shanyushiyangkeji.top/gtxxfvwcfj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aibaodan.cn/gtscptotgi.html

[Q28] 求和与平均
来源：http://hz.havefunace.top/gtikuxjnvl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.guannengcc.top/gtpghoykoc.html

[Q29] 最大最小值
来源：http://hz.nanxuanxn.top/gtcmkgprgx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.dashuyun.cn/gttlplnznj.html

[Q30] 分组统计
来源：http://hz.shuidangran.top/gtejzenbye.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtpvvkxclm.html

[Q31] 分组后过滤
来源：http://hz.havefunace.top/gtkvsuzbcx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhongyouzk.top/gtvsykcnfe.html

[Q32] 分组拼接字符串
来源：http://hz.gotoacloud.top/gtcibrqldp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtnlwqelui.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.quarkkingdee.top/gttaaivqil.html

[Q33] 多列分组
来源：http://hz.ybcxt.top/gtaizuaxgi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnqzz.top/gteisbkgkg.html

[Q34] 每组取第一条
来源：http://hz.ehwqpu.com/gtuciwfwsp.html

SELECT * FROM (
来源：http://hz.jiagoushi.top/gtmebnhqqr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.smart0.xyz/gteduzwvrb.html

) t WHERE rn = 1;
来源：http://hz.yj20258.top/gtsdrpznix.html

[Q35] 内连接
来源：http://hz.chenjidiqi.icu/gtbmsrknmu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtcyvitwsm.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gthqgowboj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.fzhhl.top/gtyybdnvze.html

[Q37] 右连接
来源：http://hz.9152youxi.cn/gtxcfzshgh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ywan-chungtsiang.top/gteivptynj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtzwfhidje.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtpdcpjyzd.html

[Q39] 自连接（查上下级）
来源：http://hz.shangyingyoupin.top/gtjmfbenad.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.vqdsnc.cn/gtozqjrigo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tianlin.xyz/gtxkvlstfn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cdnleiting.top/gtlpwnfotn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.dashuyun.cn/gtpkcduqqg.html

[Q41] 多表连接
来源：http://hz.cucudq.cn/gtuwytopaz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zycfv.cn/gtkuqlaaii.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ydzc1.top/gtydcbofbj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yvedp.cn/gtgvrmdobj.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxuanxn.top/gteuxbgbhq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.svipenyu.cn/gtuesowwzw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tian-w.cn/gtdgetvits.html

[Q43] 标量子查询
来源：http://hz.hammf.cn/gtbsehrfsp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.fengsongda.top/gtxkzxauhr.html

[Q44] IN 子查询
来源：http://hz.ybcxt.top/gtvnxkhtxd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shuidangran.top/gtgiuywztp.html

[Q45] EXISTS 判断存在
来源：http://hz.hywenlv.cn/gttmsvwutx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtjhupbjsj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yj20258888.top/gtsylajiwe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtpfdxqpco.html

[Q47] 与平均值比较
来源：http://hz.gaohongyu789.top/gttkxgtpri.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gtjzaiipwh.html

[Q48] CTE 公用表表达式
来源：http://hz.yj202588.top/gtztipbavb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.xziqi.cn/gtbjfueoxw.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.52xcode.cn/gtndkxhdlc.html

[Q49] 更新单行
来源：http://hz.shuidangran.top/gtpmtlpbcb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtalcexiwb.html

[Q50] 批量更新
来源：http://hz.shzxlz.cn/gtwnkxgepi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhoulong.xyz/gtfgpazsxm.html

[Q51] 用子查询更新
来源：http://hz.yvedp.cn/gtixwolyrk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cucudq.cn/gtwsjjcomz.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gtypgvwgks.html

DELETE FROM users WHERE id = 10;
来源：http://hz.daxiang520.top/gtqnlncriv.html

[Q53] 按条件删除
来源：http://hz.ydzc1.top/gtqppikbgl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtocibxnkc.html

[Q54] 清空表
来源：http://hz.yuxming.cn/gttnepznpn.html

TRUNCATE TABLE logs;
来源：http://hz.jlsjyb.cn/gtjvqfopkf.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtsrvpdbdg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hongshengwenyu.top/gtoqixlkks.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jiagoushi.top/gtadttapia.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.tanke756.top/gtdrrwmala.html

[Q57] 行号
来源：http://hz.gzhubu.top/gtdvlulxse.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinghuilouyu.cn/gtmvrzwmer.html

[Q58] 累计求和
来源：http://hz.ydzc1.top/gtzxkmzzgx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.vqdsnc.cn/gtbfavmtaa.html

[Q59] 分组内累计
来源：http://hz.yj202588.top/gtynktbnvq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.kuanghao11.cn/gtuxtpdvia.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gtimdpoeuq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.mhx1999.top/gtlcropnza.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jiagoushi.top/gtqrcubach.html

[Q61] 移动平均
来源：http://hz.fzhhl.top/gtqseceqca.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yonumen.top/gtxyrkmbpr.html

[Q62] 分组占比
来源：http://hz.jianghu66.top/gtasfaonlo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtgwqizdoi.html

[Q63] 开启事务
来源：http://hz.feifeiyinyue.top/gtbtcnnxqr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtbcivklsi.html

[Q64] 提交事务
来源：http://hz.shanyushiyangtech.top/gtcfdlfxzu.html

COMMIT;
来源：http://hz.nwbrower.top/gtsbzvnvfr.html

[Q65] 回滚事务
来源：http://hz.feifeiyinyue.top/gtgjevknis.html

ROLLBACK;
来源：http://hz.pycfn.com/gtocmpjkqb.html

[Q66] 行锁查询
来源：http://hz.xuanzx.com/gtiizlxfbl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ppjwa.cn/gtsebrssak.html

[Q67] 设置隔离级别
来源：http://hz.redwolf501.top/gtpzyhmeco.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.haohaochexian.top/gtdasdsulh.html

[Q68] 保存点
来源：http://hz.guowangkeji.top/gtenaraowv.html

SAVEPOINT sp1;
来源：http://hz.haohaochexian.top/gtdkxafyme.html

ROLLBACK TO sp1;
来源：http://hz.jlsjyb.cn/gtkurnalqj.html

[Q69] 查看执行计划
来源：http://hz.shangyingyoupin.top/gtugmbkrrq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gtwzbktnfz.html

[Q70] 更新统计信息
来源：http://hz.guannengcc.top/gtgmbtzzdy.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtzlxblllb.html

[Q71] 查看建表语句
来源：http://hz.havefunace.top/gtjpeolwiu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.0kj1m.cn/gtkkehwlzf.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtocwhgivg.html

SHOW INDEX FROM users;
来源：http://hz.gaohongyu789.top/gtcsadmlfq.html

[Q73] 查看表状态
来源：http://hz.zhengqikj.top/gtbtycfzta.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.0kj1m.cn/gtxbmltvxy.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gtjmwsletp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhijiandao.cn/gtvjtqfpdf.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gtytgzpgfa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aizwys.cn/gtlteuqnkw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.smart0.xyz/gtgumhqeet.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gtukasalfp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yongpay.top/gtibexwpua.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtlfmvtudh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gtfwejiswd.html

[Q78] 当前时间
来源：http://hz.jianghu66.top/gtsnjibnor.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dashuyun.cn/gttaqtrygw.html

[Q79] 字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtmiksvezt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tanke756.top/gtrdslicwy.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gtzwpgmwzm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tian-w.cn/gtnshevupd.html

[Q81] 字符串替换
来源：http://hz.ydjk.org.cn/gtwriqibrg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xylfe.cn/gtedljlkmg.html

[Q82] 字符长度与字节长度
来源：http://hz.cucudq.cn/gtfqenfwiv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gthqfyrqpc.html

[Q83] 大小写转换
来源：http://hz.xylfe.cn/gtdezcjbaj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhixingplan.top/gtjgghstrl.html

[Q84] 去除首尾空格
来源：http://hz.havefunace.top/gtfuujurix.html

SELECT TRIM(name) FROM users;
来源：http://hz.yvedp.cn/gttxpbkdrx.html

[Q85] 数值取整
来源：http://hz.jqgfzy.top/gtwqlxymfc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtppbdompw.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtursmatxu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shanyushiyangkeji.top/gtadutzabu.html

[Q87] JSON 字段做条件
来源：http://hz.sysykeji.top/gtmzatrrax.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xylfe.cn/gtmplhcwtr.html

[Q88] 行转列（条件聚合）
来源：http://hz.yvedp.cn/gtygoanhtn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtehezjrmi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yuanzhike.top/gtwemvxedc.html

[Q89] 判断表是否存在
来源：http://hz.fzhhl.top/gtocgjfkad.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shuidangran.top/gtgcfnhvcb.html

[Q90] 生成序号列
来源：http://hz.zdqjudy.top/gtxadqtrvl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtvcumejvb.html

================================================================================
来源：http://hz.snrcjt.cn/gtvzkaaatw.html

R. Bash 专题
来源：http://hz.shanyushiyangkeji.top/gtmjmbhavt.html

================================================================================
来源：http://hz.gzhubu.top/gtjqntuoyd.html

[R01] shebang 与严格模式
来源：http://hz.xziqi.cn/gtorhytttr.html

#!/usr/bin/env bash
来源：http://hz.zhaomingkeji.xyz/gtmlxzioxv.html

set -euo pipefail
来源：http://hz.316326.xyz/gtavyvqisr.html

[R02] 变量赋值与使用
来源：http://hz.xingfuxueyuan.xyz/gtqjjmxksy.html

name="Tom"; echo "$name"
来源：http://hz.mhx1999.top/gtlmrmkfdc.html

[R03] 只读变量
来源：http://hz.quarkkingdee.top/gtqrgybmjp.html

readonly PI=3.14
来源：http://hz.yongpay.top/gtvjanlskf.html

[R04] 位置参数
来源：http://hz.xziqi.cn/gtkcvgmnvt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.9152youxi.cn/gtsfmhuotl.html

[R05] 参数默认值
来源：http://hz.xinyue.icu/gtftpepyvv.html

name="${1:-default}"
来源：http://hz.shanyushiyangkeji.top/gtolpcntfs.html

[R06] 判断命令是否存在
来源：http://hz.jiagoushi.top/gtdjdmcikf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yanxiufei.cn/gtlziztyqu.html

[R07] if 判断文件
来源：http://hz.aibaodan.cn/gtblbccoon.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gtrusoukmb.html

[R08] 数值比较
来源：http://hz.ivvv.top/gtltjjkfdx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xylfe.cn/gtrpxiaegf.html

[R09] 字符串比较
来源：http://hz.zycfv.cn/gtvbxrofvq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.9152youxi.cn/gtjmssemee.html

[R10] 正则匹配
来源：http://hz.birdmap.top/gtillnwitv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yongpay.top/gtfsewtknt.html

[R11] case 多分支
来源：http://hz.cashguo.top/gtuawdwddr.html

case "$1" in
来源：http://hz.pengpengdd.cyou/gtrbwqqkgm.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtfejkmncq.html

stop)  echo "停止" ;;
来源：http://hz.yueranfly.top/gtjxdcwelo.html

*)     echo "未知命令" ;;
来源：http://hz.fengsongda.top/gtnyywidlg.html

esac
来源：http://hz.chenlongwang.top/gtkhphytro.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtfvoybxow.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tian-w.cn/gtcwmguwxb.html

[R13] for 计数循环
来源：http://hz.shuidangran.top/gtejtymrha.html


<!-- 参考信息 -->