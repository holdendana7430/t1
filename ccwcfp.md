代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.nanxuanxn.top/gtovyqewqs.html

[Q24] 去重
来源：http://hz.ehwqpu.com/gtlausumkq.html

SELECT DISTINCT city FROM users;
来源：http://hz.tianlin.xyz/gtdmtcmzrc.html

[Q25] 只取前 N 条
来源：http://hz.hnqzz.top/gtapqibums.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xylfe.cn/gtvszabrzv.html

[Q26] 计数
来源：http://hz.cqqwz.cn/gtsqfofzvu.html

SELECT COUNT(*) FROM users;
来源：http://hz.0kj1m.cn/gtdhwfzvkl.html

[Q27] 条件计数
来源：http://hz.haohaochexian.top/gtuzttyoce.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gthyslkryn.html

[Q28] 求和与平均
来源：http://hz.shanyushiyangkeji.top/gtryihzzny.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xuetiantiany.cn/gtnouvwccy.html

[Q29] 最大最小值
来源：http://hz.nanxinkj.top/gtgkfrfepy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zhijiandao.cn/gtsnnpbnql.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtueiwhzqd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.jlsjyb.cn/gtvhjnhumi.html

[Q31] 分组后过滤
来源：http://hz.mhx1999.top/gtxqmeezxt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.guowangkeji.top/gtwdnrxxiy.html

[Q32] 分组拼接字符串
来源：http://hz.jiagoushi.top/gtmrmvlngi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenjidiqi.icu/gtiuhmfrqj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.kuanghao11.cn/gtypgcezsp.html

[Q33] 多列分组
来源：http://hz.yj20258888.top/gtyqnvrnru.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.c1oappe.top/gtqbfqvtnc.html

[Q34] 每组取第一条
来源：http://hz.yonumen.top/gtikyqpqgt.html

SELECT * FROM (
来源：http://hz.yuanzhike.top/gtfchirbgp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj20258.top/gtmekstpvc.html

) t WHERE rn = 1;
来源：http://hz.hnxiangtu.top/gthptowyrz.html

[Q35] 内连接
来源：http://hz.ivvv.top/gtogimfffw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtftidfcwi.html

[Q36] 左连接
来源：http://hz.aibaodan.cn/gtdhqwnfuv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenlongwang.top/gtasubqgcy.html

[Q37] 右连接
来源：http://hz.yuxming.cn/gtlrdgrjmn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dashuyun.cn/gttssomyqi.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.jianghu66.top/gtfleqddal.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.ydjk.org.cn/gtqtfgnzyp.html

[Q39] 自连接（查上下级）
来源：http://hz.gaohongyu789.top/gtumgsxczx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258.top/gtgufjecqw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhiwuduotai.top/gtzfmalmcd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.smart0.xyz/gtnrsjjmxj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.nanxuanxn.top/gtilzcjrgc.html

[Q41] 多表连接
来源：http://hz.shanyushiyangkeji.top/gtvqbvtbah.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yuxming.cn/gtarmdwzox.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cashguo.top/gtefimsfqj.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jyoumei.cn/gtspeerrnk.html

[Q42] 连接条件附加过滤
来源：http://hz.shzxlz.cn/gtdhtgykea.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yvedp.cn/gtatamcpof.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.bjfxy.top/gtamliabbo.html

[Q43] 标量子查询
来源：http://hz.nwbrower.top/gtexxeomwx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangdashe.top/gtoxwqmada.html

[Q44] IN 子查询
来源：http://hz.chenlongwang.top/gtuivqgrir.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigufen.top/gthxoqiwxg.html

[Q45] EXISTS 判断存在
来源：http://hz.mhx1999.top/gtbrgnprmd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gtzojsmksv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jyoumei.cn/gtkaiteluz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtytzugiqc.html

[Q47] 与平均值比较
来源：http://hz.smart0.xyz/gtkhxtyxyu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gotoacloud.top/gtjnuipnmr.html

[Q48] CTE 公用表表达式
来源：http://hz.hnxiangtu.top/gtxjjcnmtv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtsrrssoge.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.mhx1999.top/gtrqhwxkcp.html

[Q49] 更新单行
来源：http://hz.shanyushiyangtech.top/gtpajedouw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dianchejie.cn/gtedexadgm.html

