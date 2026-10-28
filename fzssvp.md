代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.gotoacloud.top/gtswylvxxe.html

[Q18] 模糊匹配
来源：http://hz.fzhhl.top/gtwozodqcy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.xylfe.cn/gtgzmedpey.html

[Q19] 范围查询
来源：http://hz.hnxiangtu.top/gtetsarzyw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.andypj.xyz/gtjrlvwvci.html

[Q20] IN 列表
来源：http://hz.jinqigufen.top/gthrpydhvq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gzhubu.top/gtyioewwsd.html

[Q21] 空值判断
来源：http://hz.iojbl.cn/gtovamapxj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.jinghuilouyu.cn/gtceyolwrt.html

[Q22] 排序
来源：http://hz.xziqi.cn/gtpctguecr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.tian-w.cn/gtbhftcdga.html

[Q23] 分页
来源：http://hz.zhaomingkeji.xyz/gtmjcgffhp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.jinqigufen.top/gtlehmbbzn.html

[Q24] 去重
来源：http://hz.xziqi.cn/gtokcrqbrc.html

SELECT DISTINCT city FROM users;
来源：http://hz.zycfv.cn/gtmdwtqgmm.html

[Q25] 只取前 N 条
来源：http://hz.shuidangran.top/gtgwtutprq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.svipenyu.cn/gtdasqneis.html

[Q26] 计数
来源：http://hz.hysaishi.cn/gttgkacmsu.html

SELECT COUNT(*) FROM users;
来源：http://hz.wangshuangyany.cn/gtgqpxvebv.html

[Q27] 条件计数
来源：http://hz.smart0.xyz/gtkgfiuapw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.nwbrower.top/gticadjfxr.html

[Q28] 求和与平均
来源：http://hz.nanxuanxn.top/gtkpgdimno.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zdqjudy.top/gtppzbtxvo.html

[Q29] 最大最小值
来源：http://hz.kuanghao11.cn/gtjayzfhpt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigfzy.top/gtffzhcebf.html

[Q30] 分组统计
来源：http://hz.ydjk.org.cn/gtjztqwoix.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.kuanghao11.cn/gtwunsyfua.html

[Q31] 分组后过滤
来源：http://hz.aibaodan.cn/gtbxqjzkss.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.gzhubu.top/gtgwpvdvuf.html

[Q32] 分组拼接字符串
来源：http://hz.zhixingplan.top/gtrunqujwo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtyrrovswl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.jinyuanbaomall.cn/gtrybfxwpp.html

[Q33] 多列分组
来源：http://hz.hysaishi.cn/gtqhvdzvni.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gtxemybgvy.html

[Q34] 每组取第一条
来源：http://hz.meibo888.top/gtpdriwjxu.html

SELECT * FROM (
来源：http://hz.ehwqpu.com/gtmeeophlq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daria6918.cn/gtxqqpqfbu.html

) t WHERE rn = 1;
来源：http://hz.52xcode.cn/gteeqpgqln.html

[Q35] 内连接
来源：http://hz.ehwqpu.com/gtwaezhgvf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shanyushiyangtech.top/gtvuowfejx.html

[Q36] 左连接
来源：http://hz.sxryk.cn/gtljhdmjok.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jinghuilouyu.cn/gtlumesltn.html

[Q37] 右连接
来源：http://hz.hammf.cn/gtnfhgarby.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxinkj.top/gtxutzskbg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cheryme.top/gtcpsvfzjv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xylfe.cn/gtbvwhkjcn.html

[Q39] 自连接（查上下级）
来源：http://hz.daxiang520.top/gtletvgaje.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinghuilouyu.cn/gtdqxqifrr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hfpthk.cn/gtkaofmwuc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.tanke756.top/gthdtqwdqc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guowangkeji.top/gtjhjamwhm.html

[Q41] 多表连接
来源：http://hz.ehwqpu.com/gtcekzgbyb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shuidangran.top/gtqwequyvm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yvedp.cn/gttcdgaokk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.andypj.xyz/gtjocxfbfi.html

[Q42] 连接条件附加过滤
来源：http://hz.iojbl.cn/gttlavimrz.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jianghu66.top/gtzrcaeavj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.quarkkingdee.top/gtubxhmdvm.html

