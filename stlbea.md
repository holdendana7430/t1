代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.xziqi.cn/gtstgsjoxi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.feifeiyinyue.top/gtolvderdq.html

[Q13] 忽略重复插入
来源：http://hz.jinghuilouyu.cn/gtodztejff.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.316326.xyz/gtxtdsrguw.html

[Q14] 存在则更新（upsert）
来源：http://hz.zhiwuduotai.top/gtjagitcci.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.aizwys.cn/gtickkevec.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.ivvv.top/gtgxbqoerl.html

[Q15] 查询全部
来源：http://hz.shanyushiyangtech.top/gtrqgojdkx.html

SELECT * FROM users;
来源：http://hz.ydjk.org.cn/gtqkcwbuln.html

[Q16] 查询指定列
来源：http://hz.quarkkingdee.top/gtmmswofml.html

SELECT id, name FROM users;
来源：http://hz.xylfe.cn/gtcrjnaili.html

[Q17] 条件查询
来源：http://hz.ywan-chungtsiang.top/gtfrfijlaz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yangfankeji.com/gtaumnratg.html

[Q18] 模糊匹配
来源：http://hz.52xcode.cn/gtottvcxtb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.gotoacloud.top/gtjdfltxfu.html

[Q19] 范围查询
来源：http://hz.zdqjudy.top/gtkxkzsrfs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.sufxvd.cn/gtjghzstax.html

[Q20] IN 列表
来源：http://hz.jinqigfzy.top/gtlazqlpaa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yvedp.cn/gtmxfenvjg.html

[Q21] 空值判断
来源：http://hz.pycfn.com/gtbccarrec.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinyuanbaomall.cn/gtmpbdifke.html

[Q22] 排序
来源：http://hz.tanke756.top/gtkbrmjkzv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ydjk.org.cn/gtrhxteqbo.html

[Q23] 分页
来源：http://hz.svipenyu.cn/gtihqhcaid.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.quarkkingdee.top/gtukckimcf.html

[Q24] 去重
来源：http://hz.zhengqikj.top/gtirfmhzqa.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhoulong.xyz/gtjbjhwyzg.html

[Q25] 只取前 N 条
来源：http://hz.ppjwa.cn/gtdgtxqxts.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.chenzaomai.com/gtxhbctdtq.html

[Q26] 计数
来源：http://hz.jinqigufen.top/gtsjvsikiv.html

SELECT COUNT(*) FROM users;
来源：http://hz.52xcode.cn/gtrenpqald.html

[Q27] 条件计数
来源：http://hz.yj202588.top/gtqzwejydc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jlsjyb.cn/gtiteoeklo.html

[Q28] 求和与平均
来源：http://hz.xuanzx.com/gtjyjyisnr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.fzhhl.top/gtvitpbsyk.html

[Q29] 最大最小值
来源：http://hz.xinyue.icu/gtmaospuhj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtgcgukieu.html

[Q30] 分组统计
来源：http://hz.cdnleiting.top/gtfnlfybds.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.52xcode.cn/gtdlrktmkk.html

[Q31] 分组后过滤
来源：http://hz.shangyingyoupin.top/gteqeiugrc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.iojbl.cn/gtiwisjvwx.html

[Q32] 分组拼接字符串
来源：http://hz.pengpengdd.cyou/gtrbmfsfbl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtqytoewnv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.snrcjt.cn/gtcfurnghf.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtdwljaqif.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ivvv.top/gtfkdbahso.html

[Q34] 每组取第一条
来源：http://hz.xylfe.cn/gtjbjggpty.html

SELECT * FROM (
来源：http://hz.quarkkingdee.top/gtpezzrrfh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.shangyingyoupin.top/gteiyandxz.html

) t WHERE rn = 1;
来源：http://hz.jyoumei.cn/gtbtzvcywg.html

[Q35] 内连接
来源：http://hz.zhoulong.xyz/gttnmdnqcd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gtuhjdmobs.html

[Q36] 左连接
来源：http://hz.ybcxt.top/gtpqfxxcbk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtkxkepubg.html

[Q37] 右连接
来源：http://hz.zhoulong.xyz/gtbiuxjspk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.tian-w.cn/gtiepzxbtg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sxryk.cn/gtiybyqkqq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.9152youxi.cn/gtjttxrzqr.html