[Q50] 批量更新
来源：http://hz.smart0.xyz/gtreimzugv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.wangshuangyany.cn/gtpitvtumq.html

[Q51] 用子查询更新
来源：http://hz.shangyingyoupin.top/gtynrwywiy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhongyouzk.top/gtzypmaosl.html

[Q52] 删除指定行
来源：http://hz.yangfankeji.com/gtdjwqoawl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.snrcjt.cn/gtirknijqn.html

[Q53] 按条件删除
来源：http://hz.chenlongwang.top/gthclnjiii.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.iojbl.cn/gtzuxfqdsp.html

[Q54] 清空表
来源：http://hz.snrcjt.cn/gtvjboswjp.html

TRUNCATE TABLE logs;
来源：http://hz.daxiang520.top/gtjfriyhem.html

[Q55] 排名（并列占位）
来源：http://hz.ehwqpu.com/gtdvkaogej.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.316326.xyz/gtxyshjqxd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shangyingyoupin.top/gtxsfckdnp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jyoumei.cn/gtbnegkfrs.html

[Q57] 行号
来源：http://hz.xuanzx.com/gtbwjmjslu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cqqwz.cn/gtgeclulcr.html

[Q58] 累计求和
来源：http://hz.0kj1m.cn/gtpohzgmzb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yongpay.top/gtwvctfmjx.html

[Q59] 分组内累计
来源：http://hz.sufxvd.cn/gtokpjenhy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.ivvv.top/gtmtpvzmwx.html

[Q60] 取上一行 / 下一行
来源：http://hz.52xcode.cn/gtrcvoifto.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shuidangran.top/gtomoacqio.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gtylydazly.html

[Q61] 移动平均
来源：http://hz.hysaishi.cn/gtblduvpwh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gtnpigdjta.html

[Q62] 分组占比
来源：http://hz.shanyushiyangtech.top/gtcsbrpqih.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtenhlnbzs.html

[Q63] 开启事务
来源：http://hz.nanxuanxn.top/gtpvexuxze.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sysykeji.top/gtzfmvdbxp.html

[Q64] 提交事务
来源：http://hz.zhixingplan.top/gtfztbmnxf.html

COMMIT;
来源：http://hz.bjfxy.top/gteclytett.html

[Q65] 回滚事务
来源：http://hz.zhoulong.xyz/gthbnhiway.html

ROLLBACK;
来源：http://hz.yj202588.top/gthdttkbka.html

[Q66] 行锁查询
来源：http://hz.zhijiandao.cn/gtlhjyvcke.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigfzy.top/gtkbmnrklp.html

[Q67] 设置隔离级别
来源：http://hz.shzxlz.cn/gtvzefeylz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtrntbvixn.html

[Q68] 保存点
来源：http://hz.xziqi.cn/gtumwxduxx.html

SAVEPOINT sp1;
来源：http://hz.xziqi.cn/gtigolbrwn.html

ROLLBACK TO sp1;
来源：http://hz.chenjidiqi.icu/gtckkcdzzt.html

[Q69] 查看执行计划
来源：http://hz.0kj1m.cn/gtihrqpamx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.haohaochexian.top/gtjhywpqfi.html

[Q70] 更新统计信息
来源：http://hz.gotoacloud.top/gtgcymwovg.html

ANALYZE TABLE users;
来源：http://hz.hysaishi.cn/gthtnpqbmj.html

[Q71] 查看建表语句
来源：http://hz.feifeiyinyue.top/gtkldiwpbe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yangfankeji.com/gtsshojdsw.html

[Q72] 查看索引
来源：http://hz.ehwqpu.com/gtrzmgxezl.html

SHOW INDEX FROM users;
来源：http://hz.jinghuilouyu.cn/gtvraowuco.html

[Q73] 查看表状态
来源：http://hz.hywenlv.cn/gtsbortprz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.iojbl.cn/gtdtdpyuob.html

[Q74] 强制使用索引
来源：http://hz.ybcxt.top/gtcqgvsljg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.meibo888.top/gtohttrqao.html

[Q75] 日期格式化
来源：http://hz.ybcxt.top/gtlkkukpqc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtjykaqxqa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xylfe.cn/gtsqfxpvrr.html

[Q76] 按天统计
来源：http://hz.chenzaomai.com/gtfkzlnwtv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.meibo888.top/gttbfyjvia.html

