代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.52xcode.cn/gtteywaerr.html

[Q20] IN 列表
来源：http://hz.sufxvd.cn/gtjasnspiy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.yonumen.top/gtfykogwpv.html

[Q21] 空值判断
来源：http://hz.xingfuxueyuan.xyz/gtwxxatpbw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yanxiufei.cn/gtgzmmvjbz.html

[Q22] 排序
来源：http://hz.cdnleiting.top/gtlipsnvek.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.hammf.cn/gtigksdfbm.html

[Q23] 分页
来源：http://hz.gotoacloud.top/gthpgfaywx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhaomingkeji.xyz/gtekqriaat.html

[Q24] 去重
来源：http://hz.nanxuanxn.top/gtdxsipzlf.html

SELECT DISTINCT city FROM users;
来源：http://hz.daria6918.cn/gtoteowedk.html

[Q25] 只取前 N 条
来源：http://hz.316326.xyz/gtpdgtnmdy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.fengsongda.top/gtophdmidb.html

[Q26] 计数
来源：http://hz.pengpengdd.cyou/gtkssksvsr.html

SELECT COUNT(*) FROM users;
来源：http://hz.hfpthk.cn/gtkjzopyao.html

[Q27] 条件计数
来源：http://hz.shzxlz.cn/gtaxafvabi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangkeji.top/gtlnxegwjd.html

[Q28] 求和与平均
来源：http://hz.yanxiufei.cn/gtdyxkectu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtmzcmsuaf.html

[Q29] 最大最小值
来源：http://hz.shanyushiyangtech.top/gtszsfbwqr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.quarkkingdee.top/gttikicumi.html

[Q30] 分组统计
来源：http://hz.shanyushiyangtech.top/gtlyrpyblp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtbmigznun.html

[Q31] 分组后过滤
来源：http://hz.vqdsnc.cn/gtryavxanc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.quarkkingdee.top/gtmifbpzbk.html

[Q32] 分组拼接字符串
来源：http://hz.sufxvd.cn/gtbypcqijz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.shangyingyoupin.top/gtsyzbqyin.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shanyushiyangkeji.top/gtlzpoyzny.html

[Q33] 多列分组
来源：http://hz.hongshengwenyu.top/gteffiridy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shangyingyoupin.top/gtatozzgoe.html

[Q34] 每组取第一条
来源：http://hz.9152youxi.cn/gteyvmwwlh.html

SELECT * FROM (
来源：http://hz.yonumen.top/gtzempgund.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jinyuanbaomall.cn/gtjyvsjvvt.html

) t WHERE rn = 1;
来源：http://hz.shanyushiyangkeji.top/gtzzazgaee.html

[Q35] 内连接
来源：http://hz.9152youxi.cn/gtsthyzfte.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtnemzffel.html

[Q36] 左连接
来源：http://hz.9152youxi.cn/gtgvflmeka.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yj20258.top/gtkwpimttw.html

[Q37] 右连接
来源：http://hz.aizwys.cn/gtrowpsrdw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.wangshuangyany.cn/gtjqlqxcrb.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cucudq.cn/gtsrkwjcmg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.iojbl.cn/gtxqexwxmy.html

[Q39] 自连接（查上下级）
来源：http://hz.zhoulong.xyz/gtyvvnqbpo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.guowangkeji.top/gtiqgwwzuq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.cucudq.cn/gtltkfbsdk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nwbrower.top/gtbtalxfso.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shuidangran.top/gtcmfarswd.html

[Q41] 多表连接
来源：http://hz.ydzc1.top/gtvfzeyuhg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.nanxuanxn.top/gtybuekciw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.0kj1m.cn/gtrrxdgivv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shanyushiyangkeji.top/gtozqpwkjj.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxuanxn.top/gtcnggrndw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hammf.cn/gttexkaqgp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hnqzz.top/gtrkgxtufs.html

[Q43] 标量子查询
来源：http://hz.hammf.cn/gtjsrhvktp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xziqi.cn/gtdmkgedgw.html

[Q44] IN 子查询
来源：http://hz.ybcxt.top/gtpbxkvrjs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhoulong.xyz/gtfuvtrzdp.html

[Q45] EXISTS 判断存在
来源：http://hz.yuanzhike.top/gtczvamlva.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.guannengcc.top/gtzjztajgy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yueranfly.top/gtcghvnemy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.0kj1m.cn/gtzmmstusi.html