[Q39] 自连接（查上下级）
来源：http://hz.zhixingplan.top/gtlhxvijfo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jlsjyb.cn/gtajqvropg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xziqi.cn/gtvastctqm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shangyingyoupin.top/gtwtuyjqov.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hammf.cn/gtgfgpjdhq.html

[Q41] 多表连接
来源：http://hz.316326.xyz/gtnactdsjd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yanxiufei.cn/gtejqolthh.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gthvgtacao.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.meibo888.top/gtqeeifzhp.html

[Q42] 连接条件附加过滤
来源：http://hz.zdqjudy.top/gtgsdypyyy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.birdmap.top/gtvhbbosxp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigufen.top/gthdwkaokt.html

[Q43] 标量子查询
来源：http://hz.yongpay.top/gtapinbzce.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.daxiang520.top/gtiszqvujr.html

[Q44] IN 子查询
来源：http://hz.sufxvd.cn/gtllyfzihf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenzaomai.com/gtgbiencsr.html

[Q45] EXISTS 判断存在
来源：http://hz.xylfe.cn/gtjvyvxqia.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtgovvotee.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shzxlz.cn/gtygbgrpwr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtgwracanc.html

[Q47] 与平均值比较
来源：http://hz.haohaochexian.top/gtgwrbzilt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cqqwz.cn/gtbgpmnjgi.html

[Q48] CTE 公用表表达式
来源：http://hz.jianghu66.top/gtcfpipqxe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.0kj1m.cn/gtiahjjjhl.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenjidiqi.icu/gtdqhvjcfd.html

[Q49] 更新单行
来源：http://hz.feifeiyinyue.top/gtgvymcqgq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.vqdsnc.cn/gtbuzyjlhs.html

[Q50] 批量更新
来源：http://hz.tianlin.xyz/gtcimyldlo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.bjfxy.top/gtxbllnlrd.html

[Q51] 用子查询更新
来源：http://hz.nwbrower.top/gtmjwmktux.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtkegqntwo.html

[Q52] 删除指定行
来源：http://hz.jinqigfzy.top/gtgcqtmvuu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhijiandao.cn/gtiyutuzyc.html

[Q53] 按条件删除
来源：http://hz.hywenlv.cn/gtcjulamry.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ehwqpu.com/gtuusweohv.html

[Q54] 清空表
来源：http://hz.jqgfzy.top/gtcpmlspyj.html

TRUNCATE TABLE logs;
来源：http://hz.daxiang520.top/gtfmglyndn.html

[Q55] 排名（并列占位）
来源：http://hz.cqqwz.cn/gtgekzzcvv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtovfsahsf.html

[Q56] 密集排名（并列不占位）
来源：http://hz.316326.xyz/gtagmhvufe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gzhubu.top/gtetbtbcxc.html

[Q57] 行号
来源：http://hz.meibo888.top/gtsmvpstec.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shangyingyoupin.top/gtznaxlpna.html

[Q58] 累计求和
来源：http://hz.dianchejie.cn/gtmlguppgj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtccamzabr.html

[Q59] 分组内累计
来源：http://hz.tanke756.top/gtrsrwqurh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhijiandao.cn/gtshikzysg.html

[Q60] 取上一行 / 下一行
来源：http://hz.gogol.net.cn/gtklpsrvwi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinqigfzy.top/gtkxjhjxxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sysykeji.top/gtnvwopotc.html

[Q61] 移动平均
来源：http://hz.hnxiangtu.top/gtnjkuqyqk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.shangyingyoupin.top/gtbzxrebyd.html

[Q62] 分组占比
来源：http://hz.yvedp.cn/gtjltfzsba.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ivvv.top/gtomztwgff.html

[Q63] 开启事务
来源：http://hz.gzhubu.top/gtqqbqqxqz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.snrcjt.cn/gtvgjomwvi.html

[Q64] 提交事务
来源：http://hz.shanyushiyangkeji.top/gtvxenzeew.html

COMMIT;
来源：http://hz.c1oappe.top/gthvgcsovi.html

[Q65] 回滚事务
来源：http://hz.cashguo.top/gtagdsdgnz.html

ROLLBACK;
来源：http://hz.meibo888.top/gtstltgviu.html

