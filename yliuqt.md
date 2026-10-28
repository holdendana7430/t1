代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.guannengcc.top/gtybbonqse.html

[Q24] 去重
来源：http://hz.wangdashe.top/gtvulyttys.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuanzhike.top/gtiakghcbx.html

[Q25] 只取前 N 条
来源：http://hz.zhiwuduotai.top/gthcfjedvm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yonumen.top/gtwcatknmp.html

[Q26] 计数
来源：http://hz.hongshengwenyu.top/gtcuyhuuzt.html

SELECT COUNT(*) FROM users;
来源：http://hz.pengpengdd.cyou/gtddlybrmo.html

[Q27] 条件计数
来源：http://hz.zhengqikj.top/gtyapxtyss.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yvedp.cn/gtzcshmgrr.html

[Q28] 求和与平均
来源：http://hz.yueranfly.top/gtplbuxsyr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xinyue.icu/gtgiinibjw.html

[Q29] 最大最小值
来源：http://hz.ydjk.org.cn/gtkltddend.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zycfv.cn/gtemrfucow.html

[Q30] 分组统计
来源：http://hz.yueranfly.top/gtnduopvgl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gteaxukvbq.html

[Q31] 分组后过滤
来源：http://hz.wangdashe.top/gtsvuyzpze.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yvedp.cn/gtjtxypkaq.html

[Q32] 分组拼接字符串
来源：http://hz.andypj.xyz/gtfazkvzsf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.hfpthk.cn/gtiyfnvkih.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ivvv.top/gtjvlbgesj.html

[Q33] 多列分组
来源：http://hz.iojbl.cn/gtulfltgdw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jyoumei.cn/gtcaxxxdnp.html

[Q34] 每组取第一条
来源：http://hz.hnxiangtu.top/gtvqaxmzry.html

SELECT * FROM (
来源：http://hz.xuanzx.com/gtqtriqxwv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.iojbl.cn/gtwnhnefyu.html

) t WHERE rn = 1;
来源：http://hz.vqdsnc.cn/gtgorgnsfj.html

[Q35] 内连接
来源：http://hz.pycfn.com/gtadjzlayu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuxming.cn/gtsvtyaeps.html

[Q36] 左连接
来源：http://hz.zhoulong.xyz/gteaomazmp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.c1oappe.top/gtxxpyciwj.html

[Q37] 右连接
来源：http://hz.guowangkeji.top/gtmntpbaxy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cqqwz.cn/gtdtwcsysv.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.wangdashe.top/gtjwswziew.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cqqwz.cn/gtwxhjqedd.html

[Q39] 自连接（查上下级）
来源：http://hz.hnqzz.top/gtpdqoovdf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gogol.net.cn/gtoecuipff.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.smart0.xyz/gtyikxbnso.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.aibaodan.cn/gtircfszpr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yonumen.top/gtpmzcehmh.html

[Q41] 多表连接
来源：http://hz.9152youxi.cn/gtlipjntwp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.tian-w.cn/gtpbknoeii.html

JOIN users u ON u.id = o.user_id
来源：http://hz.daxiang520.top/gtjylwamrj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnxiangtu.top/gtmntsmjvk.html

[Q42] 连接条件附加过滤
来源：http://hz.chenlongwang.top/gtnkypxwrt.html

SELECT u.name, o.amount FROM users u
来源：http://hz.meibo888.top/gtbcxyaykz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.gaohongyu789.top/gtzfmsfppj.html

[Q43] 标量子查询
来源：http://hz.fengsongda.top/gtidlywswr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.guannengcc.top/gtzylohyfa.html

[Q44] IN 子查询
来源：http://hz.jinqigfzy.top/gtbwpiixdb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.fzhhl.top/gtrizcgtqk.html

[Q45] EXISTS 判断存在
来源：http://hz.zhengqikj.top/gtcpnzucic.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtsukpyovs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.wangshuangyany.cn/gtmyqyohcx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hysaishi.cn/gtycqjeodv.html

[Q47] 与平均值比较
来源：http://hz.cashguo.top/gtephddvhg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.fengsongda.top/gtsgfomagc.html

