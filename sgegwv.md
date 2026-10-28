代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.birdmap.top/gtoapmtrph.html

[Q11] 一次插入多行
来源：http://hz.ivvv.top/gtnlivoxnf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.shuidangran.top/gtrozqtoak.html

[Q12] 插入后取自增 ID
来源：http://hz.sysykeji.top/gtnlawtlhi.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xinyue.icu/gtofnlseaz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.jinyuanbaomall.cn/gtzaulhsvs.html

[Q13] 忽略重复插入
来源：http://hz.shzxlz.cn/gthvefuhhy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yj202588.top/gtdqhssqbo.html

[Q14] 存在则更新（upsert）
来源：http://hz.ppjwa.cn/gtjelnascy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.zhoulong.xyz/gtjfcsoymw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xinyue.icu/gtqprxtqff.html

[Q15] 查询全部
来源：http://hz.ydjk.org.cn/gtnrvbptid.html

SELECT * FROM users;
来源：http://hz.gzhubu.top/gtnswlnovq.html

[Q16] 查询指定列
来源：http://hz.shuidangran.top/gtqbkyojom.html

SELECT id, name FROM users;
来源：http://hz.shanyushiyangkeji.top/gtcfhszvva.html

[Q17] 条件查询
来源：http://hz.zhengqikj.top/gtloxijjod.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.andypj.xyz/gtfzfnbonw.html

[Q18] 模糊匹配
来源：http://hz.ydjk.org.cn/gttgbrhqyg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ppjwa.cn/gtggkwllns.html

[Q19] 范围查询
来源：http://hz.yj20258888.top/gtdxnymrpc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.316326.xyz/gtfvyzpdhy.html

[Q20] IN 列表
来源：http://hz.yj20258888.top/gtdpzkgazf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.aizwys.cn/gtoawrrfic.html

[Q21] 空值判断
来源：http://hz.jqgufenzy.top/gtifevuhok.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jqgufenzy.top/gtwzlntbjg.html

[Q22] 排序
来源：http://hz.iojbl.cn/gtfnesyumw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gtsxysuxbh.html

[Q23] 分页
来源：http://hz.dashuyun.cn/gtamtoofwt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gzhubu.top/gtxskuzjxa.html

[Q24] 去重
来源：http://hz.ywan-chungtsiang.top/gtqnbosaxy.html

SELECT DISTINCT city FROM users;
来源：http://hz.xinyue.icu/gteujejppl.html

[Q25] 只取前 N 条
来源：http://hz.feifeiyinyue.top/gtnxgphosb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.52xcode.cn/gtfwhhfymc.html

[Q26] 计数
来源：http://hz.zdqjudy.top/gtdlytuwzu.html

SELECT COUNT(*) FROM users;
来源：http://hz.hongshengwenyu.top/gtrwrglwav.html

[Q27] 条件计数
来源：http://hz.chenzaomai.com/gtrijxiuev.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jqgufenzy.top/gtfnxounbo.html

[Q28] 求和与平均
来源：http://hz.zycfv.cn/gtkcrrteeq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shzxlz.cn/gtebpoilmc.html

[Q29] 最大最小值
来源：http://hz.wangdashe.top/gtawktqjwr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258.top/gthodyvnwe.html

[Q30] 分组统计
来源：http://hz.fzhhl.top/gtqqdqgdlb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.daria6918.cn/gtgzorfwba.html

[Q31] 分组后过滤
来源：http://hz.jinyuanbaomall.cn/gtdbnpiezl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yanxiufei.cn/gtrtmgksmm.html

[Q32] 分组拼接字符串
来源：http://hz.cucudq.cn/gtirzoophf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gogol.net.cn/gtwcuarkia.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cqqwz.cn/gtfvxvprfy.html

[Q33] 多列分组
来源：http://hz.xuanzx.com/gtuiyhfbxz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.gogol.net.cn/gtnxcwojoe.html

[Q34] 每组取第一条
来源：http://hz.mhx1999.top/gthgjnuosj.html

SELECT * FROM (
来源：http://hz.redwolf501.top/gtltfqzczk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.dianchejie.cn/gtlrwccpqu.html

) t WHERE rn = 1;
来源：http://hz.jinqigufen.top/gtrixgqutt.html

