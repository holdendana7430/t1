代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.kuanghao11.cn/gtplwbmqkl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.jinyuanbaomall.cn/gtvhqsbxoi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.nanxinkj.top/gttlwguvdt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.hnqzz.top/gtzzznujoj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.nanxuanxn.top/gtasvfgbiw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yangfankeji.com/gtbeukjdyq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hysaishi.cn/gtwvfoawwb.html

[P04] 求长度
来源：http://hz.jqgufenzy.top/gtxkqqskyp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.feifeiyinyue.top/gtnxhwpaju.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtgzrlyzpn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yj202588.top/gtbdwhpred.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.yongpay.top/gtjydevcds.html

Java: list.size();  map.size();  s.length()
来源：http://hz.birdmap.top/gtticiedzc.html

Go:   len(arr);  len(m)
来源：http://hz.wangdashe.top/gtutnkdsyg.html

Ruby: x.length;  x.size
来源：http://hz.yonumen.top/gtomeaaiqw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.smart0.xyz/gthhxxzzud.html

[P05] 判断两个对象内容是否相等
来源：http://hz.xinyue.icu/gtrpgkfjxc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.mhx1999.top/gtejfnwklr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.yj202588.top/gtmmskoksf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.zhengqikj.top/gtbiqadjjg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhaomingkeji.xyz/gtwgynhfkl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.wangdashe.top/gtvwxvpoxc.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.redwolf501.top/gthzugqgpf.html

Ruby: a == b
来源：http://hz.sxryk.cn/gtbimnrgrv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.52xcode.cn/gtnrewlfhe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.zhixingplan.top/gtiutjgduy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.guowangkeji.top/gtnegfscxu.html

PHP:  if (empty($x)) {}
来源：http://hz.tianlin.xyz/gttkzkiyrq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.gaohongyu789.top/gtcfwjamsm.html

TS:   if (x == null) {}
来源：http://hz.shangyingyoupin.top/gtfdwpnlfj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.mhx1999.top/gtfbghjqhi.html

Go:   if x == nil {}
来源：http://hz.yj202588.top/gtzgawcyip.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.yanxiufei.cn/gtwnyhdgsh.html

C#:   if (x is null) {}
来源：http://hz.snrcjt.cn/gtdtbdibof.html

[P07] 防抖与节流
来源：http://hz.cheryme.top/gtweolcjov.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.guowangkeji.top/gtstizsyod.html

PHP:  // 手写时间戳比较
来源：http://hz.ybcxt.top/gtjqlbqmon.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hywenlv.cn/gtmajortlx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ydjk.org.cn/gtrzsdwavl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.hywenlv.cn/gtfismguor.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.fzhhl.top/gtcgbkadil.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.gotoacloud.top/gtrohunsjc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.zhixingplan.top/gtctdlqocz.html

[P08] 处理浮点精度问题
来源：http://hz.hongshengwenyu.top/gtsunzzbve.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.pengpengdd.cyou/gtsljuffgf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.gogol.net.cn/gtgccrbmpk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.9152youxi.cn/gtsoxvkjdx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.svipenyu.cn/gtpvgbztsi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.cqqwz.cn/gtubyucqhj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.hysaishi.cn/gtrydddzmf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.nanxinkj.top/gtzkpikevp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.c1oappe.top/gtycukfhsw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtatdupsoo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.wangdashe.top/gtdiviikcq.html

================================================================================
来源：http://hz.daria6918.cn/gtzbcsbttm.html

[Q01] 创建表
来源：http://hz.svipenyu.cn/gtubemlkyw.html

CREATE TABLE users (
来源：http://hz.yueranfly.top/gtftqmdlno.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.ydjk.org.cn/gtruhsysxv.html

name VARCHAR(50) NOT NULL,
来源：http://hz.fengsongda.top/gtrlwoqlza.html

email VARCHAR(100) UNIQUE,
来源：http://hz.jinyuanbaomall.cn/gtzatczzor.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.sufxvd.cn/gtomqquqzi.html

);
来源：http://hz.nanxinkj.top/gtwqslsdyl.html