[Q43] 标量子查询
来源：http://hz.tanke756.top/gtixbulnne.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.sweek.top/gthtvsiwxl.html

[Q44] IN 子查询
来源：http://hz.nwbrower.top/gtaqxqsvof.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.chenzaomai.com/gtwzkozbwf.html

[Q45] EXISTS 判断存在
来源：http://hz.jianghu66.top/gtgpxkzvfr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xziqi.cn/gtnwwnheon.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.daxiang520.top/gtrcgxqckv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yuanzhike.top/gtlkpprogp.html

[Q47] 与平均值比较
来源：http://hz.aibaodan.cn/gtommjmgmy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jiagoushi.top/gtdbqhhmgg.html

[Q48] CTE 公用表表达式
来源：http://hz.jinqigufen.top/gtprgwlxix.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangtech.top/gtulhakian.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gotoacloud.top/gtvnaqfikr.html

[Q49] 更新单行
来源：http://hz.nanxuanxn.top/gtcaphflnh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yanxiufei.cn/gtgzpblyhi.html

[Q50] 批量更新
来源：http://hz.yanxiufei.cn/gtnkfzbibu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.havefunace.top/gtomcgwfap.html

[Q51] 用子查询更新
来源：http://hz.52xcode.cn/gtuwkiqqre.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yj202588.top/gtozfrqzqj.html

[Q52] 删除指定行
来源：http://hz.yj20258.top/gtgyyvscvq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj202588.top/gtnnzobtpn.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtdvlhokun.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hnxiangtu.top/gtqzxvemcr.html

[Q54] 清空表
来源：http://hz.yongpay.top/gtxkqhdood.html

TRUNCATE TABLE logs;
来源：http://hz.daria6918.cn/gtbixbdihy.html

[Q55] 排名（并列占位）
来源：http://hz.xuanzx.com/gtmraponsr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ivvv.top/gtyjbsfgjn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhijiandao.cn/gtmngxwhje.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgfzy.top/gtxlmbzhsn.html

[Q57] 行号
来源：http://hz.ivvv.top/gtprhataoe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.kuanghao11.cn/gtxfxgkdcp.html

[Q58] 累计求和
来源：http://hz.sysykeji.top/gtbxgoehmw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhiwuduotai.top/gtmfgtzuxg.html

[Q59] 分组内累计
来源：http://hz.ybcxt.top/gtyoqteyiv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fzhhl.top/gtccoubzln.html

[Q60] 取上一行 / 下一行
来源：http://hz.kuanghao11.cn/gtmvwrfsft.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.daria6918.cn/gtzyjewjhm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ybcxt.top/gtjzdcjbpg.html

[Q61] 移动平均
来源：http://hz.fengsongda.top/gtbgeeerog.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigfzy.top/gtxmkgdxyr.html

[Q62] 分组占比
来源：http://hz.zycfv.cn/gtniuehook.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gturkssvck.html

[Q63] 开启事务
来源：http://hz.ivvv.top/gtmmixnfsh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jlsjyb.cn/gttmynpeew.html

[Q64] 提交事务
来源：http://hz.52xcode.cn/gtuwvsckts.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtliqterzy.html

[Q65] 回滚事务
来源：http://hz.yuanzhike.top/gtvbosppag.html

ROLLBACK;
来源：http://hz.jlsjyb.cn/gtywbmrjdr.html

[Q66] 行锁查询
来源：http://hz.zdqjudy.top/gtwxacwpzj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fzhhl.top/gtwwlvqqbv.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtplhoprfr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenlongwang.top/gtuzvyvqft.html

[Q68] 保存点
来源：http://hz.chenlongwang.top/gthzspvsrw.html

SAVEPOINT sp1;
来源：http://hz.cashguo.top/gtgcatgfpt.html

ROLLBACK TO sp1;
来源：http://hz.meibo888.top/gtrekpecny.html

[Q69] 查看执行计划
来源：http://hz.ydjk.org.cn/gtukkujlkx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhixingplan.top/gtmtwnzgak.html

[Q70] 更新统计信息
来源：http://hz.zhengqikj.top/gtwzpjycca.html