[Q47] 与平均值比较
来源：http://hz.xingfuxueyuan.xyz/gtbpyuyegc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ywan-chungtsiang.top/gtotatqefy.html

[Q48] CTE 公用表表达式
来源：http://hz.dashuyun.cn/gtdxlvngaq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hysaishi.cn/gtuhbdlfgr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daria6918.cn/gtvjwkorvt.html

[Q49] 更新单行
来源：http://hz.ivvv.top/gthptloeta.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cqqwz.cn/gtlkdxsfrp.html

[Q50] 批量更新
来源：http://hz.pengpengdd.cyou/gtpfvohqxk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.52xcode.cn/gtlwuspdwb.html

[Q51] 用子查询更新
来源：http://hz.haohaochexian.top/gtnnfweguv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtwqukzydv.html

[Q52] 删除指定行
来源：http://hz.zdqjudy.top/gtbtgrctyw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.wangdashe.top/gtgtoxdsde.html

[Q53] 按条件删除
来源：http://hz.xziqi.cn/gtsgbbpkpt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhaomingkeji.xyz/gtftomdptj.html

[Q54] 清空表
来源：http://hz.iojbl.cn/gttokeyooo.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gteljnqbsn.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gtwseusuwy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tanke756.top/gtcyhpditk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.guowangkeji.top/gtwgwmbylx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.chenlongwang.top/gtgbfbeebf.html

[Q57] 行号
来源：http://hz.wangdashe.top/gtcryjzwsb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.feifeiyinyue.top/gtnoycghhi.html

[Q58] 累计求和
来源：http://hz.daria6918.cn/gtaoufsakn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gtbzvcqvpa.html

[Q59] 分组内累计
来源：http://hz.jianghu66.top/gtqqugzyfh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yanxiufei.cn/gtpabdlghb.html

[Q60] 取上一行 / 下一行
来源：http://hz.52xcode.cn/gtubcrckqb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jlsjyb.cn/gtselsrxkx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fengsongda.top/gtpdzrczop.html

[Q61] 移动平均
来源：http://hz.shzxlz.cn/gtorsktsxl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sysykeji.top/gtkuqovlmc.html

[Q62] 分组占比
来源：http://hz.9152youxi.cn/gttxhcrekh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj20258.top/gtvymkhmyc.html

[Q63] 开启事务
来源：http://hz.hongshengwenyu.top/gtkotsehqz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxinkj.top/gtfaqzencx.html

[Q64] 提交事务
来源：http://hz.ydjk.org.cn/gtqizcjtsd.html

COMMIT;
来源：http://hz.ppjwa.cn/gtrbcnveiv.html

[Q65] 回滚事务
来源：http://hz.yongpay.top/gtldrxgjpf.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtthjwysrr.html

[Q66] 行锁查询
来源：http://hz.daxiang520.top/gtdjnftmfq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zycfv.cn/gtktepbpwl.html

[Q67] 设置隔离级别
来源：http://hz.hysaishi.cn/gtmrehymmm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.hongshengwenyu.top/gtpdihpasl.html

[Q68] 保存点
来源：http://hz.svipenyu.cn/gtqfbdznxe.html

SAVEPOINT sp1;
来源：http://hz.dianchejie.cn/gtthhkwgtl.html

ROLLBACK TO sp1;
来源：http://hz.guowangkeji.top/gtfdasgfzg.html

[Q69] 查看执行计划
来源：http://hz.yuanzhike.top/gtcviuqwqc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtnjbllcpd.html

[Q70] 更新统计信息
来源：http://hz.pycfn.com/gtjeklekag.html

ANALYZE TABLE users;
来源：http://hz.nanxuanxn.top/gtemwetsjn.html

[Q71] 查看建表语句
来源：http://hz.jiagoushi.top/gteqaeppoz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hfpthk.cn/gtvoenbrsj.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gtfeiudsbb.html

SHOW INDEX FROM users;
来源：http://hz.zhongyouzk.top/gtuuecrten.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gtjyrzrexk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.andypj.xyz/gtawflwfjg.html

[Q74] 强制使用索引
来源：http://hz.shangyingyoupin.top/gtdkduzuce.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jianghu66.top/gtsivgorhz.html