[Q02] 创建带外键的表
来源：http://hz.iojbl.cn/gtfdkxakig.html

CREATE TABLE orders (
来源：http://hz.sysykeji.top/gtvcakqamt.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.cdnleiting.top/gthgpankez.html

user_id INT NOT NULL,
来源：http://hz.iojbl.cn/gtnweocjnz.html

amount DECIMAL(10, 2),
来源：http://hz.zycfv.cn/gtipmnzuqr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.zycfv.cn/gtwzluvaxm.html

);
来源：http://hz.zhoulong.xyz/gtiwbfptad.html

[Q03] 增加列
来源：http://hz.sweek.top/gtzadwbkeu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.chenzaomai.com/gtxxgszlnu.html

[Q04] 修改列类型
来源：http://hz.gzhubu.top/gtlgejwloc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.hywenlv.cn/gtwybajkwl.html

[Q05] 重命名列
来源：http://hz.hammf.cn/gtnrganqtb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.sweek.top/gtfyzbndmv.html

[Q06] 删除列
来源：http://hz.yj20258888.top/gtsdjrfyat.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.hywenlv.cn/gtdkosmfld.html

[Q07] 删除表
来源：http://hz.0kj1m.cn/gtxhueygff.html

DROP TABLE IF EXISTS orders;
来源：http://hz.quarkkingdee.top/gtynqgofdz.html

[Q08] 创建普通索引
来源：http://hz.zhongyouzk.top/gtjzjklhxv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.quarkkingdee.top/gtgkqhzhyt.html

[Q09] 创建唯一索引
来源：http://hz.ivvv.top/gteluruncl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.sxryk.cn/gtiycxujkg.html

[Q10] 插入单行
来源：http://hz.andypj.xyz/gtdhvhfhri.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.xziqi.cn/gtykqwcdkw.html

[Q11] 一次插入多行
来源：http://hz.havefunace.top/gtepysrzzr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.jqgfzy.top/gtqklavtpv.html

[Q12] 插入后取自增 ID
来源：http://hz.yj20258.top/gtapakwquz.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zdqjudy.top/gtvatpnndu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dianchejie.cn/gtxhfwboqo.html

[Q13] 忽略重复插入
来源：http://hz.jiagoushi.top/gtrfntckgo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.dashuyun.cn/gtsohqwzsw.html

[Q14] 存在则更新（upsert）
来源：http://hz.feifeiyinyue.top/gtggziuefb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.wangdashe.top/gtkmfhktxt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.bjfxy.top/gtnmpkzkhw.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtkxjrymlq.html

SELECT * FROM users;
来源：http://hz.haohaochexian.top/gtjbfdrvhd.html

[Q16] 查询指定列
来源：http://hz.tian-w.cn/gtjsodkdjm.html

SELECT id, name FROM users;
来源：http://hz.daxiang520.top/gthjnhibcq.html

[Q17] 条件查询
来源：http://hz.jqgufenzy.top/gtdpgiktia.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.ivvv.top/gtpywvjdzi.html

[Q18] 模糊匹配
来源：http://hz.xziqi.cn/gtofzdjkrz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ybcxt.top/gtmcgcewye.html

[Q19] 范围查询
来源：http://hz.nwbrower.top/gtxgbcugdg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jinqigufen.top/gtdqsxcmbl.html

[Q20] IN 列表
来源：http://hz.dianchejie.cn/gthwcktphh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.cucudq.cn/gtnklojgpx.html

[Q21] 空值判断
来源：http://hz.daxiang520.top/gtrqqicwqh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.bjfxy.top/gthmxvtrbp.html

[Q22] 排序
来源：http://hz.daxiang520.top/gtxzopfxli.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.feifeiyinyue.top/gtfcliyxaw.html

[Q23] 分页
来源：http://hz.gogol.net.cn/gtrnjasagy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yongpay.top/gtflpddqxk.html

[Q24] 去重
来源：http://hz.sufxvd.cn/gtjjsvrzwv.html

