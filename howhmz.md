代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cashguo.top/gtzulhewvq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hongshengwenyu.top/gtgeilemzs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.vqdsnc.cn/gtjdmraznd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.tian-w.cn/gtmcbzxcah.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.316326.xyz/gttmucunqb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.nanxuanxn.top/gtqdjflydo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.gaohongyu789.top/gtamzsmjru.html

[P04] 求长度
来源：http://hz.yangfankeji.com/gtcqzkdlre.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.hammf.cn/gtcpxjcisf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sufxvd.cn/gtlergcpza.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ppjwa.cn/gthujbwfnw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.meibo888.top/gtaykjedfs.html

Java: list.size();  map.size();  s.length()
来源：http://hz.sxryk.cn/gtdawefpak.html

Go:   len(arr);  len(m)
来源：http://hz.dianchejie.cn/gtbjmvvpat.html

Ruby: x.length;  x.size
来源：http://hz.yanxiufei.cn/gtmopbntvi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.quarkkingdee.top/gtwkoedldc.html

[P05] 判断两个对象内容是否相等
来源：http://hz.yueranfly.top/gtskbqjiyp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://hz.birdmap.top/gtjhtsvkbp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hz.zdqjudy.top/gthaylfszf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hz.redwolf501.top/gtmhsneiyg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.shanyushiyangtech.top/gtbslirhvc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hz.smart0.xyz/gtpnvppodj.html

Go:   reflect.DeepEqual(a, b)
来源：http://hz.guannengcc.top/gtshhppvrj.html

Ruby: a == b
来源：http://hz.316326.xyz/gtnmajgdbx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hz.zhoulong.xyz/gtjumkqsmp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hz.havefunace.top/gtheovwspg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hz.jinqigfzy.top/gtuizzgfmo.html

PHP:  if (empty($x)) {}
来源：http://hz.xinyue.icu/gtgghiifsn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hz.yvedp.cn/gtfzgatnmf.html

TS:   if (x == null) {}
来源：http://hz.zycfv.cn/gtuhgvuvhn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://hz.guannengcc.top/gteklxaibe.html

Go:   if x == nil {}
来源：http://hz.yangfankeji.com/gtwtsxqpgr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hz.aibaodan.cn/gtaknefyjd.html

C#:   if (x is null) {}
来源：http://hz.hammf.cn/gtldoozyke.html

[P07] 防抖与节流
来源：http://hz.iojbl.cn/gtjgyvsvrr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hz.sufxvd.cn/gtqgtfktxm.html

PHP:  // 手写时间戳比较
来源：http://hz.birdmap.top/gtrtnjizix.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.zdqjudy.top/gtgsvllzfj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fengsongda.top/gtrrtjydmo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hz.xinyue.icu/gtpopdsnoe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hz.yj20258.top/gtvskxjvcw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://hz.ybcxt.top/gtadnufgsv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hz.gotoacloud.top/gtersonhti.html

[P08] 处理浮点精度问题
来源：http://hz.xziqi.cn/gtkxxtmsun.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hz.shuidangran.top/gtuhahjfjh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hz.iojbl.cn/gtfjkedqzq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hz.iojbl.cn/gtmhbjvaum.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hz.xylfe.cn/gtusaravuu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hz.kuanghao11.cn/gtqzegorcq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hz.yonumen.top/gtzpufxrfb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hz.hnqzz.top/gtmmmuyiwy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hz.quarkkingdee.top/gtpwobdczw.html

================================================================================
来源：http://hz.shzxlz.cn/gtlyusknxw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hz.sysykeji.top/gtehuxxajb.html

================================================================================
来源：http://hz.zhongyouzk.top/gtipztttcm.html

[Q01] 创建表
来源：http://hz.daxiang520.top/gterlnkkkz.html

CREATE TABLE users (
来源：http://hz.jiagoushi.top/gteucptscb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.pycfn.com/gtebipymiy.html

name VARCHAR(50) NOT NULL,
来源：http://hz.yangfankeji.com/gtgofvdqif.html

email VARCHAR(100) UNIQUE,
来源：http://hz.aibaodan.cn/gtrfykdgcy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hz.hywenlv.cn/gtjkhdridi.html

);
来源：http://hz.0kj1m.cn/gtycqnhnyr.html