[Q35] 内连接
来源：http://hz.zhijiandao.cn/gttkifncfl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtdgbiqcyx.html

[Q36] 左连接
来源：http://hz.wangshuangyany.cn/gtbfxhyrbu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gtbhxlxxem.html

[Q37] 右连接
来源：http://hz.feifeiyinyue.top/gttjekhvmy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cdnleiting.top/gthqfmmzak.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.kuanghao11.cn/gtrhfmzlwn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.snrcjt.cn/gtlniutgyx.html

[Q39] 自连接（查上下级）
来源：http://hz.chenlongwang.top/gtpcniqsdc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxinkj.top/gtzaauqkxg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gtevkuujkr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gtgbzykiqc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yvedp.cn/gtuhkqeedd.html

[Q41] 多表连接
来源：http://hz.ydzc1.top/gtrogvzftw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnxiangtu.top/gtazeoqxdi.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigufen.top/gtiurkscaf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtwclzeqdf.html

[Q42] 连接条件附加过滤
来源：http://hz.feifeiyinyue.top/gtsmmmkwqq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ywan-chungtsiang.top/gtggkhapud.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangkeji.top/gtymxdtpdx.html

[Q43] 标量子查询
来源：http://hz.fzhhl.top/gtqecaofpo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gtqgoszpwa.html

[Q44] IN 子查询
来源：http://hz.fzhhl.top/gtzniurudi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinghuilouyu.cn/gtvmqlpkuv.html

[Q45] EXISTS 判断存在
来源：http://hz.yanxiufei.cn/gtafpismou.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cucudq.cn/gtjscahcxg.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.chenlongwang.top/gtvmszuedj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ybcxt.top/gtikapkgua.html

[Q47] 与平均值比较
来源：http://hz.quarkkingdee.top/gtctinobat.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtgdvxtykb.html

[Q48] CTE 公用表表达式
来源：http://hz.xinyue.icu/gthqyjcick.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.wangshuangyany.cn/gtvxojwtns.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.guannengcc.top/gtyukczidk.html

[Q49] 更新单行
来源：http://hz.xuanzx.com/gtalqyvjmt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.redwolf501.top/gtmehgffnr.html

[Q50] 批量更新
来源：http://hz.xinyue.icu/gtomvzvxcw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.birdmap.top/gtzvyhlrcx.html

[Q51] 用子查询更新
来源：http://hz.xuanzx.com/gtsbwyxjfh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shuidangran.top/gtmvsijzsd.html

[Q52] 删除指定行
来源：http://hz.nwbrower.top/gtacgvmewa.html

DELETE FROM users WHERE id = 10;
来源：http://hz.9152youxi.cn/gtsirbzmhl.html

[Q53] 按条件删除
来源：http://hz.ppjwa.cn/gteyenyedq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yonumen.top/gtpxcqqhaz.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gteliqebsw.html

TRUNCATE TABLE logs;
来源：http://hz.sysykeji.top/gtuzurxazi.html

[Q55] 排名（并列占位）
来源：http://hz.yueranfly.top/gttptwycso.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xylfe.cn/gtdcibgtfr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dashuyun.cn/gtpatemolv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtkteyzrjp.html

[Q57] 行号
来源：http://hz.zhiwuduotai.top/gtipdodyoh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shanyushiyangkeji.top/gtqrfkfdrb.html

[Q58] 累计求和
来源：http://hz.52xcode.cn/gtsqxmgirk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhoulong.xyz/gtvkaimcrd.html

[Q59] 分组内累计
来源：http://hz.shuidangran.top/gtqiulqwqs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gthicuanir.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuxming.cn/gtcscefccv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yongpay.top/gtlmczycin.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gogol.net.cn/gtwmbkpoxg.html

[Q61] 移动平均
来源：http://hz.hfpthk.cn/gtrnmolvwg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuanzhike.top/gtujzfxqia.html

[Q62] 分组占比
来源：http://hz.fzhhl.top/gttvvnztzz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gtzuybkmsa.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtgdorbspo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.kuanghao11.cn/gtvifnzerl.html

[Q64] 提交事务
来源：http://hz.gaohongyu789.top/gticfdecie.html

