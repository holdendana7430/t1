代发 wailian999

[P01] 生成 UUID
来源：http://hz.pengpengdd.cyou/gtxdudagsb.html

Py:   str(uuid.uuid4())
来源：http://hz.cqqwz.cn/gtvaaiwhqz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.9152youxi.cn/gtwrxpaism.html

JS:   crypto.randomUUID()
来源：http://hz.yuxming.cn/gtlkfspgui.html

TS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtewqgtuqb.html

Java: UUID.randomUUID().toString()
来源：http://hz.yj20258.top/gtjczfljxc.html

Go:   // 用 github.com/google/uuid
来源：http://hz.shangyingyoupin.top/gtawmhvcwb.html

Ruby: SecureRandom.uuid
来源：http://hz.hywenlv.cn/gtyuogjupp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zhongyouzk.top/gtnaxayxqe.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yanxiufei.cn/gtqybiucus.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ehwqpu.com/gtyfshlaxk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jlsjyb.cn/gtgdpawtyy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zhiwuduotai.top/gtpunxptee.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinghuilouyu.cn/gttwywoegl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhixingplan.top/gtxansgexf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.sweek.top/gtuxzkjfbx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hywenlv.cn/gtclaeiyru.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.gogol.net.cn/gtjgumzlzy.html

[P03] 生成短随机字符串
来源：http://hz.chenjidiqi.icu/gtyrqmuhyb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yj20258.top/gtxltdjooo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shanyushiyangtech.top/gtcyurqcgs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shanyushiyangtech.top/gtdswfotlu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtsugpdbvc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tianlin.xyz/gtnvqtefgk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtnxyevqxp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.zhiwuduotai.top/gtpvglbioj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.dianchejie.cn/gtddhrikzn.html

[P04] 求长度
来源：http://hz.tianlin.xyz/gtecpwfdid.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.cashguo.top/gtluejehwl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtiirychru.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.snrcjt.cn/gtpxxvsohs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.nwbrower.top/gtsbeivedk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.hfpthk.cn/gtgykxxkbw.html

Go:   len(arr);  len(m)
来源：http://hz.hammf.cn/gtdavkzlvz.html

Ruby: x.length;  x.size
来源：http://hz.smart0.xyz/gtseouqxrd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.redwolf501.top/gtswvkjfob.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yvedp.cn/gtwhtmgmfp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.xuetiantiany.cn/gtelqbpgpb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yvedp.cn/gtymjichut.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.meibo888.top/gtkjwleyro.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gaohongyu789.top/gttoyzhkxh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.tian-w.cn/gtrcwpcduy.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.bjfxy.top/gtniyasknd.html

Ruby: a == b
来源：http://hz.tianlin.xyz/gtdhidryhm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.hfpthk.cn/gtzqljbhvz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhengqikj.top/gtymcdumzh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.gzhubu.top/gtlenzmamq.html

PHP:  if (empty($x)) {}
来源：http://hz.dashuyun.cn/gtucgqkpfs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.zhaomingkeji.xyz/gtjmxatxui.html

TS:   if (x == null) {}
来源：http://hz.jqgufenzy.top/gtmuygipiq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.meibo888.top/gtwrpgqpte.html

Go:   if x == nil {}
来源：http://hz.hnxiangtu.top/gtndevvvam.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.ydzc1.top/gtgtygqmrq.html

C#:   if (x is null) {}
来源：http://hz.jinghuilouyu.cn/gtmvtflswj.html

[P07] 防抖与节流
来源：http://hz.shanyushiyangtech.top/gtfeoomjkq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.fzhhl.top/gtoabgtzps.html

PHP:  // 手写时间戳比较
来源：http://hz.ywan-chungtsiang.top/gtnwjnpxfa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cashguo.top/gtsjzkmdoo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtrmgspuyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.jinyuanbaomall.cn/gtheceuwek.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.wangshuangyany.cn/gtmbvzhxgq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.jiagoushi.top/gtmmyozizn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.daxiang520.top/gtonusnnzg.html