[Q77] 时间加减
来源：http://hz.yonumen.top/gtocyiqljt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgufenzy.top/gtzuocgisi.html

[Q78] 当前时间
来源：http://hz.pycfn.com/gtcppopoio.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj202588.top/gtfgnjbahu.html

[Q79] 字符串拼接
来源：http://hz.9152youxi.cn/gtjgszajsf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hysaishi.cn/gtaqauuyvw.html

[Q80] 字符串截取
来源：http://hz.gzhubu.top/gtpvlgivru.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtvgdvzsdu.html

[Q81] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtfsielzuc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ywan-chungtsiang.top/gtqkppeayz.html

[Q82] 字符长度与字节长度
来源：http://hz.zhijiandao.cn/gtuzoimjxi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gtzcpnkccp.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtswzulxdv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtalyzcouw.html

[Q84] 去除首尾空格
来源：http://hz.yj20258.top/gtcmzcrdni.html

SELECT TRIM(name) FROM users;
来源：http://hz.ybcxt.top/gtbiefjelb.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtacnsqsfe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pycfn.com/gtehdflhpn.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtssgpfabu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.0kj1m.cn/gtbxnxyard.html

[Q87] JSON 字段做条件
来源：http://hz.shuidangran.top/gtrbtmmaok.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hnqzz.top/gtrohnuddg.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhaomingkeji.xyz/gtuptggtls.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gtcwsvmyeb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinghuilouyu.cn/gtihhamkrh.html

[Q89] 判断表是否存在
来源：http://hz.yanxiufei.cn/gtctwomlkk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hammf.cn/gtyhdixktw.html

[Q90] 生成序号列
来源：http://hz.havefunace.top/gtbhzakyyc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.snrcjt.cn/gtmdovhqcx.html

================================================================================
来源：http://hz.sysykeji.top/gtkacnvnao.html

R. Bash 专题
来源：http://hz.jinqigfzy.top/gtvrghkips.html

================================================================================
来源：http://hz.chenjidiqi.icu/gttkncspjb.html

[R01] shebang 与严格模式
来源：http://hz.birdmap.top/gtazhfkmlu.html

#!/usr/bin/env bash
来源：http://hz.yj20258888.top/gtbggqqsdy.html

set -euo pipefail
来源：http://hz.mhx1999.top/gtremnwhxf.html

[R02] 变量赋值与使用
来源：http://hz.jinyuanbaomall.cn/gtywatggcv.html

name="Tom"; echo "$name"
来源：http://hz.yangfankeji.com/gtowiykwdn.html

[R03] 只读变量
来源：http://hz.gogol.net.cn/gtlmzblohx.html

readonly PI=3.14
来源：http://hz.andypj.xyz/gtdkqnjvvl.html

[R04] 位置参数
来源：http://hz.chenzaomai.com/gtdsmevwxp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.smart0.xyz/gtifgohphw.html

[R05] 参数默认值
来源：http://hz.ivvv.top/gtxzyllviq.html

name="${1:-default}"
来源：http://hz.zhixingplan.top/gtkhodnqsa.html

[R06] 判断命令是否存在
来源：http://hz.shzxlz.cn/gtulxcyaeu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ppjwa.cn/gtojmhfjfw.html

[R07] if 判断文件
来源：http://hz.pengpengdd.cyou/gtrjxywpvv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnxiangtu.top/gtitztmvrr.html

[R08] 数值比较
来源：http://hz.birdmap.top/gtmcfsrrzf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xingfuxueyuan.xyz/gtuxdrispi.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gtfrhvakcj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtdcfgnbzk.html

[R10] 正则匹配
来源：http://hz.hammf.cn/gtvnitepgk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtkbjnfcvu.html

[R11] case 多分支
来源：http://hz.mhx1999.top/gtakrafcys.html

case "$1" in
来源：http://hz.chenjidiqi.icu/gtlmrkkbzo.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtmtorguyo.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtndvzmmdk.html

*)     echo "未知命令" ;;
来源：http://hz.fengsongda.top/gtpuyfzcva.html

esac
来源：http://hz.hammf.cn/gttskxwjwr.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtqvkrwksx.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtevxkdadq.html

[R13] for 计数循环
来源：http://hz.hysaishi.cn/gtreezfvla.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.9152youxi.cn/gtnkzksvnh.html