[Q48] CTE 公用表表达式
来源：http://hz.jianghu66.top/gtflhcnzdc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.smart0.xyz/gtmwfwhkfn.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.haohaochexian.top/gtcsfksutj.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtinjgkmdq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtpmfulmab.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtejwdhubk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtnoukpvdy.html

[Q51] 用子查询更新
来源：http://hz.0kj1m.cn/gtsigzbsfa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.havefunace.top/gtbfyranxf.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtwazmxuls.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtgrlotnrj.html

[Q53] 按条件删除
来源：http://hz.hysaishi.cn/gtoqgsjgzi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hongshengwenyu.top/gtsfelihgc.html

[Q54] 清空表
来源：http://hz.hysaishi.cn/gtcmajkaqk.html

TRUNCATE TABLE logs;
来源：http://hz.c1oappe.top/gttuslncqk.html

[Q55] 排名（并列占位）
来源：http://hz.zhongyouzk.top/gtvbctjpwe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ppjwa.cn/gtecongyha.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtonharkud.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yj20258.top/gtciqsactv.html

[Q57] 行号
来源：http://hz.aibaodan.cn/gtifnkkwni.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.dianchejie.cn/gtkwrbkyaw.html

[Q58] 累计求和
来源：http://hz.xuanzx.com/gtsltuomuc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shangyingyoupin.top/gtsgaxnsnt.html

[Q59] 分组内累计
来源：http://hz.yongpay.top/gtwaziuyiu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhijiandao.cn/gtcbwkggtw.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinyuanbaomall.cn/gtjqdggggl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hongshengwenyu.top/gtodbqxvxv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangshuangyany.cn/gtulhvzvdh.html

[Q61] 移动平均
来源：http://hz.nanxuanxn.top/gtosekorwx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zycfv.cn/gtdhfyptpx.html

[Q62] 分组占比
来源：http://hz.hnqzz.top/gtpehaxhcz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.gotoacloud.top/gtyqncplyu.html

[Q63] 开启事务
来源：http://hz.cheryme.top/gtfkwalrxz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuanzhike.top/gtrzsomukn.html

[Q64] 提交事务
来源：http://hz.shzxlz.cn/gtjtebdooc.html

COMMIT;
来源：http://hz.gzhubu.top/gtivtebuek.html

[Q65] 回滚事务
来源：http://hz.zhaomingkeji.xyz/gtqfxztcvv.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtyvnscoav.html

[Q66] 行锁查询
来源：http://hz.sxryk.cn/gtwmhtiaes.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tian-w.cn/gtqhzkavvk.html

[Q67] 设置隔离级别
来源：http://hz.ydjk.org.cn/gtsryrsvas.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.andypj.xyz/gtnfngqlli.html

[Q68] 保存点
来源：http://hz.tian-w.cn/gtuxdvfdvg.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtyqynieiu.html

ROLLBACK TO sp1;
来源：http://hz.daxiang520.top/gtalbczkwe.html

[Q69] 查看执行计划
来源：http://hz.havefunace.top/gtpzdpfafg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xingfuxueyuan.xyz/gtxsxtkamh.html

[Q70] 更新统计信息
来源：http://hz.hfpthk.cn/gtkersnbed.html

ANALYZE TABLE users;
来源：http://hz.wangdashe.top/gtxdqjldjf.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gtvjhmwdlq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xingfuxueyuan.xyz/gtqvwcrexr.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtlptibbeq.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gtzsbtacjf.html

[Q73] 查看表状态
来源：http://hz.mhx1999.top/gtcpqeulvc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xuetiantiany.cn/gteegnjgic.html

[Q74] 强制使用索引
来源：http://hz.andypj.xyz/gtpvcdugkj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jiagoushi.top/gtzdtingda.html

[Q75] 日期格式化
来源：http://hz.xziqi.cn/gtutbawwnp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenlongwang.top/gtbcyfnhej.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuanzhike.top/gtcdqxloem.html

[Q76] 按天统计
来源：http://hz.cdnleiting.top/gtatlposrf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.c1oappe.top/gtfogezwms.html