[Q66] 行锁查询
来源：http://hz.cheryme.top/gttonmejlw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cashguo.top/gtosnreeir.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtopjqlewv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.dashuyun.cn/gtfcvtogtm.html

[Q68] 保存点
来源：http://hz.yuxming.cn/gtkolmhmnm.html

SAVEPOINT sp1;
来源：http://hz.tianlin.xyz/gtlthurseu.html

ROLLBACK TO sp1;
来源：http://hz.0kj1m.cn/gtvgtirqpc.html

[Q69] 查看执行计划
来源：http://hz.yvedp.cn/gtawxjonon.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgufenzy.top/gtbqnburfk.html

[Q70] 更新统计信息
来源：http://hz.yangfankeji.com/gtgfvxgsfc.html

ANALYZE TABLE users;
来源：http://hz.tanke756.top/gttfkodlyu.html

[Q71] 查看建表语句
来源：http://hz.yuxming.cn/gtansqnupn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.gogol.net.cn/gtumlhxaoa.html

[Q72] 查看索引
来源：http://hz.feifeiyinyue.top/gtvapaquak.html

SHOW INDEX FROM users;
来源：http://hz.dashuyun.cn/gtpbanghxt.html

[Q73] 查看表状态
来源：http://hz.xziqi.cn/gtxyirvfin.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.quarkkingdee.top/gtxonmcgog.html

[Q74] 强制使用索引
来源：http://hz.ivvv.top/gtxngvobxq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hammf.cn/gtqltslvsx.html

[Q75] 日期格式化
来源：http://hz.pengpengdd.cyou/gtdjbztsku.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtkenjxxvv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zycfv.cn/gtudiuvwst.html

[Q76] 按天统计
来源：http://hz.sysykeji.top/gtcuotyowz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gteojcllll.html

[Q77] 时间加减
来源：http://hz.yj20258888.top/gtkdzyiwsj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pengpengdd.cyou/gtsnvjiieu.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtowpaymmx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenzaomai.com/gtvydybrwu.html

[Q79] 字符串拼接
来源：http://hz.jinqigfzy.top/gtfxjjqfog.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cashguo.top/gtmfdoswgc.html

[Q80] 字符串截取
来源：http://hz.chenjidiqi.icu/gtqkfzxvod.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hfpthk.cn/gtrecpeuvb.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangtech.top/gticboohef.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hysaishi.cn/gtedsbhajs.html

[Q82] 字符长度与字节长度
来源：http://hz.redwolf501.top/gtxtghfcon.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtuatrtxfb.html

[Q83] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtvsawebav.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuanzx.com/gttzxtxyks.html

[Q84] 去除首尾空格
来源：http://hz.jianghu66.top/gtesxtcuvc.html

SELECT TRIM(name) FROM users;
来源：http://hz.hywenlv.cn/gtzdyhlsfr.html

[Q85] 数值取整
来源：http://hz.xuanzx.com/gtnrijfdaw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.feifeiyinyue.top/gtjxdkodrr.html

[Q86] 读取 JSON 字段
来源：http://hz.sweek.top/gtmzibhtid.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtnkzrxedu.html

[Q87] JSON 字段做条件
来源：http://hz.tianlin.xyz/gtslhqvlag.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.snrcjt.cn/gtddrbaxtb.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gtraqdmcwa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtckkpdumz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhiwuduotai.top/gtzgzcygsq.html

[Q89] 判断表是否存在
来源：http://hz.nwbrower.top/gtnygcfwib.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yueranfly.top/gtemvsubeg.html

[Q90] 生成序号列
来源：http://hz.chenzaomai.com/gtpggtrmmq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.c1oappe.top/gtbzubfkfv.html

================================================================================
来源：http://hz.9152youxi.cn/gtxrarvaac.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtjrvijhxg.html

================================================================================
来源：http://hz.guowangkeji.top/gtznysncsz.html

[R01] shebang 与严格模式
来源：http://hz.pycfn.com/gtsfwaiuqo.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gtzisasvdn.html

set -euo pipefail
来源：http://hz.cheryme.top/gtlxhtlkef.html

[R02] 变量赋值与使用
来源：http://hz.ppjwa.cn/gtbgzxhzmf.html

name="Tom"; echo "$name"
来源：http://hz.feifeiyinyue.top/gtcomqhdeg.html

[R03] 只读变量
来源：http://hz.gotoacloud.top/gtcwvlbtia.html

