代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.c1oappe.top/gtrehnrlur.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.52xcode.cn/gtlpyhuizh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.zycfv.cn/gtmumdsekn.html

[Q15] 查询全部
来源：http://hz.cucudq.cn/gtjphwefgo.html

SELECT * FROM users;
来源：http://hz.jianghu66.top/gtqueiqjmg.html

[Q16] 查询指定列
来源：http://hz.gaohongyu789.top/gtnsvpzugp.html

SELECT id, name FROM users;
来源：http://hz.zycfv.cn/gtlwoivfgh.html

[Q17] 条件查询
来源：http://hz.jinqigfzy.top/gtnrqeepbv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.xingfuxueyuan.xyz/gtokdayigk.html

[Q18] 模糊匹配
来源：http://hz.ppjwa.cn/gtexgsgzgz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.yuanzhike.top/gteahzsstg.html

[Q19] 范围查询
来源：http://hz.tianlin.xyz/gtwhwxhhnq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.cqqwz.cn/gttstsxitj.html

[Q20] IN 列表
来源：http://hz.haohaochexian.top/gtixsjuvmb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.hysaishi.cn/gtghwynjzp.html

[Q21] 空值判断
来源：http://hz.xuanzx.com/gtoudhxoaw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.nanxuanxn.top/gtczdkzemr.html

[Q22] 排序
来源：http://hz.jyoumei.cn/gtcsqoaivd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.jlsjyb.cn/gtbumypxhu.html

[Q23] 分页
来源：http://hz.ppjwa.cn/gtezkoztzp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yuxming.cn/gtqfeiteom.html

[Q24] 去重
来源：http://hz.shangyingyoupin.top/gtlobpgicd.html

SELECT DISTINCT city FROM users;
来源：http://hz.feifeiyinyue.top/gtnsidppjp.html

[Q25] 只取前 N 条
来源：http://hz.gaohongyu789.top/gtsucltfwc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.redwolf501.top/gtnzubdffa.html

[Q26] 计数
来源：http://hz.yonumen.top/gtxhuktebe.html

SELECT COUNT(*) FROM users;
来源：http://hz.yonumen.top/gtalrnfzan.html

[Q27] 条件计数
来源：http://hz.jyoumei.cn/gtzpgzculb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.xuanzx.com/gtqmmrgora.html

[Q28] 求和与平均
来源：http://hz.dashuyun.cn/gtpfxejmhy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.mhx1999.top/gtbczxgplh.html

[Q29] 最大最小值
来源：http://hz.shuidangran.top/gtbjmffrtu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtlfnimvam.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtpuocltsb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.quarkkingdee.top/gtymwpzqht.html

[Q31] 分组后过滤
来源：http://hz.cashguo.top/gtyvphopok.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xingfuxueyuan.xyz/gtgdxcxrix.html

[Q32] 分组拼接字符串
来源：http://hz.guowangkeji.top/gtrmhwbpck.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.smart0.xyz/gtaychvtll.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtcsgxnqit.html

[Q33] 多列分组
来源：http://hz.vqdsnc.cn/gtumalwifr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.zdqjudy.top/gtexaooiof.html

[Q34] 每组取第一条
来源：http://hz.zhongyouzk.top/gttrlfrxxu.html

SELECT * FROM (
来源：http://hz.xinyue.icu/gtocsmhqjr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.zhengqikj.top/gtmkupomrz.html

) t WHERE rn = 1;
来源：http://hz.zhoulong.xyz/gtgmpmfdxr.html

[Q35] 内连接
来源：http://hz.yvedp.cn/gttlefqfyi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.snrcjt.cn/gtsbxswnub.html

[Q36] 左连接
来源：http://hz.sysykeji.top/gtaqgzmiyy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gzhubu.top/gttvufcoph.html

[Q37] 右连接
来源：http://hz.cashguo.top/gtpvxdqtdt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dianchejie.cn/gtbezckvro.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ivvv.top/gtjtmhkyre.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.daxiang520.top/gtvtrhtdrm.html

[Q39] 自连接（查上下级）
来源：http://hz.xziqi.cn/gtzrqljszt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xingfuxueyuan.xyz/gtkwbmktap.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jqgufenzy.top/gtawpiszyr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.52xcode.cn/gtnkixhdcz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cashguo.top/gtnzfdrfhe.html