SELECT DISTINCT city FROM users;
来源：http://hz.ppjwa.cn/gtynmkomdm.html

[Q25] 只取前 N 条
来源：http://hz.gzhubu.top/gtbsvykqwn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.zhijiandao.cn/gtniwgjapt.html

[Q26] 计数
来源：http://hz.guowangkeji.top/gtcxqnhswz.html

SELECT COUNT(*) FROM users;
来源：http://hz.daria6918.cn/gtcifxwbbb.html

[Q27] 条件计数
来源：http://hz.nwbrower.top/gtfzjfnvhv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.redwolf501.top/gtfkrhdcag.html

[Q28] 求和与平均
来源：http://hz.zhengqikj.top/gtlqhcnzwc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zhongyouzk.top/gtsskwnjuc.html

[Q29] 最大最小值
来源：http://hz.316326.xyz/gttfgpgwhb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.cdnleiting.top/gtsevgiwal.html

[Q30] 分组统计
来源：http://hz.sxryk.cn/gtegzhbbdw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtaenjpxwa.html

[Q31] 分组后过滤
来源：http://hz.yongpay.top/gtdkshwyat.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xylfe.cn/gtmpzzeagx.html

[Q32] 分组拼接字符串
来源：http://hz.aizwys.cn/gtwznkwahu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtyajouwna.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtkswngrww.html

[Q33] 多列分组
来源：http://hz.shzxlz.cn/gtbzutmfpr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jyoumei.cn/gtgixdxeiy.html

[Q34] 每组取第一条
来源：http://hz.bjfxy.top/gtrthcaogs.html

SELECT * FROM (
来源：http://hz.cucudq.cn/gtyffrukij.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shangyingyoupin.top/gteoemjzex.html

) t WHERE rn = 1;
来源：http://hz.yonumen.top/gtmvwgiwqn.html

[Q35] 内连接
来源：http://hz.xingfuxueyuan.xyz/gtgbgtedaq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtpmzogoix.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gthtupbfiz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.xingfuxueyuan.xyz/gtvnkyqgom.html

[Q37] 右连接
来源：http://hz.xingfuxueyuan.xyz/gtyjnqnelm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hfpthk.cn/gtnbmaaqiz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gogol.net.cn/gtsjccykfw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.zhijiandao.cn/gtjhzghgkd.html

[Q39] 自连接（查上下级）
来源：http://hz.zhiwuduotai.top/gtsfeyqdkx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtdbkblzmi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.tanke756.top/gtsdndtxkn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hysaishi.cn/gtexumjwmd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.gotoacloud.top/gtlmcfrpjk.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtuuabdflu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.bjfxy.top/gtgdriqxcn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jianghu66.top/gtihtdbxsy.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.ydjk.org.cn/gtwgnpwpai.html

[Q42] 连接条件附加过滤
来源：http://hz.9152youxi.cn/gtbymdwfgj.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yonumen.top/gtfonerkyl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.52xcode.cn/gtisvaqohj.html

[Q43] 标量子查询
来源：http://hz.jianghu66.top/gtwlmrndcg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hywenlv.cn/gtauqowfvw.html

[Q44] IN 子查询
来源：http://hz.cqqwz.cn/gttbpimeva.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ybcxt.top/gthyssxzex.html

[Q45] EXISTS 判断存在
来源：http://hz.tianlin.xyz/gtogspfsnl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cdnleiting.top/gticroxtwy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yuxming.cn/gtfjqinqzz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.dashuyun.cn/gtptalcsdd.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtzvxwflta.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aibaodan.cn/gtdzlqiwyi.html

[Q48] CTE 公用表表达式
来源：http://hz.hnqzz.top/gtoreiqdhg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jianghu66.top/gtlsqgczsk.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hysaishi.cn/gtcudjhhzx.html

[Q49] 更新单行
来源：http://hz.jianghu66.top/gtuuvpmpaj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.52xcode.cn/gtddlmpknx.html

[Q50] 批量更新
来源：http://hz.yongpay.top/gtbecimdmn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jyoumei.cn/gtmoweredo.html