[Q75] 日期格式化
来源：http://hz.zhongyouzk.top/gtunqtnrmf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ybcxt.top/gtediinuax.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.daxiang520.top/gtzoxobpuz.html

[Q76] 按天统计
来源：http://hz.feifeiyinyue.top/gtrvjpwoqm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yonumen.top/gtqyyfxcpq.html

[Q77] 时间加减
来源：http://hz.zdqjudy.top/gtbovtrwud.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shzxlz.cn/gtbfneyxde.html

[Q78] 当前时间
来源：http://hz.chenlongwang.top/gtkejiyfrt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.bjfxy.top/gtcpbslwwz.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtqurqwkat.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.snrcjt.cn/gtugqwhxry.html

[Q80] 字符串截取
来源：http://hz.ehwqpu.com/gtrrdryloc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtasumbapp.html

[Q81] 字符串替换
来源：http://hz.cdnleiting.top/gtfwuuzwma.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dashuyun.cn/gtjlzkdpdg.html

[Q82] 字符长度与字节长度
来源：http://hz.zhengqikj.top/gtusaiozdq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yueranfly.top/gtsepbqxju.html

[Q83] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtddojplmx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yangfankeji.com/gtqpmfeemw.html

[Q84] 去除首尾空格
来源：http://hz.kuanghao11.cn/gtmwmzyzum.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtdchukyjj.html

[Q85] 数值取整
来源：http://hz.tian-w.cn/gtkjyajfoo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cqqwz.cn/gtobwzmycl.html

[Q86] 读取 JSON 字段
来源：http://hz.9152youxi.cn/gtojnynqhx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yueranfly.top/gtoiqxhggk.html

[Q87] JSON 字段做条件
来源：http://hz.andypj.xyz/gtguwoowtr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gtpfhftdow.html

[Q88] 行转列（条件聚合）
来源：http://hz.svipenyu.cn/gtkumzjelr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtkwkdiujr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.redwolf501.top/gtodzcgeqb.html

[Q89] 判断表是否存在
来源：http://hz.yueranfly.top/gttualhanx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtmlwzhmud.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtqpuwsjgb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtzhdqgfcp.html

================================================================================
来源：http://hz.c1oappe.top/gtdogqmlcz.html

R. Bash 专题
来源：http://hz.yonumen.top/gttymwvbtj.html

================================================================================
来源：http://hz.cucudq.cn/gtkrttxgfs.html

[R01] shebang 与严格模式
来源：http://hz.ydzc1.top/gtrgojlaka.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtbbxchdjt.html

set -euo pipefail
来源：http://hz.haohaochexian.top/gtcroivkim.html

[R02] 变量赋值与使用
来源：http://hz.cheryme.top/gtfjqmdkaj.html

name="Tom"; echo "$name"
来源：http://hz.tian-w.cn/gtcllfkbxz.html

[R03] 只读变量
来源：http://hz.shzxlz.cn/gtgflzoqna.html

readonly PI=3.14
来源：http://hz.sufxvd.cn/gtqezjmrwz.html

[R04] 位置参数
来源：http://hz.zhixingplan.top/gtmxwdbrnz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhongyouzk.top/gtmywovimj.html

[R05] 参数默认值
来源：http://hz.yonumen.top/gtrpnqivwp.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtqtydydqa.html

[R06] 判断命令是否存在
来源：http://hz.ivvv.top/gtqennnesd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtxaqmhagw.html

[R07] if 判断文件
来源：http://hz.jinqigfzy.top/gttwpsokda.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtvxviqgzo.html

[R08] 数值比较
来源：http://hz.sufxvd.cn/gtdxqrzzpl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yj20258.top/gtfxipnyqy.html

[R09] 字符串比较
来源：http://hz.dianchejie.cn/gtcradgmln.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sweek.top/gtrlpadjdt.html

[R10] 正则匹配
来源：http://hz.sysykeji.top/gtqlfowfat.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenlongwang.top/gtipakynsj.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtfvscxtro.html

case "$1" in
来源：http://hz.jlsjyb.cn/gtzirgjdql.html

start) echo "启动" ;;
来源：http://hz.ehwqpu.com/gtbpoivunq.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gthbemkgys.html