[Q02] 创建带外键的表
来源：http://hz.daria6918.cn/gtokodpuoo.html

CREATE TABLE orders (
来源：http://hz.zhixingplan.top/gthhywzane.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hz.gaohongyu789.top/gtlovborro.html

user_id INT NOT NULL,
来源：http://hz.jyoumei.cn/gtbvaajsph.html

amount DECIMAL(10, 2),
来源：http://hz.aibaodan.cn/gtwczynolq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hz.jinghuilouyu.cn/gtejngmnza.html

);
来源：http://hz.52xcode.cn/gtocdskqwx.html

[Q03] 增加列
来源：http://hz.jinghuilouyu.cn/gtzwvismah.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hz.gzhubu.top/gtgtocjtft.html

[Q04] 修改列类型
来源：http://hz.kuanghao11.cn/gtmxmtcmdj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hz.xziqi.cn/gtyavbdlng.html

[Q05] 重命名列
来源：http://hz.xuanzx.com/gtharunkhe.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hz.daria6918.cn/gtcpktopwv.html

[Q06] 删除列
来源：http://hz.hnxiangtu.top/gtxizwaiip.html

ALTER TABLE users DROP COLUMN age;
来源：http://hz.redwolf501.top/gtfirxubny.html

[Q07] 删除表
来源：http://hz.havefunace.top/gtayryzsnc.html

DROP TABLE IF EXISTS orders;
来源：http://hz.feifeiyinyue.top/gtbvkadtyi.html

[Q08] 创建普通索引
来源：http://hz.bjfxy.top/gtcloctohb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://hz.xuanzx.com/gthddrkqco.html

[Q09] 创建唯一索引
来源：http://hz.tianlin.xyz/gtsfwndnqh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hz.yonumen.top/gtyvwxuudm.html

[Q10] 插入单行
来源：http://hz.jyoumei.cn/gtcmfezafr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.shanyushiyangtech.top/gtmwugsmio.html

[Q11] 一次插入多行
来源：http://hz.aizwys.cn/gtezibmpxi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.hnxiangtu.top/gtjwmorhkr.html

[Q12] 插入后取自增 ID
来源：http://hz.sufxvd.cn/gttrwjdukr.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.zhiwuduotai.top/gtrbvrwzyq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.dashuyun.cn/gtnkkgsckf.html

[Q13] 忽略重复插入
来源：http://hz.hammf.cn/gtyxempnpo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.hysaishi.cn/gttpgjlned.html

[Q14] 存在则更新（upsert）
来源：http://hz.shanyushiyangtech.top/gtlkxybosh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.vqdsnc.cn/gtgbwpdprt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.meibo888.top/gthvffcrhr.html

[Q15] 查询全部
来源：http://hz.xylfe.cn/gtjpvfiavl.html

SELECT * FROM users;
来源：http://hz.hysaishi.cn/gteenkkfei.html

[Q16] 查询指定列
来源：http://hz.cqqwz.cn/gtuljbgcwq.html

SELECT id, name FROM users;
来源：http://hz.gaohongyu789.top/gtieevrsbm.html

[Q17] 条件查询
来源：http://hz.zhongyouzk.top/gttrlpgujh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.hywenlv.cn/gtygjvihoi.html

[Q18] 模糊匹配
来源：http://hz.daria6918.cn/gtgbeckajf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.redwolf501.top/gtirfaigwa.html

[Q19] 范围查询
来源：http://hz.havefunace.top/gtiveiflir.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.0kj1m.cn/gtklnccwyu.html

[Q20] IN 列表
来源：http://hz.daxiang520.top/gtfqmnvbes.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.aizwys.cn/gtzeirdhjx.html

[Q21] 空值判断
来源：http://hz.sxryk.cn/gtlarhdizt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.meibo888.top/gtktwtdwip.html

[Q22] 排序
来源：http://hz.tianlin.xyz/gtnsicrywv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gtswsddabi.html

[Q23] 分页
来源：http://hz.jiagoushi.top/gtnqusgzkk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jqgufenzy.top/gtngebkxqq.html

[Q24] 去重
来源：http://hz.tianlin.xyz/gthcfkugel.html

SELECT DISTINCT city FROM users;
来源：http://hz.andypj.xyz/gtdpnqkmgy.html

