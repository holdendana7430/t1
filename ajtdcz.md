代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangdashe.top/gttaepeger.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gogol.net.cn/gtcdrxjfek.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj202588.top/gtcfmofqti.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jlsjyb.cn/gtocikjhze.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.ywan-chungtsiang.top/gtggkjawur.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hfpthk.cn/gtyppzekql.html

[P03] 生成短随机字符串
来源：http://hz.hywenlv.cn/gtvsxvltmn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtfgighfcz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.zhongyouzk.top/gtonxtdnnw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj20258.top/gtfcbosolw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yonumen.top/gtpuiigkwc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yuxming.cn/gtwefduqkl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.quarkkingdee.top/gtieiuhgcu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ydjk.org.cn/gtjivwplpg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.svipenyu.cn/gtcrlmnsvh.html

[P04] 求长度
来源：http://hz.jyoumei.cn/gteucgdavj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.gaohongyu789.top/gtydzsjywt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtjmszryep.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.redwolf501.top/gtejdfngur.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shzxlz.cn/gttpsaaqkk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.mhx1999.top/gtmghukoun.html

Go:   len(arr);  len(m)
来源：http://hz.316326.xyz/gtqhmjwrue.html

Ruby: x.length;  x.size
来源：http://hz.nanxinkj.top/gtxtjvqukg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.hnqzz.top/gtwcrwofui.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yongpay.top/gtbikuqaaa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.sxryk.cn/gtlmvzocth.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.shangyingyoupin.top/gtdepzxtjg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.yuanzhike.top/gttwyvzgzl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ywan-chungtsiang.top/gtdknysdac.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.cucudq.cn/gtkucuyclx.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.xuetiantiany.cn/gtznbxtzxp.html

Ruby: a == b
来源：http://hz.jyoumei.cn/gtgpvqbzqv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.yj202588.top/gtkzblircb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.fzhhl.top/gtiqfacwuo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.aizwys.cn/gtimstecev.html

PHP:  if (empty($x)) {}
来源：http://hz.jinqigfzy.top/gteoyanpqo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.smart0.xyz/gtftmaeqsz.html

TS:   if (x == null) {}
来源：http://hz.tianlin.xyz/gtdtgwoyqk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.vqdsnc.cn/gtyeglubqc.html

Go:   if x == nil {}
来源：http://hz.shangyingyoupin.top/gtvyxzfkzu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.xziqi.cn/gtsoshuasl.html

C#:   if (x is null) {}
来源：http://hz.bjfxy.top/gtmhqqcjug.html

[P07] 防抖与节流
来源：http://hz.sxryk.cn/gtojvwfbyg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.gzhubu.top/gtdqlgarqg.html

PHP:  // 手写时间戳比较
来源：http://hz.yongpay.top/gthhwmjwgb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.smart0.xyz/gtodeqmteo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtstamajrn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.nwbrower.top/gtaunmtsey.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.daria6918.cn/gtabdjjtys.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.yangfankeji.com/gtbjdsfmvj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.0kj1m.cn/gtxkjnptla.html

[P08] 处理浮点精度问题
来源：http://hz.wangshuangyany.cn/gttgwcclpx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.vqdsnc.cn/gtotjgjcor.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.zhixingplan.top/gtnffciukg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.dianchejie.cn/gtbkaunnld.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.kuanghao11.cn/gteypfqouk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.havefunace.top/gtnwvhbkfs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.snrcjt.cn/gtssriqvzc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.kuanghao11.cn/gtevrnotlo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.nanxinkj.top/gtuwmziryb.html

================================================================================
来源：http://hz.zhengqikj.top/gtzucghoaa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.cdnleiting.top/gtwfqweodx.html

================================================================================
来源：http://hz.yuanzhike.top/gtsqoglbwg.html

[Q01] 创建表
来源：http://hz.gotoacloud.top/gtmtddkloe.html