[Q41] 多表连接
来源：http://hz.nanxinkj.top/gtzveuspem.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jiagoushi.top/gtmkbuviiw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhixingplan.top/gtvzlhanbd.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtghgcxvim.html

[Q42] 连接条件附加过滤
来源：http://hz.jinyuanbaomall.cn/gtlnqxgbpd.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gtkjcwjpcs.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.meibo888.top/gtkjmhxldq.html

[Q43] 标量子查询
来源：http://hz.zhoulong.xyz/gtkpvymnlm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yonumen.top/gtqibjoaql.html

[Q44] IN 子查询
来源：http://hz.snrcjt.cn/gtlkuyrtlf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.mhx1999.top/gtopsqjvpo.html

[Q45] EXISTS 判断存在
来源：http://hz.chenjidiqi.icu/gtpntvdbsy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhengqikj.top/gtxojrzcan.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.sxryk.cn/gtagagwawc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gtnqtsjmvt.html

[Q47] 与平均值比较
来源：http://hz.jinyuanbaomall.cn/gtjifyabmz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhiwuduotai.top/gtcacztxhz.html

[Q48] CTE 公用表表达式
来源：http://hz.hywenlv.cn/gtoawhaqsy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fzhhl.top/gtnpnohnry.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shangyingyoupin.top/gtmtzdzrln.html

[Q49] 更新单行
来源：http://hz.zhoulong.xyz/gtgehctypn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangdashe.top/gtvcdkskah.html

[Q50] 批量更新
来源：http://hz.aibaodan.cn/gtkmxofqmb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sxryk.cn/gtcxoxrhkl.html

[Q51] 用子查询更新
来源：http://hz.shangyingyoupin.top/gtakfesiwi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnqzz.top/gtsvstbnbq.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtdsfuobxg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtaymuebfo.html

[Q53] 按条件删除
来源：http://hz.havefunace.top/gtabgfpwjb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tianlin.xyz/gtcxybtkky.html

[Q54] 清空表
来源：http://hz.zhongyouzk.top/gtligzlhtp.html

TRUNCATE TABLE logs;
来源：http://hz.yueranfly.top/gtwgbplciu.html

[Q55] 排名（并列占位）
来源：http://hz.chenzaomai.com/gtzkjuntgm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yonumen.top/gtvrrbrvjh.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guowangkeji.top/gtihufvxej.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ppjwa.cn/gtvdlyzxuc.html

[Q57] 行号
来源：http://hz.316326.xyz/gtuzzyhabk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.smart0.xyz/gtovnksmlp.html

[Q58] 累计求和
来源：http://hz.xinyue.icu/gtmfobgnxd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtggnnagqj.html

[Q59] 分组内累计
来源：http://hz.zhoulong.xyz/gttddrpxqk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258.top/gtugmuegsk.html

[Q60] 取上一行 / 下一行
来源：http://hz.ywan-chungtsiang.top/gtxhfasgst.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gtzbwzrkxd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hysaishi.cn/gtudtlnsib.html

[Q61] 移动平均
来源：http://hz.smart0.xyz/gtmmbrstvq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.nanxinkj.top/gtqkbmbrep.html

[Q62] 分组占比
来源：http://hz.yj202588.top/gtlxcpjlyd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtvpywiqlo.html

[Q63] 开启事务
来源：http://hz.jinqigufen.top/gtwuwpqpao.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shangyingyoupin.top/gttlikdvwm.html

[Q64] 提交事务
来源：http://hz.nanxinkj.top/gtbfzivbin.html

COMMIT;
来源：http://hz.xinyue.icu/gtrkcbnfbx.html

[Q65] 回滚事务
来源：http://hz.vqdsnc.cn/gtigufcrkq.html

ROLLBACK;
来源：http://hz.zhaomingkeji.xyz/gtkbfxtrhs.html

[Q66] 行锁查询
来源：http://hz.shanyushiyangkeji.top/gtepbnpwik.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aizwys.cn/gttqqixtmn.html

[Q67] 设置隔离级别
来源：http://hz.tian-w.cn/gtbisxloup.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sysykeji.top/gtglmnshog.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtlpplihlm.html

SAVEPOINT sp1;
来源：http://hz.daria6918.cn/gtchrgetes.html