readonly PI=3.14
来源：http://hz.c1oappe.top/gtqnsqmxgv.html

[R04] 位置参数
来源：http://hz.hnxiangtu.top/gttygvvuem.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hammf.cn/gtmlxmyycf.html

[R05] 参数默认值
来源：http://hz.pycfn.com/gtoufzsgsf.html

name="${1:-default}"
来源：http://hz.wangdashe.top/gtqdbxppll.html

[R06] 判断命令是否存在
来源：http://hz.yonumen.top/gtykjgcmas.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.316326.xyz/gtnfpuquao.html

[R07] if 判断文件
来源：http://hz.mhx1999.top/gtdgmsmlvs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gtjynjxxkv.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gttbnxisyl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.mhx1999.top/gtelwcottn.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtvrifrdhs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cqqwz.cn/gtwghuoyqz.html

[R10] 正则匹配
来源：http://hz.nanxinkj.top/gtvaoadcwb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zycfv.cn/gttlmkibql.html

[R11] case 多分支
来源：http://hz.kuanghao11.cn/gtykkumozd.html

case "$1" in
来源：http://hz.cheryme.top/gtesgeqaub.html

start) echo "启动" ;;
来源：http://hz.zhengqikj.top/gtsfjxlice.html

stop)  echo "停止" ;;
来源：http://hz.yuxming.cn/gtzrxulxpg.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtwjcepbxw.html

esac
来源：http://hz.guowangkeji.top/gttyjzmgcw.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtztvhmzam.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenzaomai.com/gtfiyexikn.html

[R13] for 计数循环
来源：http://hz.xingfuxueyuan.xyz/gtjjmptxeq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aibaodan.cn/gtyiugzbpu.html

[R14] C 风格 for
来源：http://hz.yj20258888.top/gthklnuxra.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cqqwz.cn/gtgkgqaomg.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gtfyjxuupe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aibaodan.cn/gtklmsxrau.html

[R16] until 等待条件
来源：http://hz.ydjk.org.cn/gtudgxsbpm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.c1oappe.top/gtdzlvdyqi.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gtfzkoolzm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gogol.net.cn/gtxvloslqc.html

[R18] 遍历数组
来源：http://hz.c1oappe.top/gtzsfnnzqr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtyfnnmqrf.html

[R19] 数组长度
来源：http://hz.shuidangran.top/gtyodchczf.html

echo "${#arr[@]}"
来源：http://hz.dianchejie.cn/gteipldtze.html

[R20] 关联数组（字典）
来源：http://hz.smart0.xyz/gtrottdcfm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shuidangran.top/gthpwkxxer.html

[R21] 字符串长度
来源：http://hz.zhongyouzk.top/gtqghchjmj.html

echo "${#s}"
来源：http://hz.yueranfly.top/gtpudjqthw.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtkbxioafx.html

echo "${s:0:5}"
来源：http://hz.nwbrower.top/gttaxbonok.html

[R23] 字符串替换
来源：http://hz.nanxinkj.top/gtmherqmnc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgufenzy.top/gtzkoiohie.html

[R24] 大小写转换
来源：http://hz.jinqigufen.top/gtmhyvtizn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.9152youxi.cn/gtoqqgdpwc.html

[R25] 去后缀 / 去前缀
来源：http://hz.ywan-chungtsiang.top/gterncoshm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtsvitobzr.html

[R26] 命令替换
来源：http://hz.zhaomingkeji.xyz/gttersywsi.html

now=$(date +%F); echo "$now"
来源：http://hz.jiagoushi.top/gtscrpsmvl.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtrbsxrszm.html

echo $((1 + 2 * 3))
来源：http://hz.aibaodan.cn/gtxpfdhmee.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtwdauylni.html

echo "scale=2; 10/3" | bc
来源：http://hz.jyoumei.cn/gtgkjxhlfb.html

[R29] 定义函数
来源：http://hz.shuidangran.top/gtteazktmf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhongyouzk.top/gtxmqivugq.html

[R30] 函数返回状态码
来源：http://hz.pycfn.com/gtbgvlhjii.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.mhx1999.top/gtiqwawpyz.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gthdnnlyhp.html

f() { local x=1; echo "$x"; }
来源：http://hz.sufxvd.cn/gtbufijveo.html