COMMIT;
来源：http://hz.nanxinkj.top/gtjevghsvq.html

[Q65] 回滚事务
来源：http://hz.snrcjt.cn/gtawnsurku.html

ROLLBACK;
来源：http://hz.gogol.net.cn/gtnefdtzfs.html

[Q66] 行锁查询
来源：http://hz.ydjk.org.cn/gtlojmstih.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gttxsmqifz.html

[Q67] 设置隔离级别
来源：http://hz.gaohongyu789.top/gthcnsydqu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aizwys.cn/gtatynaupw.html

[Q68] 保存点
来源：http://hz.quarkkingdee.top/gtcqcgqzhx.html

SAVEPOINT sp1;
来源：http://hz.cucudq.cn/gthjikgexq.html

ROLLBACK TO sp1;
来源：http://hz.c1oappe.top/gthvatnbep.html

[Q69] 查看执行计划
来源：http://hz.sufxvd.cn/gtbxymntgz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinqigfzy.top/gtfekfvyvz.html

[Q70] 更新统计信息
来源：http://hz.jinghuilouyu.cn/gthafbatno.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtrudhwoww.html

[Q71] 查看建表语句
来源：http://hz.jinghuilouyu.cn/gtwhzztsxq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtzcyfdjrb.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtanbuopwf.html

SHOW INDEX FROM users;
来源：http://hz.wangshuangyany.cn/gtqkinttrq.html

[Q73] 查看表状态
来源：http://hz.jlsjyb.cn/gtdfrdpxvv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydzc1.top/gtvszmsscr.html

[Q74] 强制使用索引
来源：http://hz.redwolf501.top/gtqskzymvj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhiwuduotai.top/gtqvfdmmkk.html

[Q75] 日期格式化
来源：http://hz.xuanzx.com/gtaqplxlql.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yueranfly.top/gtmduootqo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtkwmxonoh.html

[Q76] 按天统计
来源：http://hz.hysaishi.cn/gttnbtsgrj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.vqdsnc.cn/gtwitoccor.html

[Q77] 时间加减
来源：http://hz.tanke756.top/gtfzywjslc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnqzz.top/gtacppadqh.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtnyjyepls.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.ywan-chungtsiang.top/gteuqplkmk.html

[Q79] 字符串拼接
来源：http://hz.jinqigufen.top/gtqwfjobst.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangdashe.top/gtylbhvjqc.html

[Q80] 字符串截取
来源：http://hz.daria6918.cn/gtmnfhtlwk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jqgfzy.top/gtjawlolok.html

[Q81] 字符串替换
来源：http://hz.haohaochexian.top/gtzzevjiii.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gtcusgfuzf.html

[Q82] 字符长度与字节长度
来源：http://hz.tian-w.cn/gtrbhlnguj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tanke756.top/gtotxfzsxr.html

[Q83] 大小写转换
来源：http://hz.daxiang520.top/gtmuvwaiyx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.birdmap.top/gtbivrdqkn.html

[Q84] 去除首尾空格
来源：http://hz.zhixingplan.top/gtfpyxffiv.html

SELECT TRIM(name) FROM users;
来源：http://hz.xziqi.cn/gtbcprohxi.html

[Q85] 数值取整
来源：http://hz.aibaodan.cn/gtfuuzwqpj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xylfe.cn/gthmklukrn.html

[Q86] 读取 JSON 字段
来源：http://hz.dashuyun.cn/gtpcixxiff.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtjgrmavhl.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtjbbcqtbn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.birdmap.top/gttpedtxux.html

[Q88] 行转列（条件聚合）
来源：http://hz.yvedp.cn/gtuuvozoxg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daxiang520.top/gtumtaobhu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtbashcekp.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gtxnzkgskv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hywenlv.cn/gtxndtmnpi.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtesubgldf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xingfuxueyuan.xyz/gtspxnhyhf.html

================================================================================
来源：http://hz.ybcxt.top/gtiakjswyn.html

R. Bash 专题
来源：http://hz.yj20258.top/gtlftwheyn.html

================================================================================
来源：http://hz.xylfe.cn/gteukqqqsp.html

