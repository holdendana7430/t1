代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.hammf.cn/gtdrorezay.html

[Q30] 分组统计
来源：http://hz.pengpengdd.cyou/gtwkshspqw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.yj20258.top/gttbnpzost.html

[Q31] 分组后过滤
来源：http://hz.xuetiantiany.cn/gtvphenrua.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.tanke756.top/gtswktltkm.html

[Q32] 分组拼接字符串
来源：http://hz.nanxuanxn.top/gtpuovxztg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.pengpengdd.cyou/gtlyxmcxxx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.ivvv.top/gtpewobhpu.html

[Q33] 多列分组
来源：http://hz.jiagoushi.top/gtxueobxmf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.cqqwz.cn/gtuwrijoba.html

[Q34] 每组取第一条
来源：http://hz.aizwys.cn/gtjzblephv.html

SELECT * FROM (
来源：http://hz.yj202588.top/gtpxigoxuy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.andypj.xyz/gtdsrcxwjr.html

) t WHERE rn = 1;
来源：http://hz.zdqjudy.top/gtkczsscws.html

[Q35] 内连接
来源：http://hz.ywan-chungtsiang.top/gtirrtgque.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.wangshuangyany.cn/gtedlcaosb.html

[Q36] 左连接
来源：http://hz.yj20258.top/gtjsbfcgfy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sufxvd.cn/gtkohwiapz.html

[Q37] 右连接
来源：http://hz.chenzaomai.com/gtlvinnlpt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.redwolf501.top/gtpyrzydms.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.gaohongyu789.top/gttcwmpirg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtskswlaru.html

[Q39] 自连接（查上下级）
来源：http://hz.xingfuxueyuan.xyz/gtmycitkcp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jianghu66.top/gtezgyxwwg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xuetiantiany.cn/gtuzljfszl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.guannengcc.top/gtuqjldxbd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daxiang520.top/gtgfctidwc.html

[Q41] 多表连接
来源：http://hz.iojbl.cn/gtibbyklhu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.wangdashe.top/gtbtiizvzw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zdqjudy.top/gtwzhtnrxw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cdnleiting.top/gtceyrjftp.html

[Q42] 连接条件附加过滤
来源：http://hz.shuidangran.top/gtmjygsspc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.xuetiantiany.cn/gtzkckifxl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.dianchejie.cn/gtlsbcyqmq.html

[Q43] 标量子查询
来源：http://hz.snrcjt.cn/gtotsfvgxk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.aizwys.cn/gtfbojhabx.html

[Q44] IN 子查询
来源：http://hz.fengsongda.top/gtfcwjqpju.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dashuyun.cn/gtpolmqwzp.html

[Q45] EXISTS 判断存在
来源：http://hz.cashguo.top/gtysmreysa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gthniizxgs.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aibaodan.cn/gtlnntxltv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.c1oappe.top/gtmccjwixv.html

[Q47] 与平均值比较
来源：http://hz.svipenyu.cn/gtzegftmzj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hfpthk.cn/gtntobcemp.html

[Q48] CTE 公用表表达式
来源：http://hz.birdmap.top/gtrjcyrimt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.hammf.cn/gticxvsxrx.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ivvv.top/gtfaqcrmgj.html

[Q49] 更新单行
来源：http://hz.yj20258888.top/gtjtosteoo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yonumen.top/gtyluvpqbk.html

[Q50] 批量更新
来源：http://hz.yuanzhike.top/gthlocvazv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ehwqpu.com/gtelfuumvn.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtlapltyxd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cucudq.cn/gtvtskcvko.html

[Q52] 删除指定行
来源：http://hz.jinghuilouyu.cn/gtmdrjypvg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tanke756.top/gtrwvoutrf.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtsolrcjcg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.birdmap.top/gtizbytoct.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtaffrddum.html

TRUNCATE TABLE logs;
来源：http://hz.xingfuxueyuan.xyz/gtlhibbuzf.html

[Q55] 排名（并列占位）
来源：http://hz.tanke756.top/gtzpaifkgw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhijiandao.cn/gtndybfglq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj202588.top/gtyvhoerno.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.aibaodan.cn/gtoanhgyep.html