[Q25] 只取前 N 条
来源：http://hz.zhaomingkeji.xyz/gtfrgrodzt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.aizwys.cn/gtesimlghx.html

[Q26] 计数
来源：http://hz.cdnleiting.top/gtubkuvwsy.html

SELECT COUNT(*) FROM users;
来源：http://hz.hywenlv.cn/gtfqbsnkkl.html

[Q27] 条件计数
来源：http://hz.316326.xyz/gtsrmqnhtt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.havefunace.top/gtidxgjlix.html

[Q28] 求和与平均
来源：http://hz.gzhubu.top/gtjbfdpweq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xinyue.icu/gtljkpnnlp.html

[Q29] 最大最小值
来源：http://hz.sxryk.cn/gtogcmacgs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.pengpengdd.cyou/gtbwafqobb.html

[Q30] 分组统计
来源：http://hz.yuxming.cn/gtnznrdnpp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtimuqdxcb.html

[Q31] 分组后过滤
来源：http://hz.nanxuanxn.top/gtzjmdghfi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.sxryk.cn/gtvfosweul.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gtrcbrmkab.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtqvynbtaq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jqgfzy.top/gtuidwxinh.html

[Q33] 多列分组
来源：http://hz.daria6918.cn/gtwiyitkzm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.tian-w.cn/gtecfjkhls.html

[Q34] 每组取第一条
来源：http://hz.guowangkeji.top/gtsexwrpcb.html

SELECT * FROM (
来源：http://hz.yangfankeji.com/gtuoshcvrj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.quarkkingdee.top/gtklbsrbkg.html

) t WHERE rn = 1;
来源：http://hz.vqdsnc.cn/gtyjvgbndx.html

[Q35] 内连接
来源：http://hz.zycfv.cn/gtxupborpm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.daxiang520.top/gtoittpozb.html

[Q36] 左连接
来源：http://hz.hfpthk.cn/gtfqjahpuo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtmsiisnvc.html

[Q37] 右连接
来源：http://hz.cqqwz.cn/gtfkpkohoh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.svipenyu.cn/gtljfwnzyr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.9152youxi.cn/gtxrzakwjc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yj20258.top/gttjvvrjsp.html

[Q39] 自连接（查上下级）
来源：http://hz.zhoulong.xyz/gtkvbfobsm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhaomingkeji.xyz/gtwjwjyswa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.snrcjt.cn/gtqvhvtbls.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sysykeji.top/gtkatoptcu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.feifeiyinyue.top/gtfirmmlxc.html

[Q41] 多表连接
来源：http://hz.andypj.xyz/gtmfxgnlca.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.feifeiyinyue.top/gtinvehlxa.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xylfe.cn/gtkjciegji.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.haohaochexian.top/gtxlabsusa.html

[Q42] 连接条件附加过滤
来源：http://hz.tianlin.xyz/gtqlkertla.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nwbrower.top/gtkikfhtwr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.iojbl.cn/gthgmqxxte.html

[Q43] 标量子查询
来源：http://hz.ppjwa.cn/gtngalqevx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.quarkkingdee.top/gtgdhkzkml.html

[Q44] IN 子查询
来源：http://hz.52xcode.cn/gtclhwhacs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ywan-chungtsiang.top/gtcbimsfqv.html

[Q45] EXISTS 判断存在
来源：http://hz.guowangkeji.top/gttjblgqur.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtwvcjomsb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daria6918.cn/gtarsbxxio.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.meibo888.top/gtqelkhlys.html

[Q47] 与平均值比较
来源：http://hz.nanxuanxn.top/gtacdfkdyn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhijiandao.cn/gtnshamwig.html

[Q48] CTE 公用表表达式
来源：http://hz.yanxiufei.cn/gtgpkejekp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenlongwang.top/gtiukwsuem.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.meibo888.top/gtzepvxhvx.html

[Q49] 更新单行
来源：http://hz.iojbl.cn/gtamlbefoq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtexjgxhnw.html

[Q50] 批量更新
来源：http://hz.gaohongyu789.top/gtbvmoxvmy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xuetiantiany.cn/gtkpesjiui.html

[Q51] 用子查询更新
来源：http://hz.zhoulong.xyz/gtdatbiwdp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.svipenyu.cn/gtsjczhrvf.html