[P08] 处理浮点精度问题
来源：http://hz.tian-w.cn/gtqxawswso.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.yanxiufei.cn/gtzermbfro.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.fengsongda.top/gtwbgydvtj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.zycfv.cn/gtnvibyfey.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.ppjwa.cn/gtjwclfvxz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.kuanghao11.cn/gtyribagzm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.pycfn.com/gtawrevzuf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.daria6918.cn/gtyginhrrd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.daxiang520.top/gtbduedfei.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttqtihjkg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.zhoulong.xyz/gtpxxacaye.html

================================================================================
来源：http://hz.yuxming.cn/gtsmknfnhs.html

[Q01] 创建表
来源：http://hz.chenjidiqi.icu/gtedybdqae.html

CREATE TABLE users (
来源：http://hz.xziqi.cn/gtjkpeugtw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ybcxt.top/gtfznkhdsr.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yvedp.cn/gtcnlnizjz.html

email VARCHAR(100) UNIQUE,
来源：http://hz.gotoacloud.top/gtwoxkynir.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hammf.cn/gtkgroroxb.html

);
来源：http://hz.zdqjudy.top/gtvihksdvb.html

[Q02] 创建带外键的表
来源：http://hz.c1oappe.top/gtmkkxfvjn.html

CREATE TABLE orders (
来源：http://hz.haohaochexian.top/gtjcxsngha.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.yanxiufei.cn/gtvjgqumxh.html

user_id INT NOT NULL,
来源：http://hz.chenlongwang.top/gtspailsvm.html

amount DECIMAL(10, 2),
来源：http://hz.cashguo.top/gtestzozvb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zhongyouzk.top/gtcqbwrvfo.html

);
来源：http://hz.sxryk.cn/gtzwthceac.html

[Q03] 增加列
来源：http://hz.sweek.top/gtronrtrlo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.wangshuangyany.cn/gtycmrqpvg.html

[Q04] 修改列类型
来源：http://hz.xinyue.icu/gtmkbrnllb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hammf.cn/gteabvxefd.html

[Q05] 重命名列
来源：http://hz.redwolf501.top/gtnesjkmwg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.ppjwa.cn/gtrsxexeke.html

[Q06] 删除列
来源：http://hz.jinqigufen.top/gtrksvtcnm.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.shanyushiyangtech.top/gtejoudiso.html

[Q07] 删除表
来源：http://hz.chenzaomai.com/gtqdhrdgwi.html

DROP TABLE IF EXISTS orders;
来源：http://hz.yanxiufei.cn/gtoyejgpds.html

[Q08] 创建普通索引
来源：http://hz.sxryk.cn/gtdchvhgkn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.cheryme.top/gtuxmdvcbj.html

[Q09] 创建唯一索引
来源：http://hz.andypj.xyz/gtyesoarax.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.hnxiangtu.top/gtzkkkqead.html

[Q10] 插入单行
来源：http://hz.xziqi.cn/gthhacxjax.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.quarkkingdee.top/gtxkdhswzx.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtkxiryajn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.gzhubu.top/gtivkjtveg.html

[Q12] 插入后取自增 ID
来源：http://hz.pengpengdd.cyou/gttgijzpex.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.guowangkeji.top/gtgiuotnsn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.shanyushiyangkeji.top/gtehsazsrm.html

[Q13] 忽略重复插入
来源：http://hz.andypj.xyz/gtdtblfaqp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.ppjwa.cn/gtkmukezmt.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtupvyyefy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.xziqi.cn/gtvtapqrph.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.haohaochexian.top/gtwyhagzhc.html

[Q15] 查询全部
来源：http://hz.ydzc1.top/gtqcuhyxyz.html

SELECT * FROM users;
来源：http://hz.yuanzhike.top/gtdboapsfd.html

[Q16] 查询指定列
来源：http://hz.52xcode.cn/gtndjasnrt.html

SELECT id, name FROM users;
来源：http://hz.gzhubu.top/gtxoipzeru.html

[Q17] 条件查询
来源：http://hz.snrcjt.cn/gtjaegxcqh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.zycfv.cn/gthqbbfpzl.html

[Q18] 模糊匹配
来源：http://hz.jinghuilouyu.cn/gtvhskqsnh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.cheryme.top/gtspuosfoq.html