ANALYZE TABLE users;
来源：http://hz.chenjidiqi.icu/gtkvmsmwgu.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtthphkzsx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gthapwvxag.html

[Q72] 查看索引
来源：http://hz.wangdashe.top/gthmiljmil.html

SHOW INDEX FROM users;
来源：http://hz.hysaishi.cn/gtzafaouun.html

[Q73] 查看表状态
来源：http://hz.quarkkingdee.top/gtmycchfno.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuxming.cn/gttjjifzlt.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gthhjhslye.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tian-w.cn/gtauqqfqew.html

[Q75] 日期格式化
来源：http://hz.xuetiantiany.cn/gtqdqbyomd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtkfwcrvcc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhixingplan.top/gtwilwwdsv.html

[Q76] 按天统计
来源：http://hz.mhx1999.top/gtzaxfphuy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.havefunace.top/gtsvsqsvns.html

[Q77] 时间加减
来源：http://hz.hnxiangtu.top/gtluneylmj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangkeji.top/gtvdpgwmij.html

[Q78] 当前时间
来源：http://hz.tianlin.xyz/gtrjeupgcg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jyoumei.cn/gtcqobrnyr.html

[Q79] 字符串拼接
来源：http://hz.yongpay.top/gtzufgyxpj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj202588.top/gtxggvynpa.html

[Q80] 字符串截取
来源：http://hz.pycfn.com/gtenypvlsr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtmbltzhbv.html

[Q81] 字符串替换
来源：http://hz.meibo888.top/gtesoynjei.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shzxlz.cn/gtupdsqami.html

[Q82] 字符长度与字节长度
来源：http://hz.cdnleiting.top/gtaaqvebfv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.bjfxy.top/gtfcyfpemt.html

[Q83] 大小写转换
来源：http://hz.tianlin.xyz/gttdfrzaib.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daria6918.cn/gtxtfqridm.html

[Q84] 去除首尾空格
来源：http://hz.smart0.xyz/gtnrreelud.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtjyyabohz.html

[Q85] 数值取整
来源：http://hz.haohaochexian.top/gtudinyozj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gtzelzaybg.html

[Q86] 读取 JSON 字段
来源：http://hz.snrcjt.cn/gtkupddnrn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtuvoczfjp.html

[Q87] JSON 字段做条件
来源：http://hz.hysaishi.cn/gtwfbmzjpf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gttzbsuvjh.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtfhmtuocm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.0kj1m.cn/gtrjinpfts.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ivvv.top/gtwicoedlw.html

[Q89] 判断表是否存在
来源：http://hz.hysaishi.cn/gtdnxetihi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtlrlgqyab.html

[Q90] 生成序号列
来源：http://hz.tianlin.xyz/gtpehhrgfb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fengsongda.top/gtpezptibg.html

================================================================================
来源：http://hz.hywenlv.cn/gtdeynzfaw.html

R. Bash 专题
来源：http://hz.jyoumei.cn/gtqicolrxc.html

================================================================================
来源：http://hz.yonumen.top/gtdtkxalmw.html

[R01] shebang 与严格模式
来源：http://hz.gzhubu.top/gtvchhadgv.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtigepldri.html

set -euo pipefail
来源：http://hz.jinqigfzy.top/gttxjqpnyg.html

[R02] 变量赋值与使用
来源：http://hz.mhx1999.top/gtshxcfyhv.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtephpnyqg.html

[R03] 只读变量
来源：http://hz.zhengqikj.top/gtyucihwjj.html

readonly PI=3.14
来源：http://hz.sysykeji.top/gtthjnzdbo.html

[R04] 位置参数
来源：http://hz.yvedp.cn/gtwyrtqvqh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinqigfzy.top/gtyohbqtin.html

[R05] 参数默认值
来源：http://hz.ehwqpu.com/gtusazmbzx.html

name="${1:-default}"
来源：http://hz.9152youxi.cn/gtncyjnfuw.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtklgkpirv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zycfv.cn/gtdltsqbwu.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtkljyblln.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtrslnyyys.html

[R08] 数值比较
来源：http://hz.yj20258.top/gtgyowyjzz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.vqdsnc.cn/gtzdmhtfui.html