[Q77] 时间加减
来源：http://hz.dianchejie.cn/gtooheycdk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnqzz.top/gtehrlgxna.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtebmmpmrj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dianchejie.cn/gtibpghcon.html

[Q79] 字符串拼接
来源：http://hz.jinghuilouyu.cn/gtymntirpf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnqzz.top/gtellhbkyp.html

[Q80] 字符串截取
来源：http://hz.chenzaomai.com/gtclpcennt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daxiang520.top/gtmfxpgkaq.html

[Q81] 字符串替换
来源：http://hz.gotoacloud.top/gtcmqviqsb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yongpay.top/gtahmbhysb.html

[Q82] 字符长度与字节长度
来源：http://hz.zhaomingkeji.xyz/gtzucpvtcd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.andypj.xyz/gtblncvvad.html

[Q83] 大小写转换
来源：http://hz.cucudq.cn/gtvxtmtakp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhoulong.xyz/gtaomibett.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gtnwretzqm.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtewduwqug.html

[Q85] 数值取整
来源：http://hz.yonumen.top/gtlgstpswh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.wangdashe.top/gtrfwjkuxn.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtlgthugli.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yonumen.top/gtrtvwiaax.html

[Q87] JSON 字段做条件
来源：http://hz.yangfankeji.com/gtofsjrzuj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.aibaodan.cn/gtheoqaweb.html

[Q88] 行转列（条件聚合）
来源：http://hz.fengsongda.top/gtjnslsctq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gtycmqyhoc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxuanxn.top/gtwbaskbsj.html

[Q89] 判断表是否存在
来源：http://hz.feifeiyinyue.top/gtoiloicur.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtqezwhfel.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtytfqtqao.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daxiang520.top/gtrxqtyghr.html

================================================================================
来源：http://hz.hammf.cn/gtzhsycztm.html

R. Bash 专题
来源：http://hz.bjfxy.top/gtgdopmodz.html

================================================================================
来源：http://hz.316326.xyz/gtzzymaalv.html

[R01] shebang 与严格模式
来源：http://hz.sweek.top/gtxdtkhfsm.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gthgnsbabc.html

set -euo pipefail
来源：http://hz.yanxiufei.cn/gtkffpnzkz.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtokjjmtsw.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gtgqmnhihr.html

[R03] 只读变量
来源：http://hz.guannengcc.top/gtskcaqxrb.html

readonly PI=3.14
来源：http://hz.pengpengdd.cyou/gtfslnivts.html

[R04] 位置参数
来源：http://hz.havefunace.top/gtnkkygtqk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gtalyesndd.html

[R05] 参数默认值
来源：http://hz.jyoumei.cn/gtwesesstb.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtprbbkyaw.html

[R06] 判断命令是否存在
来源：http://hz.quarkkingdee.top/gtrepiepmv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gtzfgigysv.html

[R07] if 判断文件
来源：http://hz.yanxiufei.cn/gtqdamnzdp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.svipenyu.cn/gtwerehmcz.html

[R08] 数值比较
来源：http://hz.ppjwa.cn/gtpsvxsyrq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenlongwang.top/gtiprbfrkv.html

[R09] 字符串比较
来源：http://hz.hongshengwenyu.top/gttfgehflv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ehwqpu.com/gtzuyyifwe.html

[R10] 正则匹配
来源：http://hz.zycfv.cn/gtmwtrhuhd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ivvv.top/gtfxsuwvis.html

[R11] case 多分支
来源：http://hz.0kj1m.cn/gtjcmrhfjv.html

case "$1" in
来源：http://hz.daxiang520.top/gtevmdsmqt.html

start) echo "启动" ;;
来源：http://hz.0kj1m.cn/gtnailsadi.html

stop)  echo "停止" ;;
来源：http://hz.jinyuanbaomall.cn/gtwsxavekr.html

*)     echo "未知命令" ;;
来源：http://hz.havefunace.top/gtqajxhuhy.html

esac
来源：http://hz.wangshuangyany.cn/gtogkvosou.html

[R12] for 遍历文件
来源：http://hz.ivvv.top/gtecgzoubl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zdqjudy.top/gttceigjgj.html

[R13] for 计数循环
来源：http://hz.jinghuilouyu.cn/gtbjasyiqv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtljeqbcao.html