[Q51] 用子查询更新
来源：http://hz.nanxinkj.top/gthjrfzgyg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sweek.top/gtunxqfmog.html

[Q52] 删除指定行
来源：http://hz.yvedp.cn/gtwwfkaoyt.html

DELETE FROM users WHERE id = 10;
来源：http://hz.pycfn.com/gtjlamegme.html

[Q53] 按条件删除
来源：http://hz.pycfn.com/gtxhcvtxej.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhaomingkeji.xyz/gtoeooscei.html

[Q54] 清空表
来源：http://hz.havefunace.top/gtwrjqtfpm.html

TRUNCATE TABLE logs;
来源：http://hz.jianghu66.top/gtlakydnma.html

[Q55] 排名（并列占位）
来源：http://hz.iojbl.cn/gtpctqicfu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.havefunace.top/gtsdyaxyab.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tianlin.xyz/gtyihzlnli.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gogol.net.cn/gtbzdlefpa.html

[Q57] 行号
来源：http://hz.nanxinkj.top/gtekwdhhbv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.redwolf501.top/gtfnmpkrlh.html

[Q58] 累计求和
来源：http://hz.vqdsnc.cn/gtivzfigzg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtdoluzzin.html

[Q59] 分组内累计
来源：http://hz.zdqjudy.top/gtlufzizqd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cucudq.cn/gtojqcmegz.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtcnovncyk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hfpthk.cn/gtgccyjjla.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shzxlz.cn/gtvpkcuuko.html

[Q61] 移动平均
来源：http://hz.andypj.xyz/gtagsjplox.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gtiyagckud.html

[Q62] 分组占比
来源：http://hz.shangyingyoupin.top/gtxwfyoqwb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtrgiommph.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtxnzmpnln.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cheryme.top/gtpefrruap.html

[Q64] 提交事务
来源：http://hz.c1oappe.top/gtcskqavkm.html

COMMIT;
来源：http://hz.gzhubu.top/gtygfiwbyw.html

[Q65] 回滚事务
来源：http://hz.cdnleiting.top/gtewhjiudv.html

ROLLBACK;
来源：http://hz.shanyushiyangtech.top/gtaxqqgkvw.html

[Q66] 行锁查询
来源：http://hz.yongpay.top/gtkimghfgt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hongshengwenyu.top/gtukrvdmql.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gtxmihbeok.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yongpay.top/gtxnrhjgmr.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtjcbfubpy.html

SAVEPOINT sp1;
来源：http://hz.hnqzz.top/gtshymgmgx.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtthzccktg.html

[Q69] 查看执行计划
来源：http://hz.shanyushiyangtech.top/gtxpcahhna.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cheryme.top/gtjmbgbtkn.html

[Q70] 更新统计信息
来源：http://hz.yongpay.top/gttlvejdgd.html

ANALYZE TABLE users;
来源：http://hz.jyoumei.cn/gtwjgtlxxf.html

[Q71] 查看建表语句
来源：http://hz.zycfv.cn/gtvxiwajmb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zdqjudy.top/gtuqymvmxe.html

[Q72] 查看索引
来源：http://hz.zhoulong.xyz/gtcrbpsgys.html

SHOW INDEX FROM users;
来源：http://hz.yvedp.cn/gtblrzewdz.html

[Q73] 查看表状态
来源：http://hz.cqqwz.cn/gttefdgszs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xuanzx.com/gtcdeueyip.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtstlazrkj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.chenjidiqi.icu/gtabmwexiy.html

[Q75] 日期格式化
来源：http://hz.chenzaomai.com/gthrjvvopu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.aibaodan.cn/gtvghxnnwc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangtech.top/gtdntzgsjx.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtprjyfbsx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nwbrower.top/gtlfsmnjqj.html

[Q77] 时间加减
来源：http://hz.hfpthk.cn/gtansicapu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.c1oappe.top/gtnekpnnrb.html

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtxqcyhnzi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shangyingyoupin.top/gtmzluvxyv.html

[Q79] 字符串拼接
来源：http://hz.xziqi.cn/gtuwhcccjm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cdnleiting.top/gtqwbxrsmp.html