[R09] 字符串比较
来源：http://hz.xziqi.cn/gtxqfnqbtt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sweek.top/gtpfbowrdd.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtxuowadbo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtuzikqyxa.html

[R11] case 多分支
来源：http://hz.ppjwa.cn/gtvidklpib.html

case "$1" in
来源：http://hz.pengpengdd.cyou/gtvdtsnuji.html

start) echo "启动" ;;
来源：http://hz.cdnleiting.top/gtzvokjdia.html

stop)  echo "停止" ;;
来源：http://hz.bjfxy.top/gtmihweboc.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtoxdrikky.html

esac
来源：http://hz.kuanghao11.cn/gtenyngszr.html

[R12] for 遍历文件
来源：http://hz.316326.xyz/gtxadkkmky.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhengqikj.top/gtmzzgkass.html

[R13] for 计数循环
来源：http://hz.ppjwa.cn/gtjarhvrnr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hywenlv.cn/gtkzabhdlu.html

[R14] C 风格 for
来源：http://hz.jianghu66.top/gtqhldgxeq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnxiangtu.top/gteeduubgb.html

[R15] while 逐行读文件
来源：http://hz.sweek.top/gtiwqeuutd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ehwqpu.com/gtkmijpaom.html

[R16] until 等待条件
来源：http://hz.guowangkeji.top/gtonojhwyi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtspbzwims.html

[R17] 数组定义与取值
来源：http://hz.xuanzx.com/gtgrlhwrdp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.0kj1m.cn/gttulxnkrl.html

[R18] 遍历数组
来源：http://hz.jyoumei.cn/gtsykdzpqd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtgnjsbfdb.html

[R19] 数组长度
来源：http://hz.ppjwa.cn/gtxxmxoawl.html

echo "${#arr[@]}"
来源：http://hz.chenjidiqi.icu/gtegmgaxdi.html

[R20] 关联数组（字典）
来源：http://hz.xylfe.cn/gtzvlxqkqa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guowangkeji.top/gtcqtxdrgv.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtuvgqselh.html

echo "${#s}"
来源：http://hz.ydjk.org.cn/gtflqchwcr.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtpkqjbtai.html

echo "${s:0:5}"
来源：http://hz.zdqjudy.top/gtilwjmdkl.html

[R23] 字符串替换
来源：http://hz.zhengqikj.top/gtvjpipayi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.mhx1999.top/gthdabeooy.html

[R24] 大小写转换
来源：http://hz.sufxvd.cn/gtqpnavdec.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.redwolf501.top/gtciqxitkn.html

[R25] 去后缀 / 去前缀
来源：http://hz.zdqjudy.top/gtiyhuaszk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xziqi.cn/gtdceslwee.html

[R26] 命令替换
来源：http://hz.xylfe.cn/gtxltzyhne.html

now=$(date +%F); echo "$now"
来源：http://hz.meibo888.top/gtpcgkdbkj.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtyewfhppf.html

echo $((1 + 2 * 3))
来源：http://hz.bjfxy.top/gtknuajkrm.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gtgfwxkwja.html

echo "scale=2; 10/3" | bc
来源：http://hz.cdnleiting.top/gtjmajhrjh.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gtfzwbxwik.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtmybozutj.html

[R30] 函数返回状态码
来源：http://hz.havefunace.top/gtxlxoevfa.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yanxiufei.cn/gtdccpkzhb.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtyaffvnnj.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtvtmwdxlh.html

[R32] 参数个数校验
来源：http://hz.9152youxi.cn/gtauyuffjj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.quarkkingdee.top/gtjzbenbvo.html

[R33] 捕获错误并提示行号
来源：http://hz.wangshuangyany.cn/gtegjityao.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.guannengcc.top/gtbkwnprax.html

[R34] 退出时清理
来源：http://hz.iojbl.cn/gtbghdnrxf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtfeszxafu.html

[R35] 后台执行并等待
来源：http://hz.ydjk.org.cn/gtwhdvitbo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cucudq.cn/gtcsornyke.html

[R36] 并发执行多个任务
来源：http://hz.cashguo.top/gturueersy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hywenlv.cn/gtsaawyyjg.html

[R37] 把输出赋给变量
来源：http://hz.havefunace.top/gtflfpjfvs.html