ROLLBACK TO sp1;
来源：http://hz.xuanzx.com/gtgzuzdgei.html

[Q69] 查看执行计划
来源：http://hz.zhongyouzk.top/gtbhhvysca.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gtdthdvvkq.html

[Q70] 更新统计信息
来源：http://hz.yuanzhike.top/gttrdwulhe.html

ANALYZE TABLE users;
来源：http://hz.feifeiyinyue.top/gtkxqtmrwv.html

[Q71] 查看建表语句
来源：http://hz.c1oappe.top/gtttuclyxj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinyuanbaomall.cn/gtksnaakan.html

[Q72] 查看索引
来源：http://hz.shzxlz.cn/gtkdwemmkt.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtyqxwwzst.html

[Q73] 查看表状态
来源：http://hz.chenzaomai.com/gtgnerqdvw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinyuanbaomall.cn/gtqhuptuyx.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtqgocoxjd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yanxiufei.cn/gthlfgtcdk.html

[Q75] 日期格式化
来源：http://hz.hfpthk.cn/gtouhxpren.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jqgfzy.top/gtbwunsjan.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gzhubu.top/gtyeezruyd.html

[Q76] 按天统计
来源：http://hz.jinyuanbaomall.cn/gtfmfdruor.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.vqdsnc.cn/gthgtxcxhk.html

[Q77] 时间加减
来源：http://hz.sufxvd.cn/gtbqeqauep.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtbiyhvcay.html

[Q78] 当前时间
来源：http://hz.jyoumei.cn/gtncwindij.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sufxvd.cn/gtjfsrmbhf.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtvyylkdya.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydjk.org.cn/gtjwoawepr.html

[Q80] 字符串截取
来源：http://hz.hongshengwenyu.top/gtitsmwrim.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jyoumei.cn/gtdwvgmhzv.html

[Q81] 字符串替换
来源：http://hz.zdqjudy.top/gtqgzukcab.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sweek.top/gtenxwozbg.html

[Q82] 字符长度与字节长度
来源：http://hz.zhixingplan.top/gtdlyugmxq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtrtjemrny.html

[Q83] 大小写转换
来源：http://hz.dashuyun.cn/gthsionseh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtmlkfmenz.html

[Q84] 去除首尾空格
来源：http://hz.yanxiufei.cn/gtcfbjsqvz.html

SELECT TRIM(name) FROM users;
来源：http://hz.meibo888.top/gteflhoyds.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtxmroxvsd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gtqwhtztmv.html

[Q86] 读取 JSON 字段
来源：http://hz.xuanzx.com/gtatsryrpk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuanzx.com/gtncrxxspm.html

[Q87] JSON 字段做条件
来源：http://hz.guannengcc.top/gtmtaoffhj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtnmuowknx.html

[Q88] 行转列（条件聚合）
来源：http://hz.andypj.xyz/gtzvcdgqvj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guowangkeji.top/gteyyuvkhs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtbciuzeqe.html

[Q89] 判断表是否存在
来源：http://hz.bjfxy.top/gtqxkqupzp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jiagoushi.top/gtqpjnwjcu.html

[Q90] 生成序号列
来源：http://hz.jqgufenzy.top/gtwkhhbmdb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnxiangtu.top/gtpxrcvmbm.html

================================================================================
来源：http://hz.nanxinkj.top/gtsxlieijl.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtfebltqkz.html

================================================================================
来源：http://hz.xuanzx.com/gtgwyneqbf.html

[R01] shebang 与严格模式
来源：http://hz.ybcxt.top/gtoeluioza.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtecgfdzzg.html

set -euo pipefail
来源：http://hz.andypj.xyz/gtmjollxky.html

[R02] 变量赋值与使用
来源：http://hz.hammf.cn/gtkqqgmwoc.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gttwhnjlbt.html

[R03] 只读变量
来源：http://hz.cdnleiting.top/gtzpmfgcap.html

readonly PI=3.14
来源：http://hz.nanxinkj.top/gtwxbsssyn.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtobmloouh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.cashguo.top/gtnudphfew.html

[R05] 参数默认值
来源：http://hz.zycfv.cn/gtsguqkcnz.html

name="${1:-default}"
来源：http://hz.316326.xyz/gtledrvlzi.html