[Q57] 行号
来源：http://hz.vqdsnc.cn/gtpdupmhcs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ppjwa.cn/gttxwikfun.html

[Q58] 累计求和
来源：http://hz.jlsjyb.cn/gturxvrtbc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hfpthk.cn/gtzuywhuib.html

[Q59] 分组内累计
来源：http://hz.bjfxy.top/gtfofbjobv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.316326.xyz/gtfbiapdnl.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtjfnpobxz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.9152youxi.cn/gtjjpkvrar.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258888.top/gtwsrvmuog.html

[Q61] 移动平均
来源：http://hz.yanxiufei.cn/gtphupkloz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cdnleiting.top/gtxcvpyszt.html

[Q62] 分组占比
来源：http://hz.chenzaomai.com/gtzzbjiucm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.snrcjt.cn/gtyrsrbdnd.html

[Q63] 开启事务
来源：http://hz.nanxinkj.top/gtocsgairm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yvedp.cn/gtmefqymip.html

[Q64] 提交事务
来源：http://hz.aibaodan.cn/gtjebhvbkt.html

COMMIT;
来源：http://hz.zhoulong.xyz/gthxkthmsq.html

[Q65] 回滚事务
来源：http://hz.zhengqikj.top/gtspxnkjiq.html

ROLLBACK;
来源：http://hz.jiagoushi.top/gtiewgifvb.html

[Q66] 行锁查询
来源：http://hz.yj20258.top/gtslaqylhk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.snrcjt.cn/gtqkqpzdhg.html

[Q67] 设置隔离级别
来源：http://hz.sxryk.cn/gtbqwrhukp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenjidiqi.icu/gtnmthwlyc.html

[Q68] 保存点
来源：http://hz.jinqigufen.top/gtpbvdweeh.html

SAVEPOINT sp1;
来源：http://hz.yvedp.cn/gttewjhtvj.html

ROLLBACK TO sp1;
来源：http://hz.andypj.xyz/gtnkhdyarp.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtyvteaato.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtuogapdle.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtmogpvwfz.html

ANALYZE TABLE users;
来源：http://hz.daxiang520.top/gtfqcspmgc.html

[Q71] 查看建表语句
来源：http://hz.cqqwz.cn/gtxqrvdpnb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fengsongda.top/gtfwfupjmc.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gtghoutjnp.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtllvocsyk.html

[Q73] 查看表状态
来源：http://hz.fengsongda.top/gtrxacpkjn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tian-w.cn/gtxeomormv.html

[Q74] 强制使用索引
来源：http://hz.pycfn.com/gtotoujxlt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhaomingkeji.xyz/gtbdflocjk.html

[Q75] 日期格式化
来源：http://hz.gaohongyu789.top/gtukqprdjs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.meibo888.top/gtusymndiq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jinyuanbaomall.cn/gtujyercwh.html

[Q76] 按天统计
来源：http://hz.gogol.net.cn/gtlpysszhg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jianghu66.top/gttswqaaqt.html

[Q77] 时间加减
来源：http://hz.yj20258888.top/gtccfqabkp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.tanke756.top/gtgudsxxlo.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtkcvezjsk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cheryme.top/gteamtxwcl.html

[Q79] 字符串拼接
来源：http://hz.aibaodan.cn/gttdtvpxeo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gtmbnjbvvs.html

[Q80] 字符串截取
来源：http://hz.ywan-chungtsiang.top/gtomvvraxp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.redwolf501.top/gtocrqazou.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtjcapngoo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tanke756.top/gtysindcam.html

[Q82] 字符长度与字节长度
来源：http://hz.52xcode.cn/gtytzevbvt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.quarkkingdee.top/gtvmeovymc.html

[Q83] 大小写转换
来源：http://hz.gotoacloud.top/gtpclzueqx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.redwolf501.top/gthxxkazin.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtvlrsulou.html

SELECT TRIM(name) FROM users;
来源：http://hz.ybcxt.top/gtgwmrweei.html

[Q85] 数值取整
来源：http://hz.ehwqpu.com/gtaywsanps.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pycfn.com/gtdycgwemd.html