files=$(ls -1)
来源：http://hz.shangyingyoupin.top/gtnvzxarku.html

[R38] 管道串联
来源：http://hz.xingfuxueyuan.xyz/gtpwapgdxe.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cdnleiting.top/gtzzkotofq.html

[R39] 重定向标准输出与错误
来源：http://hz.hywenlv.cn/gtpliwmits.html

cmd > out.log 2>&1
来源：http://hz.hnxiangtu.top/gtuzbkahnr.html

[R40] 追加写日志
来源：http://hz.andypj.xyz/gtuubhildx.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtjioyqart.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gttcnwuvyz.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigfzy.top/gtoqppwynb.html

[R42] 输入重定向
来源：http://hz.tian-w.cn/gtaxjytksi.html

wc -l < a.txt
来源：http://hz.ivvv.top/gtgtdtglgl.html

[R43] 按名字查找文件
来源：http://hz.0kj1m.cn/gtybsnazdx.html

find . -name "*.log" -type f
来源：http://hz.nanxuanxn.top/gtzvnzdwgn.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtqtxqyuop.html

find . -mtime -7 -type f
来源：http://hz.dianchejie.cn/gtjxyygeaf.html

[R45] 批量删除
来源：http://hz.jlsjyb.cn/gtulivaquw.html

find . -name "*.tmp" -delete
来源：http://hz.wangdashe.top/gtqvoalioh.html

[R46] 递归替换文件内容
来源：http://hz.xuanzx.com/gtqsnzpkzr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gttynpqxks.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtclfambve.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gogol.net.cn/gtzgqyjllj.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtigyhvaba.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258.top/gtjxltsxlc.html

[R49] awk 带条件
来源：http://hz.52xcode.cn/gtytgyzvtv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtrbabsoii.html

[R50] awk 求和
来源：http://hz.cdnleiting.top/gttbsipmfd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sxryk.cn/gtvymswoyc.html

[R51] 排序去重取前几
来源：http://hz.sufxvd.cn/gthyxgzmtd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jiagoushi.top/gtjvfhgbzw.html

[R52] 统计行数
来源：http://hz.zhixingplan.top/gtqyzrudqk.html

wc -l a.txt
来源：http://hz.ydzc1.top/gttugfbfcv.html

[R53] 查看文件头与实时尾
来源：http://hz.fzhhl.top/gtwrtloekg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yongpay.top/gtpgbxxwog.html

[R54] 比较两个文件
来源：http://hz.0kj1m.cn/gtromnklou.html

diff a.txt b.txt
来源：http://hz.feifeiyinyue.top/gtqbqocztn.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtrbaefihz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yongpay.top/gtsxhryzog.html

[R56] 远程拷贝
来源：http://hz.yanxiufei.cn/gtvjbdlroj.html

scp file user@host:/path/
来源：http://hz.xinyue.icu/gtwnyluvqz.html

[R57] 远程执行命令
来源：http://hz.yvedp.cn/gtzidbrjtn.html

ssh user@host 'uptime'
来源：http://hz.hfpthk.cn/gtgynyhgms.html

[R58] 下载文件
来源：http://hz.jinghuilouyu.cn/gtjxppobwu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtslmbxjqv.html

[R59] 发 POST JSON
来源：http://hz.nanxinkj.top/gthaznmesv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cdnleiting.top/gtznpjyyun.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258888.top/gtykginpac.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sxryk.cn/gtzcjrwoya.html

[R61] 磁盘占用
来源：http://hz.havefunace.top/gtcuwugtqj.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtbyevaxcx.html

[R62] 找最占空间的文件
来源：http://hz.daria6918.cn/gtlashnwhx.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtnrsbkjmu.html

[R63] 内存与进程
来源：http://hz.c1oappe.top/gtzjfxwdje.html

free -h;  ps aux | grep nginx
来源：http://hz.jyoumei.cn/gtmlndkuvp.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gthqtiyyqd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtahrpgfii.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtxzfruepv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.316326.xyz/gtzullkjqy.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtidyhhele.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtfweaeniq.html

[R67] 生成随机十六进制串
来源：http://hz.hywenlv.cn/gtcpsiouph.html


<!-- 参考信息 -->