[R14] C 风格 for
来源：http://hz.havefunace.top/gtnukrqupx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtusgobmmq.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtxbnplifk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cdnleiting.top/gtixlzbfec.html

[R16] until 等待条件
来源：http://hz.nanxuanxn.top/gtbelaghza.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj20258.top/gtraqgejci.html

[R17] 数组定义与取值
来源：http://hz.guowangkeji.top/gtrebghxzk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.dianchejie.cn/gtbocxqofp.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtidtebgiw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.316326.xyz/gthowktlzo.html

[R19] 数组长度
来源：http://hz.xziqi.cn/gtzgqcicjc.html

echo "${#arr[@]}"
来源：http://hz.daxiang520.top/gtiyrvqrnt.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtoiqsfbhk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jianghu66.top/gtqtxdxmvb.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtgechhbix.html

echo "${#s}"
来源：http://hz.zhiwuduotai.top/gtslhysgje.html

[R22] 截取子串
来源：http://hz.yj20258.top/gtqadeomro.html

echo "${s:0:5}"
来源：http://hz.kuanghao11.cn/gtsvxdiyha.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtvlqotbuj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gotoacloud.top/gtrekcvoxd.html

[R24] 大小写转换
来源：http://hz.cdnleiting.top/gtikpsaaco.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sweek.top/gtkmrbotwp.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtbauaismi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.vqdsnc.cn/gttqgjbwbt.html

[R26] 命令替换
来源：http://hz.daria6918.cn/gteusgaetk.html

now=$(date +%F); echo "$now"
来源：http://hz.guannengcc.top/gtuvizawnz.html

[R27] 算术展开
来源：http://hz.gzhubu.top/gtrtiwkyhz.html

echo $((1 + 2 * 3))
来源：http://hz.guowangkeji.top/gtgpfyywjn.html

[R28] 浮点运算
来源：http://hz.fengsongda.top/gtqggyybkm.html

echo "scale=2; 10/3" | bc
来源：http://hz.xinyue.icu/gtkvdrdzuo.html

[R29] 定义函数
来源：http://hz.ydzc1.top/gtarikplkg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hfpthk.cn/gttnhciupm.html

[R30] 函数返回状态码
来源：http://hz.quarkkingdee.top/gtzfmmiobp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.meibo888.top/gticjfttoe.html

[R31] 局部变量
来源：http://hz.quarkkingdee.top/gtsmrkhzzm.html

f() { local x=1; echo "$x"; }
来源：http://hz.havefunace.top/gtlpuioypn.html

[R32] 参数个数校验
来源：http://hz.yangfankeji.com/gtpqsrpitp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtlnlcroxw.html

[R33] 捕获错误并提示行号
来源：http://hz.ybcxt.top/gtoktpsopk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuetiantiany.cn/gtwlwnxpmf.html

[R34] 退出时清理
来源：http://hz.iojbl.cn/gtdnzgnsww.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtyemkvhmi.html

[R35] 后台执行并等待
来源：http://hz.kuanghao11.cn/gtbdpglgoh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gotoacloud.top/gtvesqpchm.html

[R36] 并发执行多个任务
来源：http://hz.sysykeji.top/gtopmslucz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuanzx.com/gtpugfnjcg.html

[R37] 把输出赋给变量
来源：http://hz.hywenlv.cn/gtuzfwenhf.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtppohdzwh.html

[R38] 管道串联
来源：http://hz.yuanzhike.top/gtfdawwtus.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gaohongyu789.top/gtxmbstmpq.html

[R39] 重定向标准输出与错误
来源：http://hz.ivvv.top/gtjhxefsou.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gtvgnbkhnc.html

[R40] 追加写日志
来源：http://hz.zhongyouzk.top/gtrgmdwred.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtbznaphnx.html

[R41] 丢弃输出
来源：http://hz.snrcjt.cn/gtreaozkai.html

cmd >/dev/null 2>&1
来源：http://hz.xuanzx.com/gthsmkbbpz.html

[R42] 输入重定向
来源：http://hz.nanxuanxn.top/gtlweyruvp.html