[Q86] 读取 JSON 字段
来源：http://hz.fzhhl.top/gtqunyktrg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtsjhngllb.html

[Q87] JSON 字段做条件
来源：http://hz.ybcxt.top/gtnozjossk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.bjfxy.top/gtcvhsibbe.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtplrtidec.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.iojbl.cn/gtphemgodi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtrqmyihho.html

[Q89] 判断表是否存在
来源：http://hz.jinghuilouyu.cn/gtlkyloacz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aibaodan.cn/gtcrvzktpn.html

[Q90] 生成序号列
来源：http://hz.ehwqpu.com/gtzysgubdm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258.top/gtsasyxksr.html

================================================================================
来源：http://hz.ppjwa.cn/gtbqkryrgo.html

R. Bash 专题
来源：http://hz.hongshengwenyu.top/gtipoacukm.html

================================================================================
来源：http://hz.meibo888.top/gtkyantbrg.html

[R01] shebang 与严格模式
来源：http://hz.yonumen.top/gtomccbdeh.html

#!/usr/bin/env bash
来源：http://hz.aizwys.cn/gtzviyttmj.html

set -euo pipefail
来源：http://hz.hongshengwenyu.top/gtuxuazgvu.html

[R02] 变量赋值与使用
来源：http://hz.zhengqikj.top/gtxugjldlq.html

name="Tom"; echo "$name"
来源：http://hz.aizwys.cn/gtnyobhpkp.html

[R03] 只读变量
来源：http://hz.yongpay.top/gtluhtvfly.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gttlvrmjkn.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtmqcubmno.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.kuanghao11.cn/gtnswwtybf.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtmvjaqors.html

name="${1:-default}"
来源：http://hz.hfpthk.cn/gtlolsxbek.html

[R06] 判断命令是否存在
来源：http://hz.jinghuilouyu.cn/gttqanoivm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cdnleiting.top/gtrnamtpoz.html

[R07] if 判断文件
来源：http://hz.guannengcc.top/gtflztjfwv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtvywqqghz.html

[R08] 数值比较
来源：http://hz.yueranfly.top/gtgwyqjfhb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ppjwa.cn/gtvusupaei.html

[R09] 字符串比较
来源：http://hz.xuanzx.com/gtyzfctfmv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yvedp.cn/gtnqinxted.html

[R10] 正则匹配
来源：http://hz.guowangkeji.top/gtsxzaydrt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jiagoushi.top/gtfaapldth.html

[R11] case 多分支
来源：http://hz.jinqigufen.top/gtlzvdxgye.html

case "$1" in
来源：http://hz.0kj1m.cn/gtbknoabfd.html

start) echo "启动" ;;
来源：http://hz.pycfn.com/gtuoiqczao.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtjuoecsym.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gtnvzktbnf.html

esac
来源：http://hz.jinghuilouyu.cn/gtwlyyhnps.html

[R12] for 遍历文件
来源：http://hz.nwbrower.top/gtnxcwxemm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtvoltcqtn.html

[R13] for 计数循环
来源：http://hz.nwbrower.top/gtovhgujar.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sweek.top/gtghhuaevp.html

[R14] C 风格 for
来源：http://hz.zhiwuduotai.top/gtkgmztgji.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.andypj.xyz/gttmaeqfdw.html

[R15] while 逐行读文件
来源：http://hz.cdnleiting.top/gtowtwzgpx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhaomingkeji.xyz/gtltunkrzn.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtorusmavp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtzawjfswf.html

[R17] 数组定义与取值
来源：http://hz.cheryme.top/gtppmsdnex.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cashguo.top/gturuqcjml.html

[R18] 遍历数组
来源：http://hz.tanke756.top/gtxrapgfoq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgfzy.top/gtomolozsk.html

[R19] 数组长度
来源：http://hz.kuanghao11.cn/gtcwdpwjzf.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtrspujeep.html

[R20] 关联数组（字典）
来源：http://hz.iojbl.cn/gtrhfjndcn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gtvzoofnlm.html

[R21] 字符串长度
来源：http://hz.c1oappe.top/gtikiagzdp.html