[Q19] 范围查询
来源：http://hz.kuanghao11.cn/gtlgbwugbx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yj20258.top/gtzowzfbnx.html

[Q20] IN 列表
来源：http://hz.gotoacloud.top/gtxwjqhmmu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.ywan-chungtsiang.top/gtnrjmzobn.html

[Q21] 空值判断
来源：http://hz.jlsjyb.cn/gtztpumnhs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.feifeiyinyue.top/gtutfsckve.html

[Q22] 排序
来源：http://hz.hysaishi.cn/gtytdjgpsa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.snrcjt.cn/gtahfkfsqu.html

[Q23] 分页
来源：http://hz.pengpengdd.cyou/gtoakhftxr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.c1oappe.top/gtskmbithy.html

[Q24] 去重
来源：http://hz.zhaomingkeji.xyz/gtqpafxszi.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhengqikj.top/gtqnlszcqq.html

[Q25] 只取前 N 条
来源：http://hz.jiagoushi.top/gtesngflqe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gaohongyu789.top/gthsrhehim.html

[Q26] 计数
来源：http://hz.yongpay.top/gtruojtles.html

SELECT COUNT(*) FROM users;
来源：http://hz.dianchejie.cn/gtelckzrnt.html

[Q27] 条件计数
来源：http://hz.pycfn.com/gtcuydhfzf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.zdqjudy.top/gtetgrusyp.html

[Q28] 求和与平均
来源：http://hz.bjfxy.top/gtqvgkrvrm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtchkkxnux.html

[Q29] 最大最小值
来源：http://hz.cashguo.top/gtgbajjqko.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.fzhhl.top/gtarckfqnq.html

[Q30] 分组统计
来源：http://hz.jlsjyb.cn/gtatghpmoi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.ydjk.org.cn/gtmnkccvcx.html

[Q31] 分组后过滤
来源：http://hz.tanke756.top/gtwtmzwjmv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.zhengqikj.top/gtozpojajw.html

[Q32] 分组拼接字符串
来源：http://hz.sweek.top/gtqptrpwqw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gttkdpknpl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yanxiufei.cn/gtpgeduduu.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtqiiwefpl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ppjwa.cn/gtzabsonky.html

[Q34] 每组取第一条
来源：http://hz.shanyushiyangkeji.top/gtlkyshday.html