CREATE TABLE users (
来源：http://hz.hysaishi.cn/gtnvpurrkp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.xingfuxueyuan.xyz/gtcsybjapc.html

name VARCHAR(50) NOT NULL,
来源：http://hz.pycfn.com/gtvzqkwnel.html

email VARCHAR(100) UNIQUE,
来源：http://hz.sxryk.cn/gtauvnshlv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.ppjwa.cn/gtgtmrvwwd.html

);
来源：http://hz.guowangkeji.top/gtlfqepipp.html

[Q02] 创建带外键的表
来源：http://hz.quarkkingdee.top/gtlyfxbabi.html

CREATE TABLE orders (
来源：http://hz.nanxinkj.top/gtgqyuadff.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.9152youxi.cn/gtyecbymsf.html

user_id INT NOT NULL,
来源：http://hz.birdmap.top/gtemfnuakq.html

amount DECIMAL(10, 2),
来源：http://hz.zdqjudy.top/gtjbvrervu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.yuxming.cn/gtvuxptcbi.html

);
来源：http://hz.shuidangran.top/gtkulalikp.html

[Q03] 增加列
来源：http://hz.nanxuanxn.top/gtarssgtsa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.cdnleiting.top/gthxbblfru.html

[Q04] 修改列类型
来源：http://hz.gzhubu.top/gtbxolwzia.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.aizwys.cn/gtbppmnvqk.html

[Q05] 重命名列
来源：http://hz.gzhubu.top/gtmlrllyzk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.aizwys.cn/gttwlvdwzb.html

[Q06] 删除列
来源：http://hz.ybcxt.top/gtwnsuczbr.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.jyoumei.cn/gtpfqdrbjm.html

[Q07] 删除表
来源：http://hz.zhongyouzk.top/gtelihfkks.html

DROP TABLE IF EXISTS orders;
来源：http://hz.aizwys.cn/gtgztwvnbe.html

[Q08] 创建普通索引
来源：http://hz.jlsjyb.cn/gtnqkjgprn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.yueranfly.top/gtdendmnyi.html

[Q09] 创建唯一索引
来源：http://hz.redwolf501.top/gtegyyswpi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.cucudq.cn/gtfjxqabms.html

[Q10] 插入单行
来源：http://hz.mhx1999.top/gtjdlquwst.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.cdnleiting.top/gtqbdgrmrg.html

[Q11] 一次插入多行
来源：http://hz.yj20258.top/gtpspsmdzy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtiwqgzhgs.html

[Q12] 插入后取自增 ID
来源：http://hz.kuanghao11.cn/gtxlrtgdes.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhaomingkeji.xyz/gtwsachuvr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.hywenlv.cn/gtczlidwti.html

[Q13] 忽略重复插入
来源：http://hz.zdqjudy.top/gtzpksyqty.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.gzhubu.top/gtdraqkmsa.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gtifhktsre.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cashguo.top/gtshdjwqtk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.yonumen.top/gtrstmdogw.html

[Q15] 查询全部
来源：http://hz.gaohongyu789.top/gtrsepmupq.html

SELECT * FROM users;
来源：http://hz.ppjwa.cn/gtejvqjfrs.html

[Q16] 查询指定列
来源：http://hz.shanyushiyangkeji.top/gtpmfylcus.html

SELECT id, name FROM users;
来源：http://hz.yuanzhike.top/gtomwcbpvg.html

[Q17] 条件查询
来源：http://hz.mhx1999.top/gtzsqrmcpr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hnqzz.top/gtailklsjb.html

[Q18] 模糊匹配
来源：http://hz.sufxvd.cn/gttlseqreu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.andypj.xyz/gtcvrzmbxm.html

[Q19] 范围查询
来源：http://hz.haohaochexian.top/gtkstsyngq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.quarkkingdee.top/gtidtffwex.html

[Q20] IN 列表
来源：http://hz.quarkkingdee.top/gtmxgzyufz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.snrcjt.cn/gteirrafxk.html

[Q21] 空值判断
来源：http://hz.jlsjyb.cn/gtmvkyumqm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gaohongyu789.top/gtjxrbdzpc.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gtlmvrimol.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hnxiangtu.top/gtchfxxege.html

[Q23] 分页
来源：http://hz.dashuyun.cn/gtzaocuwvr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuxming.cn/gtledcnama.html