echo "${#s}"
来源：http://hz.gotoacloud.top/gtuhbkhmrh.html

[R22] 截取子串
来源：http://hz.wangdashe.top/gtfukzwwsj.html

echo "${s:0:5}"
来源：http://hz.jqgfzy.top/gtvqmvjhyc.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtlqfzzrnu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hfpthk.cn/gtfvgmipxs.html

[R24] 大小写转换
来源：http://hz.sufxvd.cn/gtunexeqnz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuanzx.com/gtvtegjbdb.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhoulong.xyz/gtjxgjjdos.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yanxiufei.cn/gtwjwlzazk.html

[R26] 命令替换
来源：http://hz.ybcxt.top/gtjyijzmiz.html

now=$(date +%F); echo "$now"
来源：http://hz.xuetiantiany.cn/gtwdgqwcjm.html

[R27] 算术展开
来源：http://hz.yj20258.top/gtwqnngdkr.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtgvjfzqut.html

[R28] 浮点运算
来源：http://hz.ivvv.top/gtcezpjixb.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhiwuduotai.top/gtvvtilbgq.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gtnmssolbw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cheryme.top/gtnsjotgko.html

[R30] 函数返回状态码
来源：http://hz.cashguo.top/gtyawhxovx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sxryk.cn/gtdqbralhr.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gtnbcgfxzn.html

f() { local x=1; echo "$x"; }
来源：http://hz.haohaochexian.top/gtsxuqmdzw.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtrqzbcmcn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhiwuduotai.top/gtfnkpspdr.html

[R33] 捕获错误并提示行号
来源：http://hz.daxiang520.top/gtzzqnhbqo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.quarkkingdee.top/gtbydiuuja.html

[R34] 退出时清理
来源：http://hz.yj20258.top/gtcixphtve.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtedmqglgz.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gtpmsnascu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydjk.org.cn/gtswaxvvze.html

[R36] 并发执行多个任务
来源：http://hz.nanxuanxn.top/gtbbtslgur.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtnudjgrta.html

[R37] 把输出赋给变量
来源：http://hz.yangfankeji.com/gtnxfjxmbp.html

files=$(ls -1)
来源：http://hz.wangdashe.top/gttjwmnher.html

[R38] 管道串联
来源：http://hz.zhoulong.xyz/gtacvuviep.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tian-w.cn/gtqxeuhycg.html

[R39] 重定向标准输出与错误
来源：http://hz.316326.xyz/gtvqlergcd.html

cmd > out.log 2>&1
来源：http://hz.wangshuangyany.cn/gtrcizdkcr.html

[R40] 追加写日志
来源：http://hz.smart0.xyz/gtuklgbmlh.html

echo "log" >> out.log
来源：http://hz.yanxiufei.cn/gtjzghlvdd.html

[R41] 丢弃输出
来源：http://hz.meibo888.top/gtmnyduhek.html

cmd >/dev/null 2>&1
来源：http://hz.jinyuanbaomall.cn/gtmztzjbyr.html

[R42] 输入重定向
来源：http://hz.wangdashe.top/gtwlxtexlg.html

wc -l < a.txt
来源：http://hz.dashuyun.cn/gtfxpwaikr.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtetdlovih.html

find . -name "*.log" -type f
来源：http://hz.jinyuanbaomall.cn/gtjicfolzp.html

[R44] 按修改时间查找
来源：http://hz.ybcxt.top/gtnoarappb.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtxazeeiap.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtbuhwifes.html

find . -name "*.tmp" -delete
来源：http://hz.ydzc1.top/gtsjbhfeji.html

[R46] 递归替换文件内容
来源：http://hz.shzxlz.cn/gtgeppukyu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ehwqpu.com/gtygcucaoy.html

[R47] sed 单行替换
来源：http://hz.gzhubu.top/gtlscdgbbm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shuidangran.top/gtcjjaokfi.html

[R48] awk 取指定列
来源：http://hz.redwolf501.top/gtktamrxmf.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtoriuinxo.html

[R49] awk 带条件
来源：http://hz.hfpthk.cn/gtejakszip.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtsnnnhrui.html