*)     echo "未知命令" ;;
来源：http://hz.chenzaomai.com/gtivcrejdn.html

esac
来源：http://hz.0kj1m.cn/gtgdmoanhn.html

[R12] for 遍历文件
来源：http://hz.gzhubu.top/gtjjwsapdu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.redwolf501.top/gtdkrmqbbs.html

[R13] for 计数循环
来源：http://hz.jqgfzy.top/gtxfgxnwef.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgufenzy.top/gtukolfxqu.html

[R14] C 风格 for
来源：http://hz.hammf.cn/gtsexlvucz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtvqmkiwfn.html

[R15] while 逐行读文件
来源：http://hz.jqgufenzy.top/gtphoyzuyw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhoulong.xyz/gtmtoczxbn.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtktadzxcx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yueranfly.top/gtogeotqgj.html

[R17] 数组定义与取值
来源：http://hz.zhaomingkeji.xyz/gtyhntilly.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ivvv.top/gtbvmxdpdd.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gtvcookbas.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sufxvd.cn/gtsnsqxlmz.html

[R19] 数组长度
来源：http://hz.9152youxi.cn/gtfnammiog.html

echo "${#arr[@]}"
来源：http://hz.zhiwuduotai.top/gtehbpfvcf.html

[R20] 关联数组（字典）
来源：http://hz.aizwys.cn/gtbajrjjls.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhaomingkeji.xyz/gtvwdawiry.html

[R21] 字符串长度
来源：http://hz.shuidangran.top/gtbqssvrjc.html

echo "${#s}"
来源：http://hz.kuanghao11.cn/gtejsxulxk.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtvpatysuq.html

echo "${s:0:5}"
来源：http://hz.xylfe.cn/gtbqvgmlge.html

[R23] 字符串替换
来源：http://hz.meibo888.top/gtdmbdilal.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jqgfzy.top/gtethykpzl.html

[R24] 大小写转换
来源：http://hz.gaohongyu789.top/gtgakpkbsv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yonumen.top/gtzekixeze.html

[R25] 去后缀 / 去前缀
来源：http://hz.jyoumei.cn/gtkcptryms.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.havefunace.top/gtocoekcff.html

[R26] 命令替换
来源：http://hz.hfpthk.cn/gtowlksfaw.html

now=$(date +%F); echo "$now"
来源：http://hz.xingfuxueyuan.xyz/gtpmktyhyu.html

[R27] 算术展开
来源：http://hz.yj20258888.top/gtpstfcxxw.html

echo $((1 + 2 * 3))
来源：http://hz.chenzaomai.com/gtcnxsvbpe.html

[R28] 浮点运算
来源：http://hz.yj20258.top/gtszuyymzf.html

echo "scale=2; 10/3" | bc
来源：http://hz.cqqwz.cn/gthbkxxhnl.html

[R29] 定义函数
来源：http://hz.dashuyun.cn/gtgvvfxgbf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.iojbl.cn/gtalgssxws.html

[R30] 函数返回状态码
来源：http://hz.chenjidiqi.icu/gtaqvaynow.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258.top/gtdyltwqsu.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gtlkmzycnq.html

f() { local x=1; echo "$x"; }
来源：http://hz.daxiang520.top/gtqrfeccms.html

[R32] 参数个数校验
来源：http://hz.wangshuangyany.cn/gtzsxcgsls.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.aizwys.cn/gtozjmqgfd.html

[R33] 捕获错误并提示行号
来源：http://hz.zdqjudy.top/gtmrovrmdr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.fzhhl.top/gtlvlcfeeg.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gtiyevytyu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gthmmbsshs.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtobbpfgng.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jianghu66.top/gtmffnpaun.html

[R36] 并发执行多个任务
来源：http://hz.ydjk.org.cn/gtcbdvvddl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.guannengcc.top/gtgrrbzbyk.html

[R37] 把输出赋给变量
来源：http://hz.meibo888.top/gtgaerwwud.html

files=$(ls -1)
来源：http://hz.yonumen.top/gtohzivkzp.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gtadvomxis.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yanxiufei.cn/gtkvsoksuv.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtmeqmaibv.html

cmd > out.log 2>&1
来源：http://hz.shangyingyoupin.top/gthwfujxfn.html

[R40] 追加写日志
来源：http://hz.0kj1m.cn/gtgnxbilig.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtmkmxcaax.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtvkzjhvqx.html