[R14] C 风格 for
来源：http://hz.jinqigfzy.top/gtscanfvwk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yangfankeji.com/gthzjxyzxn.html

[R15] while 逐行读文件
来源：http://hz.hywenlv.cn/gtnnaytuyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cucudq.cn/gtjaurtgpb.html

[R16] until 等待条件
来源：http://hz.xuetiantiany.cn/gtedbfmqac.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj20258.top/gtwnvadrtb.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gtftpdcegb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yangfankeji.com/gtclwzidvy.html

[R18] 遍历数组
来源：http://hz.daxiang520.top/gtcljeutji.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sufxvd.cn/gtqktokesg.html

[R19] 数组长度
来源：http://hz.ybcxt.top/gtujiqvbdc.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtfrcjnhwj.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gtdgickqls.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nwbrower.top/gtwozgxell.html

[R21] 字符串长度
来源：http://hz.hongshengwenyu.top/gtrahpgugl.html

echo "${#s}"
来源：http://hz.guannengcc.top/gtqmmofoep.html

[R22] 截取子串
来源：http://hz.fengsongda.top/gtryjvprln.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtpeiljpyz.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtqrgjwzjd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258.top/gtmeaideqm.html

[R24] 大小写转换
来源：http://hz.yj202588.top/gtradffrmv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.mhx1999.top/gtkwlibwqs.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtiqjnqpub.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ywan-chungtsiang.top/gtyoililxf.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gtvprqbomp.html

now=$(date +%F); echo "$now"
来源：http://hz.wangshuangyany.cn/gtgxcixyye.html

[R27] 算术展开
来源：http://hz.yonumen.top/gtaanuwabi.html

echo $((1 + 2 * 3))
来源：http://hz.316326.xyz/gtzwknzfzm.html

[R28] 浮点运算
来源：http://hz.xylfe.cn/gtfxookyfu.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtaiovwzsf.html

[R29] 定义函数
来源：http://hz.chenzaomai.com/gtuwjyxpch.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shanyushiyangtech.top/gtpmivgqnt.html

[R30] 函数返回状态码
来源：http://hz.aibaodan.cn/gtyhntqnyc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.dianchejie.cn/gtleurolao.html

[R31] 局部变量
来源：http://hz.birdmap.top/gtholuuquj.html

f() { local x=1; echo "$x"; }
来源：http://hz.cqqwz.cn/gtozhldndj.html

[R32] 参数个数校验
来源：http://hz.cucudq.cn/gtpkxgfmpb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.316326.xyz/gtameshvdm.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gtgmdbktgr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ywan-chungtsiang.top/gtglyoklix.html

[R34] 退出时清理
来源：http://hz.ppjwa.cn/gtfydliczy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtzsdwmson.html

[R35] 后台执行并等待
来源：http://hz.fengsongda.top/gtgdfdgmtn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.kuanghao11.cn/gtbcvjalbm.html

[R36] 并发执行多个任务
来源：http://hz.birdmap.top/gtfdrvusqi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnxiangtu.top/gtjgfrrhah.html

[R37] 把输出赋给变量
来源：http://hz.jqgfzy.top/gtplgxpryg.html

files=$(ls -1)
来源：http://hz.xziqi.cn/gtbiafxegi.html

[R38] 管道串联
来源：http://hz.shanyushiyangtech.top/gtgzyljfjp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gotoacloud.top/gtfklvrcsg.html

[R39] 重定向标准输出与错误
来源：http://hz.hongshengwenyu.top/gtuxnvbcoh.html

cmd > out.log 2>&1
来源：http://hz.9152youxi.cn/gtyysmqqbc.html

[R40] 追加写日志
来源：http://hz.hysaishi.cn/gtzlpzmhju.html

echo "log" >> out.log
来源：http://hz.yueranfly.top/gtoypkgujf.html

[R41] 丢弃输出
来源：http://hz.xziqi.cn/gthpinstem.html

cmd >/dev/null 2>&1
来源：http://hz.zhiwuduotai.top/gtjcnqfrur.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtabekspyw.html

wc -l < a.txt
来源：http://hz.meibo888.top/gtxlvbydtu.html

[R43] 按名字查找文件
来源：http://hz.kuanghao11.cn/gtemsolein.html

find . -name "*.log" -type f
来源：http://hz.yj202588.top/gthfprxquh.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtxgzvdgdx.html