[Q80] 字符串截取
来源：http://hz.sweek.top/gtdyghqher.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtqgwsmtxm.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtcjbfrubs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yj202588.top/gtmffndiku.html

[Q82] 字符长度与字节长度
来源：http://hz.yangfankeji.com/gtmwibjgin.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtejxqkjbp.html

[Q83] 大小写转换
来源：http://hz.hammf.cn/gtxjyyekqf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgufenzy.top/gtluwszgmb.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtzueywwdq.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtkkcvyhke.html

[Q85] 数值取整
来源：http://hz.fzhhl.top/gtjkduexjl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.mhx1999.top/gtgpsebkho.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gttczwykzt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zdqjudy.top/gtzbjyovqv.html

[Q87] JSON 字段做条件
来源：http://hz.iojbl.cn/gthscqbrxx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtgudpkaqx.html

[Q88] 行转列（条件聚合）
来源：http://hz.mhx1999.top/gtfoyrxtwf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cheryme.top/gtjtvqquwf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.svipenyu.cn/gtwcyodszh.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gtkuanftuv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pengpengdd.cyou/gtgpmzolhz.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtydljgllg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hywenlv.cn/gttzizyebw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtniysxtia.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gtrwbchghq.html

================================================================================
来源：http://hz.sufxvd.cn/gthgjdivoc.html

[R01] shebang 与严格模式
来源：http://hz.yj20258.top/gtujluygga.html

#!/usr/bin/env bash
来源：http://hz.gotoacloud.top/gtbzqltxxt.html

set -euo pipefail
来源：http://hz.52xcode.cn/gtkaiuhyvq.html

[R02] 变量赋值与使用
来源：http://hz.guannengcc.top/gtuodgjzjv.html

name="Tom"; echo "$name"
来源：http://hz.0kj1m.cn/gtzdckagmr.html

[R03] 只读变量
来源：http://hz.yangfankeji.com/gtepqylbrh.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gtpzxlmcdu.html

[R04] 位置参数
来源：http://hz.zhixingplan.top/gtazcsmawn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtywllhbmo.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtlgofmdss.html

name="${1:-default}"
来源：http://hz.dianchejie.cn/gtwzsddosk.html

[R06] 判断命令是否存在
来源：http://hz.aibaodan.cn/gtlgcorngn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hfpthk.cn/gtjcmqmeuw.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gtkscqtacb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daxiang520.top/gtwerevtdu.html

[R08] 数值比较
来源：http://hz.ivvv.top/gtrgxwoyei.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.redwolf501.top/gtdhormvoh.html

[R09] 字符串比较
来源：http://hz.sweek.top/gtcapjbzlg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinghuilouyu.cn/gtlrehinha.html

[R10] 正则匹配
来源：http://hz.xylfe.cn/gtxdztyiml.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gzhubu.top/gtbizjsumo.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtzgbbiixr.html

case "$1" in
来源：http://hz.birdmap.top/gtjuerabil.html

start) echo "启动" ;;
来源：http://hz.tanke756.top/gthnievgji.html

stop)  echo "停止" ;;
来源：http://hz.wangdashe.top/gtdarkbejx.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gttllobqkl.html

esac
来源：http://hz.jinghuilouyu.cn/gtbsuztmnk.html

[R12] for 遍历文件
来源：http://hz.wangshuangyany.cn/gtuqayfega.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinghuilouyu.cn/gthvakmqka.html

[R13] for 计数循环
来源：http://hz.0kj1m.cn/gtvkototcu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258888.top/gtisgabkmc.html

[R14] C 风格 for
来源：http://hz.ydzc1.top/gtqvpvwuqf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtzbdhldxc.html

[R15] while 逐行读文件
来源：http://hz.aizwys.cn/gtjqlqkeli.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigufen.top/gtteacaxdf.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtzomdonxs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhixingplan.top/gtyphrdlmu.html

[R17] 数组定义与取值
来源：http://hz.jqgufenzy.top/gtzzxmlfpo.html


<!-- 参考信息 -->