cmd >/dev/null 2>&1
来源：http://hz.yuanzhike.top/gttcalapeg.html

[R42] 输入重定向
来源：http://hz.bjfxy.top/gtgkdfrzml.html

wc -l < a.txt
来源：http://hz.cheryme.top/gtsjyjpepv.html

[R43] 按名字查找文件
来源：http://hz.xingfuxueyuan.xyz/gtqdndektu.html

find . -name "*.log" -type f
来源：http://hz.zhongyouzk.top/gthmtecflj.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtcfgteaao.html

find . -mtime -7 -type f
来源：http://hz.daria6918.cn/gtkxiscjwz.html

[R45] 批量删除
来源：http://hz.zhengqikj.top/gthgkkxitq.html

find . -name "*.tmp" -delete
来源：http://hz.sweek.top/gtqmmcxafg.html

[R46] 递归替换文件内容
来源：http://hz.tian-w.cn/gtnjokwxio.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenlongwang.top/gtvtrhhiba.html

[R47] sed 单行替换
来源：http://hz.havefunace.top/gtlnhpbuux.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydjk.org.cn/gtdzmfrkfo.html

[R48] awk 取指定列
来源：http://hz.gzhubu.top/gtozchyius.html

awk '{print $1, $3}' a.txt
来源：http://hz.vqdsnc.cn/gtnjnkyhwh.html

[R49] awk 带条件
来源：http://hz.kuanghao11.cn/gtwcugcghk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dashuyun.cn/gttzaphzyc.html

[R50] awk 求和
来源：http://hz.gaohongyu789.top/gtvpouzvns.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ivvv.top/gtxdsmrkhr.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtvqfakbmr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtbtwotplx.html

[R52] 统计行数
来源：http://hz.guowangkeji.top/gtcdgjhssl.html

wc -l a.txt
来源：http://hz.zhijiandao.cn/gtcjdkckzk.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtvzmbtxyi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.52xcode.cn/gtdybqwyuy.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtitizdsym.html

diff a.txt b.txt
来源：http://hz.zhaomingkeji.xyz/gtssrnrbdb.html

[R55] 压缩与解压
来源：http://hz.nwbrower.top/gtjrpjhwjy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jyoumei.cn/gtjlzmzmna.html

[R56] 远程拷贝
来源：http://hz.havefunace.top/gtodfrgcew.html

scp file user@host:/path/
来源：http://hz.shanyushiyangkeji.top/gtmtltdywm.html

[R57] 远程执行命令
来源：http://hz.jqgfzy.top/gtybgpbxlk.html

ssh user@host 'uptime'
来源：http://hz.yvedp.cn/gtuvtcyajo.html

[R58] 下载文件
来源：http://hz.daria6918.cn/gtxyzghohd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtgwslfpxk.html

[R59] 发 POST JSON
来源：http://hz.jqgfzy.top/gtlqvfytbe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhoulong.xyz/gtpabciauv.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtubkafajy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gtnvlmbniq.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangkeji.top/gtrbtvfmcw.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gthkgqccew.html

[R62] 找最占空间的文件
来源：http://hz.ybcxt.top/gtpnxwtykb.html

du -ah . | sort -rh | head -10
来源：http://hz.smart0.xyz/gthvmxubui.html

[R63] 内存与进程
来源：http://hz.zdqjudy.top/gtyvdkpcqh.html

free -h;  ps aux | grep nginx
来源：http://hz.xziqi.cn/gtfohjrmzo.html

[R64] 结束进程
来源：http://hz.jinghuilouyu.cn/gtpljbkool.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gteyzowmiz.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gtddjnzsmh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yvedp.cn/gtilgrpdbd.html

[R66] 定时任务
来源：http://hz.yonumen.top/gtfbwzyqkz.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gtmzlmyulx.html

[R67] 生成随机十六进制串
来源：http://hz.yvedp.cn/gthhxffpii.html

openssl rand -hex 16
来源：http://hz.xuanzx.com/gtqmpqnvyp.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangtech.top/gtxhqxvggq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.9152youxi.cn/gtdnuslqny.html

[R69] 生成随机密码
来源：http://hz.hammf.cn/gtgbixguse.html


<!-- 参考信息 -->