[Q52] 删除指定行
来源：http://hz.yueranfly.top/gtdudjkhih.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ywan-chungtsiang.top/gtbsovecgs.html

[Q53] 按条件删除
来源：http://hz.haohaochexian.top/gtyxsxtucw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtzdndrgvu.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtraojatcp.html

TRUNCATE TABLE logs;
来源：http://hz.guannengcc.top/gtkpmvrrat.html

[Q55] 排名（并列占位）
来源：http://hz.daxiang520.top/gtxcbzwocu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yj20258.top/gtrozumwbb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.vqdsnc.cn/gtupsysiiu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yongpay.top/gtozycbojr.html

[Q57] 行号
来源：http://hz.tian-w.cn/gtcjcetjis.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinyuanbaomall.cn/gtocwbmqcb.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gtofegifsh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gotoacloud.top/gtziyrqwnl.html

[Q59] 分组内累计
来源：http://hz.yj202588.top/gtbptaiame.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.haohaochexian.top/gtghchagsh.html

[Q60] 取上一行 / 下一行
来源：http://hz.fengsongda.top/gtsrnzekgw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gaohongyu789.top/gtarqkdism.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gaohongyu789.top/gtvqvajvyj.html

[Q61] 移动平均
来源：http://hz.ppjwa.cn/gtinjrkslm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenjidiqi.icu/gtoxgaxdvs.html

[Q62] 分组占比
来源：http://hz.gogol.net.cn/gtrdzwlwau.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.nanxinkj.top/gtzmhzgrqz.html

[Q63] 开启事务
来源：http://hz.tianlin.xyz/gtmdkrxblq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yvedp.cn/gtqaisntfe.html

[Q64] 提交事务
来源：http://hz.gzhubu.top/gtfmqbyhto.html

COMMIT;
来源：http://hz.yueranfly.top/gtqesmvkyl.html

[Q65] 回滚事务
来源：http://hz.jyoumei.cn/gtxfebgrpf.html

ROLLBACK;
来源：http://hz.tianlin.xyz/gtnfzutxmp.html

[Q66] 行锁查询
来源：http://hz.hfpthk.cn/gtbyiacipv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.pycfn.com/gtkmsxgzly.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gtxcolovwn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zdqjudy.top/gtiwkwousr.html

[Q68] 保存点
来源：http://hz.dianchejie.cn/gtwouhswwz.html

SAVEPOINT sp1;
来源：http://hz.yangfankeji.com/gtdzqekqbz.html

ROLLBACK TO sp1;
来源：http://hz.hammf.cn/gtuucrgjac.html

[Q69] 查看执行计划
来源：http://hz.zhaomingkeji.xyz/gtchgoybzg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hammf.cn/gtsggpeocr.html

[Q70] 更新统计信息
来源：http://hz.nwbrower.top/gtgrhebeho.html

ANALYZE TABLE users;
来源：http://hz.52xcode.cn/gttfcldoxz.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtrlpbzvvf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cqqwz.cn/gthahpletg.html

[Q72] 查看索引
来源：http://hz.yonumen.top/gtsclcswba.html

SHOW INDEX FROM users;
来源：http://hz.xuetiantiany.cn/gtqtpolwka.html

[Q73] 查看表状态
来源：http://hz.aibaodan.cn/gtnqkchqyg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guowangkeji.top/gtpwehrowt.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtwqkewycs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj202588.top/gtfdsyljkg.html

[Q75] 日期格式化
来源：http://hz.yj20258.top/gtoenpdyso.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jlsjyb.cn/gtptzkdkju.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.iojbl.cn/gtzwjgamxg.html

[Q76] 按天统计
来源：http://hz.xziqi.cn/gtncgyzdyn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinghuilouyu.cn/gtdizmdljx.html

[Q77] 时间加减
来源：http://hz.snrcjt.cn/gtyglsumos.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.316326.xyz/gtjnbpxxko.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gttcdgidse.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.haohaochexian.top/gtzvihkaha.html

[Q79] 字符串拼接
来源：http://hz.yuxming.cn/gtsifmpoxr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hammf.cn/gtqoporwoo.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gtjzielxak.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gtqqqlktbk.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtklmdfhzk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenzaomai.com/gtncmymxnz.html