[Q24] 去重
来源：http://hz.chenzaomai.com/gtwyyuqncz.html

SELECT DISTINCT city FROM users;
来源：http://hz.daria6918.cn/gtukkpqucq.html

[Q25] 只取前 N 条
来源：http://hz.hammf.cn/gtltrnfyej.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jlsjyb.cn/gtonzqdfnl.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtuvvxruqs.html

SELECT COUNT(*) FROM users;
来源：http://hz.gotoacloud.top/gtfwllfjtj.html

[Q27] 条件计数
来源：http://hz.gotoacloud.top/gtpswotycm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.hammf.cn/gttcfrsbqn.html

[Q28] 求和与平均
来源：http://hz.guowangkeji.top/gticgfvdwf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.chenzaomai.com/gtxhavnfcf.html

[Q29] 最大最小值
来源：http://hz.0kj1m.cn/gtriegrhbj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xziqi.cn/gtxmkfwfyc.html

[Q30] 分组统计
来源：http://hz.hysaishi.cn/gtoxyleziq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xuetiantiany.cn/gtrfvnzygm.html

[Q31] 分组后过滤
来源：http://hz.yueranfly.top/gtxrvkvlck.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.jinqigfzy.top/gtbeqpypeu.html

[Q32] 分组拼接字符串
来源：http://hz.jianghu66.top/gtwcqmlzkv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtekzyzeds.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtoziqkrog.html

[Q33] 多列分组
来源：http://hz.gzhubu.top/gtxdwldrin.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.chenlongwang.top/gtepoybpaa.html

[Q34] 每组取第一条
来源：http://hz.jinqigufen.top/gtoqytqmcu.html

SELECT * FROM (
来源：http://hz.sxryk.cn/gtlkmqnuye.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xingfuxueyuan.xyz/gtlaxkrksq.html

) t WHERE rn = 1;
来源：http://hz.quarkkingdee.top/gtrfckegih.html

[Q35] 内连接
来源：http://hz.haohaochexian.top/gtiddtxatb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtklugqtjz.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtbmcuqhnt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtdjfflbcb.html

[Q37] 右连接
来源：http://hz.kuanghao11.cn/gtbbikxayl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ybcxt.top/gtcdfmbmjq.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.havefunace.top/gtfburuazo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.snrcjt.cn/gtxipnoajp.html

[Q39] 自连接（查上下级）
来源：http://hz.shzxlz.cn/gthnxrmxmb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.9152youxi.cn/gtpatxwlla.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gteqwxoakz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cashguo.top/gtvwrsvfbs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhixingplan.top/gtqdtpunbi.html

[Q41] 多表连接
来源：http://hz.jiagoushi.top/gtslijkcds.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtmhetjpmi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.316326.xyz/gttqtekmzp.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtolqfdzjs.html

[Q42] 连接条件附加过滤
来源：http://hz.dashuyun.cn/gtavsdgpjs.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aibaodan.cn/gtiozvpmig.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yj202588.top/gtoiqxfhso.html

[Q43] 标量子查询
来源：http://hz.zhaomingkeji.xyz/gtmmvfiyax.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jianghu66.top/gtfktpomfm.html

[Q44] IN 子查询
来源：http://hz.cheryme.top/gtqbaopqiw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yonumen.top/gtopccprmp.html

[Q45] EXISTS 判断存在
来源：http://hz.jinghuilouyu.cn/gtjdrowjwd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtstiehiac.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.zhiwuduotai.top/gtldewxjso.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtakqkqrul.html

[Q47] 与平均值比较
来源：http://hz.fzhhl.top/gtsbrnofun.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhijiandao.cn/gtvalljkgd.html

[Q48] CTE 公用表表达式
来源：http://hz.zhixingplan.top/gtzvsqixju.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangtech.top/gtrrqfaakh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.haohaochexian.top/gtpskszxst.html

[Q49] 更新单行
来源：http://hz.jinyuanbaomall.cn/gtoraogdtd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtptlyngvz.html

[Q50] 批量更新
来源：http://hz.jinghuilouyu.cn/gtbuqbblks.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yongpay.top/gtvpahzcxg.html