[R06] 判断命令是否存在
来源：http://hz.chenjidiqi.icu/gtdstwjwxt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.mhx1999.top/gtyhryobgk.html

[R07] if 判断文件
来源：http://hz.316326.xyz/gtrziuhnvk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.feifeiyinyue.top/gtwjnjozdq.html

[R08] 数值比较
来源：http://hz.gotoacloud.top/gtxgvlejvr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.hysaishi.cn/gtaexwydks.html

[R09] 字符串比较
来源：http://hz.sufxvd.cn/gtgxeexaol.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.kuanghao11.cn/gtiytzudpr.html

[R10] 正则匹配
来源：http://hz.yanxiufei.cn/gtgbnywgjx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gogol.net.cn/gtbpanlagz.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtcdkliemw.html

case "$1" in
来源：http://hz.jinqigfzy.top/gtveclelpi.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtrbmaghue.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtegdfhels.html

*)     echo "未知命令" ;;
来源：http://hz.chenlongwang.top/gtrjbcpukb.html

esac
来源：http://hz.xingfuxueyuan.xyz/gtqmnbqddy.html

[R12] for 遍历文件
来源：http://hz.yongpay.top/gtfirsxhio.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jlsjyb.cn/gtavuhdxag.html

[R13] for 计数循环
来源：http://hz.havefunace.top/gtbxyzhtzk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtarkwgtas.html

[R14] C 风格 for
来源：http://hz.yj20258888.top/gtpytxorov.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtzbpewfjd.html

[R15] while 逐行读文件
来源：http://hz.smart0.xyz/gtvlimxbom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtarktwfze.html

[R16] until 等待条件
来源：http://hz.redwolf501.top/gtzgdfuuia.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtvejdjxsi.html

[R17] 数组定义与取值
来源：http://hz.shuidangran.top/gtvxikrelh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.snrcjt.cn/gtpszpxwoc.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gtbxwljtii.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cdnleiting.top/gtnnjwmljf.html

[R19] 数组长度
来源：http://hz.zycfv.cn/gtxextqdyp.html

echo "${#arr[@]}"
来源：http://hz.jinghuilouyu.cn/gtlvdpffsl.html

[R20] 关联数组（字典）
来源：http://hz.ehwqpu.com/gtbrosqbgl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dianchejie.cn/gthgpqumgo.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtinopszto.html

echo "${#s}"
来源：http://hz.sxryk.cn/gtpkvmyngg.html

[R22] 截取子串
来源：http://hz.tian-w.cn/gtilauxdhz.html

echo "${s:0:5}"
来源：http://hz.hysaishi.cn/gtlxzfuqxq.html

[R23] 字符串替换
来源：http://hz.jinqigufen.top/gtwzvsoqxn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuanzx.com/gtqkucsjlv.html

[R24] 大小写转换
来源：http://hz.zhijiandao.cn/gtnpmxjagg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgufenzy.top/gtgpfwlgkr.html

[R25] 去后缀 / 去前缀
来源：http://hz.gaohongyu789.top/gtsakzcmqt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenlongwang.top/gtslogdzdi.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtxwxcacfh.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtsinzrxgr.html

[R27] 算术展开
来源：http://hz.tanke756.top/gtztyhdwvh.html

echo $((1 + 2 * 3))
来源：http://hz.cheryme.top/gtwaqulstg.html

[R28] 浮点运算
来源：http://hz.nanxuanxn.top/gtgklpxiaw.html

echo "scale=2; 10/3" | bc
来源：http://hz.yonumen.top/gtdtnxfbyd.html

[R29] 定义函数
来源：http://hz.guowangkeji.top/gtmgspamuq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinyuanbaomall.cn/gtqxsmtvts.html

[R30] 函数返回状态码
来源：http://hz.zhiwuduotai.top/gtfhbyqnco.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cashguo.top/gtnufohrcf.html

[R31] 局部变量
来源：http://hz.pycfn.com/gtuzlqhafw.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhijiandao.cn/gtkblmvhxv.html

[R32] 参数个数校验
来源：http://hz.cucudq.cn/gtvfudmnxi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zdqjudy.top/gtxsnggccs.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtvzuqigtg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tanke756.top/gtucyyaael.html