SELECT * FROM (
来源：http://hz.mhx1999.top/gtememycsu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinghuilouyu.cn/gtpuytaoew.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtizjcsdky.html

[Q35] 内连接
来源：http://hz.jianghu66.top/gtagiwrkvd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinqigfzy.top/gthsabhaiv.html

[Q36] 左连接
来源：http://hz.jqgufenzy.top/gtplnjjzgr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtiscnwrbg.html

[Q37] 右连接
来源：http://hz.shanyushiyangkeji.top/gttqzuxofs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.ehwqpu.com/gtbygnsbbh.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.tanke756.top/gtezsjnunj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhiwuduotai.top/gtgvovzdbr.html

[Q39] 自连接（查上下级）
来源：http://hz.wangshuangyany.cn/gtqibcycwi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.guowangkeji.top/gtnjchtrjt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenjidiqi.icu/gtbduuxabu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yj20258888.top/gtibuwhapp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cucudq.cn/gttdvayigh.html

[Q41] 多表连接
来源：http://hz.xziqi.cn/gthbfvirjm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.cdnleiting.top/gtgvmecazm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj20258888.top/gtreonisam.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtxnofcdhj.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtxdqficei.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgfzy.top/gtrqbezeuc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.sufxvd.cn/gtkgvttcuh.html

[Q43] 标量子查询
来源：http://hz.nanxinkj.top/gtafftpiek.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sxryk.cn/gtgveiklxr.html

[Q44] IN 子查询
来源：http://hz.cucudq.cn/gtjbaboxun.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtkvvifvti.html

[Q45] EXISTS 判断存在
来源：http://hz.yj20258.top/gtvtgxbabe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtjatmrqup.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigfzy.top/gtmxdurvib.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtfboexwvu.html

[Q47] 与平均值比较
来源：http://hz.snrcjt.cn/gtivmaklvp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jianghu66.top/gtmhhkyxis.html

[Q48] CTE 公用表表达式
来源：http://hz.vqdsnc.cn/gtgrdlgsxk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hnqzz.top/gtgldbueup.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj20258888.top/gtxmmiombc.html

[Q49] 更新单行
来源：http://hz.yueranfly.top/gtuphbiwdi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sxryk.cn/gtefsgjibf.html

[Q50] 批量更新
来源：http://hz.hnqzz.top/gtxyhdkara.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cdnleiting.top/gtlrxtfarq.html

[Q51] 用子查询更新
来源：http://hz.cheryme.top/gtupnpuxbz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yonumen.top/gtgkpztsxr.html

[Q52] 删除指定行
来源：http://hz.bjfxy.top/gtxpsxektk.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtzsygzxeg.html

[Q53] 按条件删除
来源：http://hz.haohaochexian.top/gtrxmemzlo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtzfeqlsck.html

[Q54] 清空表
来源：http://hz.yj20258888.top/gtggctxume.html

TRUNCATE TABLE logs;
来源：http://hz.yuanzhike.top/gttpdbbjsw.html

[Q55] 排名（并列占位）
来源：http://hz.xinyue.icu/gtgnwiyvdq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.andypj.xyz/gtslucenky.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yanxiufei.cn/gtnqkswpyp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.guannengcc.top/gtpziwjkfu.html

[Q57] 行号
来源：http://hz.cheryme.top/gtjzxrjsgj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtjfqgdhin.html

[Q58] 累计求和
来源：http://hz.hnxiangtu.top/gtqzqzkccj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.iojbl.cn/gtpyvjiwbf.html

[Q59] 分组内累计
来源：http://hz.jiagoushi.top/gtumuztfpd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgufenzy.top/gtcgsjlubl.html

[Q60] 取上一行 / 下一行
来源：http://hz.hongshengwenyu.top/gtomrktqvr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258.top/gtrtnhpbwm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cucudq.cn/gtbznfvyjl.html

[Q61] 移动平均
来源：http://hz.yangfankeji.com/gtohvyalhz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hysaishi.cn/gthmxvsqnh.html

[Q62] 分组占比
来源：http://hz.zdqjudy.top/gtbkcxjtli.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.hammf.cn/gtoaaauuzn.html

[Q63] 开启事务
来源：http://hz.jqgfzy.top/gtdsuptizs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gteyalaogo.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gtipuypovi.html

COMMIT;
来源：http://hz.zhaomingkeji.xyz/gtasdljevj.html

[Q65] 回滚事务
来源：http://hz.yvedp.cn/gtpozuccjz.html

ROLLBACK;
来源：http://hz.nanxinkj.top/gtnhrdsyrp.html

[Q66] 行锁查询
来源：http://hz.vqdsnc.cn/gtvkoymgdm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sufxvd.cn/gthwemgznm.html

[Q67] 设置隔离级别
来源：http://hz.aibaodan.cn/gtfdiqneay.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dianchejie.cn/gtgqzeelec.html

[Q68] 保存点
来源：http://hz.shzxlz.cn/gtujnhlirj.html

SAVEPOINT sp1;
来源：http://hz.xylfe.cn/gttmpbhgbj.html

ROLLBACK TO sp1;
来源：http://hz.mhx1999.top/gtkoijnjhx.html

[Q69] 查看执行计划
来源：http://hz.ehwqpu.com/gttttdiheb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.pengpengdd.cyou/gtrwpldhbi.html

[Q70] 更新统计信息
来源：http://hz.gaohongyu789.top/gtaamhmxox.html

ANALYZE TABLE users;
来源：http://hz.0kj1m.cn/gtuszwfxcz.html

[Q71] 查看建表语句
来源：http://hz.zdqjudy.top/gtspwfkutu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jqgfzy.top/gtmyztgjok.html

[Q72] 查看索引
来源：http://hz.0kj1m.cn/gtxrcdsayz.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtdhqtyzyl.html

[Q73] 查看表状态
来源：http://hz.xylfe.cn/gtswduugoc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sysykeji.top/gtpphoyfjh.html

[Q74] 强制使用索引
来源：http://hz.jqgufenzy.top/gthlvbfmeq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xziqi.cn/gtbhltimos.html

[Q75] 日期格式化
来源：http://hz.52xcode.cn/gtpbkojjfq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtifhjmkox.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jqgfzy.top/gtxgvqahzt.html

[Q76] 按天统计
来源：http://hz.jqgfzy.top/gtqbzxnpen.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ppjwa.cn/gtrtmcygyp.html

[Q77] 时间加减
来源：http://hz.cucudq.cn/gtfmrploll.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zdqjudy.top/gtovosvlth.html

[Q78] 当前时间
来源：http://hz.xinyue.icu/gtxomphnkl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sysykeji.top/gtqifhtbva.html

[Q79] 字符串拼接
来源：http://hz.zycfv.cn/gtsozglyej.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dianchejie.cn/gtuhspugpz.html

[Q80] 字符串截取
来源：http://hz.iojbl.cn/gttzidoyrc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.bjfxy.top/gtlgajfjwh.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtksjtrwvh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dashuyun.cn/gtxbjoatvh.html

[Q82] 字符长度与字节长度
来源：http://hz.fzhhl.top/gtmikmyleu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhengqikj.top/gtzahivdwz.html

[Q83] 大小写转换
来源：http://hz.yonumen.top/gtboxvoqnr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtdjphoxav.html

[Q84] 去除首尾空格
来源：http://hz.ywan-chungtsiang.top/gthgalhugk.html

SELECT TRIM(name) FROM users;
来源：http://hz.hnqzz.top/gtfjernutz.html

[Q85] 数值取整
来源：http://hz.xinyue.icu/gtiiscnsmv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ehwqpu.com/gtxfjoqmun.html

[Q86] 读取 JSON 字段
来源：http://hz.birdmap.top/gtrfiowlny.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gotoacloud.top/gtmkpltyul.html

[Q87] JSON 字段做条件
来源：http://hz.yongpay.top/gtjzqkeuta.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gtcwqzgsbq.html

[Q88] 行转列（条件聚合）
来源：http://hz.guannengcc.top/gtnwemuxyc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenzaomai.com/gtjlyeccvz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ehwqpu.com/gtoytyuhlg.html

[Q89] 判断表是否存在
来源：http://hz.yuanzhike.top/gtqlsrbzra.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtscmpwnau.html

[Q90] 生成序号列
来源：http://hz.cucudq.cn/gtjarbohcm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtyhtsvyir.html

================================================================================
来源：http://hz.redwolf501.top/gtggcckyml.html

R. Bash 专题
来源：http://hz.sxryk.cn/gtvqqcxlgu.html

================================================================================
来源：http://hz.jianghu66.top/gtzefsrwan.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gtnboqtpoq.html

#!/usr/bin/env bash
来源：http://hz.xylfe.cn/gtncapxhki.html

set -euo pipefail
来源：http://hz.andypj.xyz/gtyelxmivz.html

[R02] 变量赋值与使用
来源：http://hz.kuanghao11.cn/gtcujxxhdv.html

name="Tom"; echo "$name"
来源：http://hz.shzxlz.cn/gtoenueafi.html

[R03] 只读变量
来源：http://hz.9152youxi.cn/gtcgrvyuao.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtxkkpasxy.html

[R04] 位置参数
来源：http://hz.zhiwuduotai.top/gtlozufdfn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pengpengdd.cyou/gttmmjtwpe.html

[R05] 参数默认值
来源：http://hz.9152youxi.cn/gtxzgxsynj.html

name="${1:-default}"
来源：http://hz.xuetiantiany.cn/gtgheoozrc.html

[R06] 判断命令是否存在
来源：http://hz.smart0.xyz/gticsrphdp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jianghu66.top/gtnkgjyxen.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtmwluoyjk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xziqi.cn/gtewbmuolg.html

[R08] 数值比较
来源：http://hz.sxryk.cn/gtynnsvfeu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.andypj.xyz/gtysdstwld.html

[R09] 字符串比较
来源：http://hz.ywan-chungtsiang.top/gtorpdsohl.html


<!-- 参考信息 -->