wc -l < a.txt
来源：http://hz.zhijiandao.cn/gtjqvxmhcm.html

[R43] 按名字查找文件
来源：http://hz.zhoulong.xyz/gtkegrnkpz.html

find . -name "*.log" -type f
来源：http://hz.zdqjudy.top/gtpztvewty.html

[R44] 按修改时间查找
来源：http://hz.wangshuangyany.cn/gtcysfmjhu.html

find . -mtime -7 -type f
来源：http://hz.xziqi.cn/gtaiuewtuo.html

[R45] 批量删除
来源：http://hz.dianchejie.cn/gtnlxcbaql.html

find . -name "*.tmp" -delete
来源：http://hz.ybcxt.top/gtuwajztmf.html

[R46] 递归替换文件内容
来源：http://hz.52xcode.cn/gtqflvslmg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.wangdashe.top/gtdiyezcgg.html

[R47] sed 单行替换
来源：http://hz.jqgfzy.top/gtmymybdmn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtejbvuama.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtoaxlxqtm.html

awk '{print $1, $3}' a.txt
来源：http://hz.zycfv.cn/gtsjjzylhi.html

[R49] awk 带条件
来源：http://hz.xingfuxueyuan.xyz/gtntkqbirl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhoulong.xyz/gtewotadhq.html

[R50] awk 求和
来源：http://hz.c1oappe.top/gtlrjoujuh.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hywenlv.cn/gtpcwhfdcg.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtmcwmgdpq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ehwqpu.com/gthrcwdbrc.html

[R52] 统计行数
来源：http://hz.nanxinkj.top/gtjoibiaib.html

wc -l a.txt
来源：http://hz.svipenyu.cn/gtlwynylhq.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtkdrtbfor.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shzxlz.cn/gtukmeyspx.html

[R54] 比较两个文件
来源：http://hz.bjfxy.top/gtlqdajiib.html

diff a.txt b.txt
来源：http://hz.pengpengdd.cyou/gtwoogoalj.html

[R55] 压缩与解压
来源：http://hz.ywan-chungtsiang.top/gtppsjgxis.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.fengsongda.top/gtjdglclhc.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtwehllqpi.html

scp file user@host:/path/
来源：http://hz.quarkkingdee.top/gtkoigoyef.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtsqkdvrmb.html

ssh user@host 'uptime'
来源：http://hz.gzhubu.top/gtromdprzs.html

[R58] 下载文件
来源：http://hz.ydjk.org.cn/gtvkqzurdd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nwbrower.top/gtvozwxrlc.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtpbvjqbne.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenlongwang.top/gtlmfkztar.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtawulvowg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xylfe.cn/gtsfitytkn.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtjfyylihw.html

df -h;  du -sh *
来源：http://hz.shanyushiyangkeji.top/gtqyzvltli.html

[R62] 找最占空间的文件
来源：http://hz.jinqigufen.top/gtaomswtsl.html

du -ah . | sort -rh | head -10
来源：http://hz.sweek.top/gtopjutgpd.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtsuynbofc.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gttmmzkkql.html

[R64] 结束进程
来源：http://hz.sysykeji.top/gtyznczdii.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenlongwang.top/gtjbftuxhl.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gtszbaxmdw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.0kj1m.cn/gtymxthmqj.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtkrpvzkpl.html

crontab -e;  crontab -l
来源：http://hz.gzhubu.top/gtojopwbge.html

[R67] 生成随机十六进制串
来源：http://hz.dianchejie.cn/gtauoijsss.html

openssl rand -hex 16
来源：http://hz.mhx1999.top/gtuwtuihru.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gtgqzvuycb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtgbqlzyir.html

[R69] 生成随机密码
来源：http://hz.jiagoushi.top/gtundkxkee.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gtxcrvkbui.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtgqejnpmq.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtjyfqyzxe.html

[R71] 日期格式化
来源：http://hz.chenzaomai.com/gtkazctgpo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cashguo.top/gtxmjfgyub.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtbkbuhmvx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daria6918.cn/gtcdoiqrls.html

[R73] 分割大日志
来源：http://hz.jlsjyb.cn/gtgssnwsss.html


<!-- 参考信息 -->