[Q51] 用子查询更新
来源：http://hz.cdnleiting.top/gtrjqnwoen.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtiidqcghw.html

[Q52] 删除指定行
来源：http://hz.nanxinkj.top/gtvbcbywbp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.feifeiyinyue.top/gtsiqlzngw.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtbgrmjsea.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.jqgfzy.top/gtsuvlxwjc.html

[Q54] 清空表
来源：http://hz.aibaodan.cn/gttzhubiil.html

TRUNCATE TABLE logs;
来源：http://hz.316326.xyz/gtcujjoaef.html

[Q55] 排名（并列占位）
来源：http://hz.9152youxi.cn/gtcqqlabmf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gogol.net.cn/gtmulnsifa.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gotoacloud.top/gtfydizbir.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.9152youxi.cn/gtlpvkocwu.html

[Q57] 行号
来源：http://hz.feifeiyinyue.top/gtllssmjtc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ydjk.org.cn/gtramulmsz.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gtwslfphus.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yueranfly.top/gtdfezfbij.html

[Q59] 分组内累计
来源：http://hz.hongshengwenyu.top/gtbnozsklj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gttamphpnk.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gtnpdmtkey.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cucudq.cn/gtyjyczoal.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhijiandao.cn/gtoejbqyxw.html

[Q61] 移动平均
来源：http://hz.tian-w.cn/gtzbonsmfx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xuanzx.com/gtartgalaa.html

[Q62] 分组占比
来源：http://hz.yuxming.cn/gthuicpvoe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhijiandao.cn/gtuqeicjwi.html

[Q63] 开启事务
来源：http://hz.zhoulong.xyz/gterlxlxao.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydzc1.top/gtytiuwjbb.html

[Q64] 提交事务
来源：http://hz.yvedp.cn/gthvkbxbhn.html

COMMIT;
来源：http://hz.zdqjudy.top/gtegtosieb.html

[Q65] 回滚事务
来源：http://hz.shzxlz.cn/gtlyojedbi.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtkjvjlptm.html

[Q66] 行锁查询
来源：http://hz.chenjidiqi.icu/gtegfxmakh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.ehwqpu.com/gtlfmfbqbf.html

[Q67] 设置隔离级别
来源：http://hz.yj20258.top/gtggadygop.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangkeji.top/gtshvluitt.html

[Q68] 保存点
来源：http://hz.yj202588.top/gtusaouyqi.html

SAVEPOINT sp1;
来源：http://hz.ywan-chungtsiang.top/gtyovvimmc.html

ROLLBACK TO sp1;
来源：http://hz.shangyingyoupin.top/gtfxdbldnd.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtrnuorhyd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xinyue.icu/gtazhsxfzw.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtuiriziul.html

ANALYZE TABLE users;
来源：http://hz.xingfuxueyuan.xyz/gtbabxqqjn.html

[Q71] 查看建表语句
来源：http://hz.tian-w.cn/gtxzkweapy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtwhsxnaaa.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtwbaakrdm.html

SHOW INDEX FROM users;
来源：http://hz.kuanghao11.cn/gtxblxyvpq.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangkeji.top/gtvrknftbh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dianchejie.cn/gtnqguylzl.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gtczppqrrx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jyoumei.cn/gtkablgefx.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtwcrbdozj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yueranfly.top/gtohkfvbxb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cashguo.top/gtfltfayxj.html

[Q76] 按天统计
来源：http://hz.hnxiangtu.top/gtaomyyvtk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dashuyun.cn/gthjkjeyyn.html

[Q77] 时间加减
来源：http://hz.sweek.top/gtwusievsm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtcyuailzb.html

[Q78] 当前时间
来源：http://hz.nanxuanxn.top/gthsktxgkx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yueranfly.top/gtnjerkepd.html

[Q79] 字符串拼接
来源：http://hz.xuanzx.com/gtsbgunjuy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtyebiopij.html

[Q80] 字符串截取
来源：http://hz.yuxming.cn/gtymrvpbfa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxuanxn.top/gtxoaawexx.html