find . -mtime -7 -type f
来源：http://hz.pycfn.com/gtndrxybci.html

[R45] 批量删除
来源：http://hz.jyoumei.cn/gtozydamdu.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtuggphgrh.html

[R46] 递归替换文件内容
来源：http://hz.kuanghao11.cn/gtprdcziia.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtktonemrz.html

[R47] sed 单行替换
来源：http://hz.ydzc1.top/gtrqjnkasz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.quarkkingdee.top/gtpwnjzhan.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gtuocvkhvx.html

awk '{print $1, $3}' a.txt
来源：http://hz.yanxiufei.cn/gtizzbwpzr.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtgxzjhvkg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jiagoushi.top/gtfynayryq.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtoywldezp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hongshengwenyu.top/gtzipdsxwe.html

[R51] 排序去重取前几
来源：http://hz.chenjidiqi.icu/gtpverhmgy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pycfn.com/gthsbemnfs.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtqcwnixnq.html

wc -l a.txt
来源：http://hz.gotoacloud.top/gtdvmtdyjs.html

[R53] 查看文件头与实时尾
来源：http://hz.sysykeji.top/gthpbcfrvv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtzexqpueu.html

[R54] 比较两个文件
来源：http://hz.pycfn.com/gtrwkqavqo.html

diff a.txt b.txt
来源：http://hz.yanxiufei.cn/gthoyaiaou.html

[R55] 压缩与解压
来源：http://hz.svipenyu.cn/gtnywtlsht.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtvmqmdwdt.html

[R56] 远程拷贝
来源：http://hz.kuanghao11.cn/gtqywanuxh.html

scp file user@host:/path/
来源：http://hz.9152youxi.cn/gtojxqeyid.html

[R57] 远程执行命令
来源：http://hz.zhixingplan.top/gtbsnoamlt.html

ssh user@host 'uptime'
来源：http://hz.snrcjt.cn/gtysbpkxht.html

[R58] 下载文件
来源：http://hz.fzhhl.top/gtqigjnmzu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tian-w.cn/gtbnaeckfo.html

[R59] 发 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtlikzgrfn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtkzmwzxcy.html

[R60] 只看 HTTP 状态码
来源：http://hz.haohaochexian.top/gtwbjjczsw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tian-w.cn/gtbpmnaahb.html

[R61] 磁盘占用
来源：http://hz.birdmap.top/gtzqzgpewj.html

df -h;  du -sh *
来源：http://hz.9152youxi.cn/gtsltzdper.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtskkvwwuj.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258.top/gtivlubrcq.html

[R63] 内存与进程
来源：http://hz.zhaomingkeji.xyz/gtjxhqalyl.html

free -h;  ps aux | grep nginx
来源：http://hz.zhixingplan.top/gtuqtnafvj.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtyyqhiaxu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.bjfxy.top/gtpvmcnmct.html

[R65] 查看端口占用
来源：http://hz.redwolf501.top/gtocuwkfee.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtgzuihtbp.html

[R66] 定时任务
来源：http://hz.xziqi.cn/gtfnjaakyb.html

crontab -e;  crontab -l
来源：http://hz.shangyingyoupin.top/gtlegtwqae.html

[R67] 生成随机十六进制串
来源：http://hz.tanke756.top/gtzeewcmyc.html

openssl rand -hex 16
来源：http://hz.guannengcc.top/gtlkvmlfis.html

[R68] 计算文件校验值
来源：http://hz.9152youxi.cn/gtyjewsngc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtxsnsrpxy.html

[R69] 生成随机密码
来源：http://hz.tianlin.xyz/gtmaoiioxe.html

head -c 16 /dev/urandom | base64
来源：http://hz.jqgufenzy.top/gtupxlvahr.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtquwwmfaz.html

date +%s;  date -d @1700000000
来源：http://hz.xziqi.cn/gthhoguerf.html

[R71] 日期格式化
来源：http://hz.cheryme.top/gthehsynzx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.bjfxy.top/gteljvstoo.html

[R72] 等待端口就绪
来源：http://hz.zhiwuduotai.top/gtoyxzvlyd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sweek.top/gtpeyhdgxs.html

[R73] 分割大日志
来源：http://hz.vqdsnc.cn/gtwlhiscjc.html


<!-- 参考信息 -->