[R32] 参数个数校验
来源：http://hz.zhixingplan.top/gtxjntolxb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtfmwwaxgy.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gtfudjrzva.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangshuangyany.cn/gtjljcjiqq.html

[R34] 退出时清理
来源：http://hz.gaohongyu789.top/gtskqsomqb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtlfehukft.html

[R35] 后台执行并等待
来源：http://hz.ivvv.top/gtiuqrfwpx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ybcxt.top/gttbikrjjm.html

[R36] 并发执行多个任务
来源：http://hz.guowangkeji.top/gtboxcqveh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cqqwz.cn/gtsaospxyg.html

[R37] 把输出赋给变量
来源：http://hz.chenlongwang.top/gtwxgehghx.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtyjadhxlt.html

[R38] 管道串联
来源：http://hz.yueranfly.top/gtvkwfsxfm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuetiantiany.cn/gtvqqzcnxf.html

[R39] 重定向标准输出与错误
来源：http://hz.xinyue.icu/gtlydzgmyd.html

cmd > out.log 2>&1
来源：http://hz.jiagoushi.top/gthtgtthzv.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtxlochoie.html

echo "log" >> out.log
来源：http://hz.iojbl.cn/gtbbsuvcip.html

[R41] 丢弃输出
来源：http://hz.yangfankeji.com/gtvdjqnnnr.html

cmd >/dev/null 2>&1
来源：http://hz.yuxming.cn/gthihzinhl.html

[R42] 输入重定向
来源：http://hz.ppjwa.cn/gtiasqkkxv.html

wc -l < a.txt
来源：http://hz.xuetiantiany.cn/gtuaxhkgic.html

[R43] 按名字查找文件
来源：http://hz.dianchejie.cn/gtgwmqwujh.html

find . -name "*.log" -type f
来源：http://hz.xuanzx.com/gtvzelzrwn.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtaxutscua.html

find . -mtime -7 -type f
来源：http://hz.52xcode.cn/gtekijbhww.html

[R45] 批量删除
来源：http://hz.chenzaomai.com/gtytzdxoqi.html

find . -name "*.tmp" -delete
来源：http://hz.nwbrower.top/gtmgmpuoxs.html

[R46] 递归替换文件内容
来源：http://hz.pengpengdd.cyou/gtfipxxonq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yuanzhike.top/gtlxbyyhaj.html

[R47] sed 单行替换
来源：http://hz.sweek.top/gtqkxbkoer.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gtrtbnsexy.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtdbgrclvm.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gteodtrkqq.html

[R49] awk 带条件
来源：http://hz.gotoacloud.top/gtsuouectj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xylfe.cn/gtrtgefqwh.html

[R50] awk 求和
来源：http://hz.snrcjt.cn/gtxlexorsr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shuidangran.top/gtdnyzpqqs.html

[R51] 排序去重取前几
来源：http://hz.guannengcc.top/gttqslzmsb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhaomingkeji.xyz/gtabyrrndj.html

[R52] 统计行数
来源：http://hz.c1oappe.top/gtmavhvolg.html

wc -l a.txt
来源：http://hz.jianghu66.top/gtabblkyao.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtrjbwrgqa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.52xcode.cn/gtollhyoox.html

[R54] 比较两个文件
来源：http://hz.sxryk.cn/gttpayakln.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtyztjqnhm.html

[R55] 压缩与解压
来源：http://hz.cqqwz.cn/gtvupuavim.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yanxiufei.cn/gtvxuizczg.html

[R56] 远程拷贝
来源：http://hz.birdmap.top/gtnpzgekjo.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtzqwgiaap.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtmsslzwxv.html

ssh user@host 'uptime'
来源：http://hz.shuidangran.top/gtlekhfaha.html

[R58] 下载文件
来源：http://hz.mhx1999.top/gtvxkfxnok.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangkeji.top/gtglvbekxz.html

[R59] 发 POST JSON
来源：http://hz.xylfe.cn/gtklyrkxqz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yueranfly.top/gtdisktidg.html

[R60] 只看 HTTP 状态码
来源：http://hz.ybcxt.top/gthdjmwmun.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.wangdashe.top/gtummfkckh.html

[R61] 磁盘占用
来源：http://hz.zhoulong.xyz/gtylcregjk.html


<!-- 参考信息 -->