[Q81] 字符串替换
来源：http://hz.hywenlv.cn/gtcvslzfql.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinyuanbaomall.cn/gtsaqqlcws.html

[Q82] 字符长度与字节长度
来源：http://hz.daxiang520.top/gtquuibxxl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cucudq.cn/gtekihljms.html

[Q83] 大小写转换
来源：http://hz.316326.xyz/gtpceneszn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtbrzqcawz.html

[Q84] 去除首尾空格
来源：http://hz.wangshuangyany.cn/gtjijhmpbi.html

SELECT TRIM(name) FROM users;
来源：http://hz.gzhubu.top/gtqnfspips.html

[Q85] 数值取整
来源：http://hz.zhiwuduotai.top/gtgvlusekb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sxryk.cn/gtawhlxawe.html

[Q86] 读取 JSON 字段
来源：http://hz.jinyuanbaomall.cn/gtfpktvqbs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shuidangran.top/gtvvsrgsji.html

[Q87] JSON 字段做条件
来源：http://hz.cucudq.cn/gtuojctfwn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aibaodan.cn/gtgvdedgfv.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gtsswyhroj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtammitoic.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.smart0.xyz/gtzswceyun.html

[Q89] 判断表是否存在
来源：http://hz.jinqigfzy.top/gtsnkzqxpq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgufenzy.top/gtatlkhkri.html

[Q90] 生成序号列
来源：http://hz.gogol.net.cn/gtaodpnimh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gtuyamgums.html

================================================================================
来源：http://hz.chenzaomai.com/gtnnbatyvi.html

R. Bash 专题
来源：http://hz.xuanzx.com/gtjtqouxqn.html

================================================================================
来源：http://hz.shuidangran.top/gtumwlhkhk.html

[R01] shebang 与严格模式
来源：http://hz.zhongyouzk.top/gtnleagfrc.html

#!/usr/bin/env bash
来源：http://hz.sufxvd.cn/gtjkkystcn.html

set -euo pipefail
来源：http://hz.guowangkeji.top/gthhvzdaia.html

[R02] 变量赋值与使用
来源：http://hz.xuetiantiany.cn/gtccgjsubc.html

name="Tom"; echo "$name"
来源：http://hz.mhx1999.top/gtwwwonisf.html

[R03] 只读变量
来源：http://hz.jinyuanbaomall.cn/gtskrcgjil.html

readonly PI=3.14
来源：http://hz.shzxlz.cn/gtbzpdwrmf.html

[R04] 位置参数
来源：http://hz.hysaishi.cn/gtuknpages.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tian-w.cn/gtqtnlvmiu.html

[R05] 参数默认值
来源：http://hz.chenjidiqi.icu/gthncavzra.html

name="${1:-default}"
来源：http://hz.vqdsnc.cn/gtqkcmlwrm.html

[R06] 判断命令是否存在
来源：http://hz.yuanzhike.top/gtczatoisb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.aizwys.cn/gtlpgoaxpk.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gthnjaxewm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gthscwjnor.html

[R08] 数值比较
来源：http://hz.hnqzz.top/gtpnafrqrd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yongpay.top/gtatreiadf.html

[R09] 字符串比较
来源：http://hz.yj20258.top/gtckjygtej.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fengsongda.top/gtzqsxfpns.html

[R10] 正则匹配
来源：http://hz.zhengqikj.top/gtwexvgdrr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtwggfdiax.html

[R11] case 多分支
来源：http://hz.zhoulong.xyz/gtwvxdjqnd.html

case "$1" in
来源：http://hz.yongpay.top/gtcknaoamk.html

start) echo "启动" ;;
来源：http://hz.jqgfzy.top/gtcwosqgdb.html

stop)  echo "停止" ;;
来源：http://hz.birdmap.top/gtacokhlya.html

*)     echo "未知命令" ;;
来源：http://hz.xylfe.cn/gtsulcsgal.html

esac
来源：http://hz.nanxuanxn.top/gtysomkeho.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gthgzqobde.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtfnyaapzw.html

[R13] for 计数循环
来源：http://hz.0kj1m.cn/gthjcdhsgb.html


<!-- 参考信息 -->