[R50] awk 求和
来源：http://hz.aibaodan.cn/gtwjsmcxlp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtlhmtztuk.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtfmwauszo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ehwqpu.com/gtrfyumyxp.html

[R52] 统计行数
来源：http://hz.sxryk.cn/gtbhzixnip.html

wc -l a.txt
来源：http://hz.gaohongyu789.top/gtlnooevpq.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtpuyuojwy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtxmalvvvv.html

[R54] 比较两个文件
来源：http://hz.mhx1999.top/gtgzyysvso.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gtxdmwjqfx.html

[R55] 压缩与解压
来源：http://hz.sufxvd.cn/gtbiwkxzzb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhiwuduotai.top/gtzrbiotje.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtaywqvtcm.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gtogvfmiom.html

[R57] 远程执行命令
来源：http://hz.guannengcc.top/gthvxircfq.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtsojjtggf.html

[R58] 下载文件
来源：http://hz.pycfn.com/gtxanvqwlr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhaomingkeji.xyz/gtksjotrdj.html

[R59] 发 POST JSON
来源：http://hz.9152youxi.cn/gtnzqmiyvc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ppjwa.cn/gtmapkqvuv.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinqigfzy.top/gteiwppziy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.feifeiyinyue.top/gtktkyogis.html

[R61] 磁盘占用
来源：http://hz.haohaochexian.top/gthiwspdtt.html

df -h;  du -sh *
来源：http://hz.xuanzx.com/gtiigkrdof.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gtyyhkplvb.html

du -ah . | sort -rh | head -10
来源：http://hz.shzxlz.cn/gtyhocqdpu.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtdckwezgl.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtwlwwzqik.html

[R64] 结束进程
来源：http://hz.andypj.xyz/gtzlatklzn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258888.top/gtzsulyodk.html

[R65] 查看端口占用
来源：http://hz.zhixingplan.top/gtditrjefc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258.top/gtvtiluwyb.html

[R66] 定时任务
来源：http://hz.316326.xyz/gtqruegvkq.html

crontab -e;  crontab -l
来源：http://hz.svipenyu.cn/gthcbyoaxp.html

[R67] 生成随机十六进制串
来源：http://hz.shuidangran.top/gtogdobzwu.html

openssl rand -hex 16
来源：http://hz.xuetiantiany.cn/gtwqmlzmiy.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtqshuehfr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtoofusddf.html

[R69] 生成随机密码
来源：http://hz.daria6918.cn/gtfxdnmfma.html

head -c 16 /dev/urandom | base64
来源：http://hz.ivvv.top/gtlaminhjf.html

[R70] 时间戳与互转
来源：http://hz.dianchejie.cn/gtecsahjej.html

date +%s;  date -d @1700000000
来源：http://hz.shangyingyoupin.top/gtflduzxdm.html

[R71] 日期格式化
来源：http://hz.daxiang520.top/gtlwqmouzx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtbbuavbki.html

[R72] 等待端口就绪
来源：http://hz.kuanghao11.cn/gtpbrxnbhu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenzaomai.com/gtevcydfnc.html

[R73] 分割大日志
来源：http://hz.hysaishi.cn/gtchoaekjb.html

split -l 1000 big.log part_
来源：http://hz.ppjwa.cn/gtvmzdkiaz.html

[R74] 批量重命名
来源：http://hz.9152youxi.cn/gtfhjvechg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ivvv.top/gtcgidtvcj.html

[R75] 导出环境变量
来源：http://hz.zhongyouzk.top/gtuxuiikwp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hfpthk.cn/gtztitqafv.html

[R76] 使用临时文件
来源：http://hz.wangshuangyany.cn/gtnmkxuesc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtjpijqkqi.html

[R77] 读取用户输入
来源：http://hz.pengpengdd.cyou/gtlswuvwdr.html

read -rp "请输入: " ans
来源：http://hz.yj20258888.top/gtloryrkmc.html

[R78] 交互式菜单
来源：http://hz.xziqi.cn/gtgmxddget.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.kuanghao11.cn/gtzwdugwha.html

[R79] 解析命令行选项
来源：http://hz.tanke756.top/gthjdolbnf.html


<!-- 参考信息 -->