[R34] 退出时清理
来源：http://hz.gaohongyu789.top/gtdtadltbd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtzqokytbe.html

[R35] 后台执行并等待
来源：http://hz.zhijiandao.cn/gtcxnowvay.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.svipenyu.cn/gtoymfgktp.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtsfwqxmdp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cucudq.cn/gtrvdzondt.html

[R37] 把输出赋给变量
来源：http://hz.svipenyu.cn/gtynbawapm.html

files=$(ls -1)
来源：http://hz.ydzc1.top/gtsdhtvaae.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gtxsyamqgq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yangfankeji.com/gtnoxgfyxi.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtgremifzz.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gtxccanumt.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtshcqxzkp.html

echo "log" >> out.log
来源：http://hz.yj20258888.top/gteitjwtrw.html

[R41] 丢弃输出
来源：http://hz.yvedp.cn/gtcphqbjso.html

cmd >/dev/null 2>&1
来源：http://hz.hysaishi.cn/gtmnvfxxjq.html

[R42] 输入重定向
来源：http://hz.shuidangran.top/gtvjvdyhds.html

wc -l < a.txt
来源：http://hz.quarkkingdee.top/gtxrnnyrln.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtzwnswrri.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gtshldjemu.html

[R44] 按修改时间查找
来源：http://hz.gotoacloud.top/gtndmtikso.html

find . -mtime -7 -type f
来源：http://hz.guannengcc.top/gtpzcvlltu.html

[R45] 批量删除
来源：http://hz.feifeiyinyue.top/gtzsauahgs.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigfzy.top/gtodwcmaab.html

[R46] 递归替换文件内容
来源：http://hz.hnqzz.top/gtxkesukzl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhiwuduotai.top/gtfaakaapm.html

[R47] sed 单行替换
来源：http://hz.ydzc1.top/gtisrfhjoo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yangfankeji.com/gtvouyvabl.html

[R48] awk 取指定列
来源：http://hz.chenjidiqi.icu/gteaxdorab.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhijiandao.cn/gtjxygaqgh.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtzaaconav.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.bjfxy.top/gtgvqmarxx.html

[R50] awk 求和
来源：http://hz.shanyushiyangkeji.top/gtvfuxcjcv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cheryme.top/gtiuvuytcd.html

[R51] 排序去重取前几
来源：http://hz.ppjwa.cn/gtdfvegyia.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xingfuxueyuan.xyz/gtvidqbdpk.html

[R52] 统计行数
来源：http://hz.yangfankeji.com/gtuowslxau.html

wc -l a.txt
来源：http://hz.wangdashe.top/gtgrjkmivr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhijiandao.cn/gtdstabzsi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtmqnjhxut.html

[R54] 比较两个文件
来源：http://hz.meibo888.top/gtmvgyszvh.html

diff a.txt b.txt
来源：http://hz.yangfankeji.com/gtvxsdgced.html

[R55] 压缩与解压
来源：http://hz.cqqwz.cn/gtnoipvknr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigufen.top/gtocdtmneh.html

[R56] 远程拷贝
来源：http://hz.tian-w.cn/gtfgnsleyc.html

scp file user@host:/path/
来源：http://hz.zhengqikj.top/gtywajrlfm.html

[R57] 远程执行命令
来源：http://hz.gzhubu.top/gtdlqwbbek.html

ssh user@host 'uptime'
来源：http://hz.hysaishi.cn/gtsycfwwso.html

[R58] 下载文件
来源：http://hz.iojbl.cn/gtznhxibmp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yongpay.top/gtfqmrwtwa.html

[R59] 发 POST JSON
来源：http://hz.jinqigfzy.top/gtzvgapoxt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gtdvkfsgow.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtslwwlvoo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydjk.org.cn/gtwdckfloy.html

[R61] 磁盘占用
来源：http://hz.chenzaomai.com/gthqtbxtbz.html

df -h;  du -sh *
来源：http://hz.52xcode.cn/gtbymxklfh.html

[R62] 找最占空间的文件
来源：http://hz.tanke756.top/gtlhbwreie.html

du -ah . | sort -rh | head -10
来源：http://hz.ydzc1.top/gtrjdlbxax.html

[R63] 内存与进程
来源：http://hz.smart0.xyz/gtvkvgdwwq.html


<!-- 参考信息 -->