[R01] shebang 与严格模式
来源：http://hz.yangfankeji.com/gtaomamepr.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtslonvvne.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtvsnoptrq.html

[R02] 变量赋值与使用
来源：http://hz.sxryk.cn/gtjilkrqfo.html

name="Tom"; echo "$name"
来源：http://hz.fzhhl.top/gtbtuulbpb.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gtubzmsmqe.html

readonly PI=3.14
来源：http://hz.pengpengdd.cyou/gtxxzzerwf.html

[R04] 位置参数
来源：http://hz.jlsjyb.cn/gtkqtahpym.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.c1oappe.top/gtomkhhkbt.html

[R05] 参数默认值
来源：http://hz.cashguo.top/gtiianxmmx.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtxjfkvrxq.html

[R06] 判断命令是否存在
来源：http://hz.9152youxi.cn/gtqhgbsosc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tian-w.cn/gtfqslumfc.html

[R07] if 判断文件
来源：http://hz.zdqjudy.top/gtnmpdhjyb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cashguo.top/gtdeisxlhz.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtcvpnasgg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtjqjzicjt.html

[R09] 字符串比较
来源：http://hz.xziqi.cn/gtmznpatav.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtefplhqet.html

[R10] 正则匹配
来源：http://hz.cheryme.top/gtyjpajppp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gtouvrtujy.html

[R11] case 多分支
来源：http://hz.9152youxi.cn/gtcgrctvyj.html

case "$1" in
来源：http://hz.xylfe.cn/gtvspzgowt.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtwseehjch.html

stop)  echo "停止" ;;
来源：http://hz.hammf.cn/gthykmojab.html

*)     echo "未知命令" ;;
来源：http://hz.tanke756.top/gtlcazxbdo.html

esac
来源：http://hz.nanxinkj.top/gtxeinmxwi.html

[R12] for 遍历文件
来源：http://hz.xuanzx.com/gtdpbsdoof.html

for f in *.txt; do echo "$f"; done
来源：http://hz.andypj.xyz/gtubzdumbr.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtgaxramrc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydzc1.top/gtgbdgpifn.html

[R14] C 风格 for
来源：http://hz.nanxuanxn.top/gtvkxpkqsg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gtbeltmxfk.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gtkuvrtfqs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ppjwa.cn/gtufuhxdss.html

[R16] until 等待条件
来源：http://hz.jinqigufen.top/gtqlkophuc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtgixifxzc.html

[R17] 数组定义与取值
来源：http://hz.ivvv.top/gtntxgnmrx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sufxvd.cn/gtlloctode.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtkvitvnro.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xziqi.cn/gtpujdsphg.html

[R19] 数组长度
来源：http://hz.birdmap.top/gtrroseybg.html

echo "${#arr[@]}"
来源：http://hz.xuanzx.com/gtdftcibps.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gtdvjlobgp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yueranfly.top/gtbhfpjnht.html

[R21] 字符串长度
来源：http://hz.svipenyu.cn/gtujvvwyzl.html

echo "${#s}"
来源：http://hz.sweek.top/gtwvgocwmz.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtmvmeaqnm.html

echo "${s:0:5}"
来源：http://hz.chenlongwang.top/gtmqymthvn.html

[R23] 字符串替换
来源：http://hz.hnxiangtu.top/gtjvltqpjn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.smart0.xyz/gtlkxtpopa.html

[R24] 大小写转换
来源：http://hz.yj20258888.top/gtzawnzshb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangshuangyany.cn/gtmwvarpbg.html

[R25] 去后缀 / 去前缀
来源：http://hz.shzxlz.cn/gteddflrsu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jiagoushi.top/gtezepymyj.html

[R26] 命令替换
来源：http://hz.xylfe.cn/gtjiryjfyp.html

now=$(date +%F); echo "$now"
来源：http://hz.gaohongyu789.top/gtvlepmpir.html

[R27] 算术展开
来源：http://hz.shangyingyoupin.top/gtqxgignyn.html

echo $((1 + 2 * 3))
来源：http://hz.iojbl.cn/gtaalxmorr.html

[R28] 浮点运算
来源：http://hz.hnxiangtu.top/gtfmuqlaqj.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtmopnphae.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtxzgeoyog.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aibaodan.cn/gtkslhkjxy.html