[Q82] 字符长度与字节长度
来源：http://hz.quarkkingdee.top/gtvcgjjueh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.52xcode.cn/gtpaqitgxi.html

[Q83] 大小写转换
来源：http://hz.hysaishi.cn/gtzkmgpjax.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gaohongyu789.top/gtwdgeacvb.html

[Q84] 去除首尾空格
来源：http://hz.pengpengdd.cyou/gtkpfldmur.html

SELECT TRIM(name) FROM users;
来源：http://hz.9152youxi.cn/gtfdxuqtsa.html

[Q85] 数值取整
来源：http://hz.xuanzx.com/gtkdtjwmey.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangshuangyany.cn/gtnkoeuhuq.html

[Q86] 读取 JSON 字段
来源：http://hz.hammf.cn/gteldvhgys.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258.top/gtttrubjvi.html

[Q87] JSON 字段做条件
来源：http://hz.yvedp.cn/gtvpejiuhu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.kuanghao11.cn/gtyjrlurhx.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxuanxn.top/gtkjmnscmx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.havefunace.top/gtwsdirojk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtftqgolzv.html

[Q89] 判断表是否存在
来源：http://hz.xziqi.cn/gtwfwyqpcb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sxryk.cn/gtbunhlbau.html

[Q90] 生成序号列
来源：http://hz.vqdsnc.cn/gtijdywoio.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jlsjyb.cn/gtepafdcnk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkorqvymb.html

R. Bash 专题
来源：http://hz.sxryk.cn/gtkpqzxupw.html

================================================================================
来源：http://hz.yj20258888.top/gtzfkpyaiq.html

[R01] shebang 与严格模式
来源：http://hz.zdqjudy.top/gtnekpinwv.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gtjpifyzwx.html

set -euo pipefail
来源：http://hz.smart0.xyz/gthdyeblju.html

[R02] 变量赋值与使用
来源：http://hz.jqgfzy.top/gtxjxrlzij.html

name="Tom"; echo "$name"
来源：http://hz.meibo888.top/gttrbillef.html

[R03] 只读变量
来源：http://hz.guowangkeji.top/gtkuievteu.html

readonly PI=3.14
来源：http://hz.andypj.xyz/gtycrinsgo.html

[R04] 位置参数
来源：http://hz.gaohongyu789.top/gtiksevnbq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuanzhike.top/gtqporvhwh.html

[R05] 参数默认值
来源：http://hz.jlsjyb.cn/gtkgzrknuh.html

name="${1:-default}"
来源：http://hz.sweek.top/gtkpmtnoba.html

[R06] 判断命令是否存在
来源：http://hz.hfpthk.cn/gtvackcqcq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sxryk.cn/gtmxzqxqkh.html

[R07] if 判断文件
来源：http://hz.0kj1m.cn/gtwtvuxshf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhiwuduotai.top/gtcqyanbhh.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gtcztqkgwe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.snrcjt.cn/gtvadgsoxy.html

[R09] 字符串比较
来源：http://hz.havefunace.top/gtwwbwclob.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhaomingkeji.xyz/gtilujwdzs.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtodcrogya.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinghuilouyu.cn/gtuxgvajte.html

[R11] case 多分支
来源：http://hz.xinyue.icu/gtpipwbvgd.html

case "$1" in
来源：http://hz.dianchejie.cn/gtdbwmysok.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtxxlcdphy.html

stop)  echo "停止" ;;
来源：http://hz.dashuyun.cn/gtxihhsclr.html

*)     echo "未知命令" ;;
来源：http://hz.quarkkingdee.top/gtgbsouoqm.html

esac
来源：http://hz.shanyushiyangkeji.top/gtluupqcrd.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gtxdmamamg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuanzhike.top/gtoschcipd.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtrgqtfwvv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yvedp.cn/gtogisthqa.html

[R14] C 风格 for
来源：http://hz.jqgfzy.top/gtpdeqjpks.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gzhubu.top/gtkqlppash.html

[R15] while 逐行读文件
来源：http://hz.shangyingyoupin.top/gtwzatnhtj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gthgwbmdzn.html

[R16] until 等待条件
来源：http://hz.hongshengwenyu.top/gtxayuwdmu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gteoenvgzn.html

[R17] 数组定义与取值
来源：http://hz.iojbl.cn/gtqclnvaaf.html


<!-- 参考信息 -->