[R30] 函数返回状态码
来源：http://hz.quarkkingdee.top/gtvqqjinuz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.snrcjt.cn/gtkxfucunl.html

[R31] 局部变量
来源：http://hz.dianchejie.cn/gtvexbgcnk.html

f() { local x=1; echo "$x"; }
来源：http://hz.andypj.xyz/gtrrwbxpin.html

[R32] 参数个数校验
来源：http://hz.zhixingplan.top/gtyndvlthm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtwhvjqkna.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtbtraerxq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258888.top/gthiyklgst.html

[R34] 退出时清理
来源：http://hz.ydzc1.top/gtrghsucyx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtcagmcagm.html

[R35] 后台执行并等待
来源：http://hz.dianchejie.cn/gtvbjglajy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtbdjeboab.html

[R36] 并发执行多个任务
来源：http://hz.xingfuxueyuan.xyz/gtastmhcyk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gthmbvsegl.html

[R37] 把输出赋给变量
来源：http://hz.daxiang520.top/gthxfjjeyj.html

files=$(ls -1)
来源：http://hz.chenlongwang.top/gtumzxgckj.html

[R38] 管道串联
来源：http://hz.xingfuxueyuan.xyz/gtrsjhjsaw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shanyushiyangtech.top/gtbnlfjwyk.html

[R39] 重定向标准输出与错误
来源：http://hz.daxiang520.top/gtonxvjxho.html

cmd > out.log 2>&1
来源：http://hz.jinghuilouyu.cn/gtqxljdcmn.html

[R40] 追加写日志
来源：http://hz.gzhubu.top/gthqvqgnhc.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtkqbamlna.html

[R41] 丢弃输出
来源：http://hz.yonumen.top/gtyfkainet.html

cmd >/dev/null 2>&1
来源：http://hz.svipenyu.cn/gtstxrlvcq.html

[R42] 输入重定向
来源：http://hz.svipenyu.cn/gtfnsfpjaa.html

wc -l < a.txt
来源：http://hz.jyoumei.cn/gtmvldaboe.html

[R43] 按名字查找文件
来源：http://hz.shanyushiyangkeji.top/gtzvdsiflc.html

find . -name "*.log" -type f
来源：http://hz.yangfankeji.com/gtqkkffnbj.html

[R44] 按修改时间查找
来源：http://hz.nanxinkj.top/gtcokimazt.html

find . -mtime -7 -type f
来源：http://hz.shzxlz.cn/gtjmfreymd.html

[R45] 批量删除
来源：http://hz.smart0.xyz/gteeafjkep.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gtlezdoqbq.html

[R46] 递归替换文件内容
来源：http://hz.zhengqikj.top/gtqdgwhmnj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gtssreunot.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtsmmwbxff.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gtzwlvxwwz.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtrsxzngzd.html

awk '{print $1, $3}' a.txt
来源：http://hz.cqqwz.cn/gtzlmiogpn.html

[R49] awk 带条件
来源：http://hz.cheryme.top/gtlotmumwp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gzhubu.top/gtevzseidh.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gtectkbvdf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydjk.org.cn/gtgrtunpki.html

[R51] 排序去重取前几
来源：http://hz.xziqi.cn/gtuumgqqqt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xuetiantiany.cn/gtidmzosot.html

[R52] 统计行数
来源：http://hz.jinqigufen.top/gtulwtyhfk.html

wc -l a.txt
来源：http://hz.redwolf501.top/gthqtzhtxy.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258888.top/gtdsoldmnc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtrnmeemvs.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtgkxbypoi.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gtdobqaqls.html

[R55] 压缩与解压
来源：http://hz.gotoacloud.top/gtljrbzhxf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.meibo888.top/gtwoqfmfxm.html

[R56] 远程拷贝
来源：http://hz.haohaochexian.top/gtvkuwhjya.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtvxkvxmlq.html

[R57] 远程执行命令
来源：http://hz.yuanzhike.top/gtfduynkbe.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gteoaiiwqy.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtkhdiobcp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.fzhhl.top/gtuymxpfse.html

[R59] 发 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtzpkcxeya.html


<!-- 参考信息 -->