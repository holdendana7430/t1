代发 wailian999

[Q33] 多列分组
来源：http://hz.aibaodan.cn/gtwoadpsef.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ehwqpu.com/gtmrlgqbmz.html

[Q34] 每组取第一条
来源：http://hz.wangdashe.top/gtioafvczp.html

SELECT * FROM (
来源：http://hz.guannengcc.top/gtligwuyfk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jianghu66.top/gtehvmsbaj.html

) t WHERE rn = 1;
来源：http://hz.ehwqpu.com/gtntqzxjvl.html

[Q35] 内连接
来源：http://hz.yanxiufei.cn/gtftqhpznv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydzc1.top/gtyfttgcsv.html

[Q36] 左连接
来源：http://hz.daxiang520.top/gtvcstgdoh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.yuxming.cn/gtgbckjivn.html

[Q37] 右连接
来源：http://hz.jiagoushi.top/gtqjzurbpa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sweek.top/gtdabwwect.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gtiwggqdzi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hongshengwenyu.top/gtmirfqrvf.html

[Q39] 自连接（查上下级）
来源：http://hz.316326.xyz/gtosqqmiaj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zdqjudy.top/gtbdozgszq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xylfe.cn/gtdaopveib.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.iojbl.cn/gtlewjnfdj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtgnfxehfv.html

[Q41] 多表连接
来源：http://hz.0kj1m.cn/gtpzjuwloe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hongshengwenyu.top/gtrbisfttw.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yonumen.top/gtowjlfgww.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.aizwys.cn/gtakcdvqjk.html

[Q42] 连接条件附加过滤
来源：http://hz.yongpay.top/gteautqpth.html

SELECT u.name, o.amount FROM users u
来源：http://hz.sysykeji.top/gteuuxrara.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jinqigfzy.top/gtmyngitsd.html

[Q43] 标量子查询
来源：http://hz.xuetiantiany.cn/gtvwatsaam.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.mhx1999.top/gtxsewqvhl.html

[Q44] IN 子查询
来源：http://hz.shuidangran.top/gtebfrxdmo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.hywenlv.cn/gtealdauzx.html

[Q45] EXISTS 判断存在
来源：http://hz.316326.xyz/gtupzmxzad.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.daria6918.cn/gtjurmhscv.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xinyue.icu/gthpdzfnpk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhaomingkeji.xyz/gteguzobzq.html

[Q47] 与平均值比较
来源：http://hz.shanyushiyangkeji.top/gtfavdlqjc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.tanke756.top/gtdnyqpblc.html

[Q48] CTE 公用表表达式
来源：http://hz.ybcxt.top/gtgnanktot.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinqigfzy.top/gtoijpzbls.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jyoumei.cn/gtfmidnlpj.html

[Q49] 更新单行
来源：http://hz.fzhhl.top/gtcztfefor.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhixingplan.top/gtdndmvzew.html

[Q50] 批量更新
来源：http://hz.jinqigfzy.top/gtgedsmqrd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.smart0.xyz/gtcjfneypz.html

[Q51] 用子查询更新
来源：http://hz.zhongyouzk.top/gtbpoiswuz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cucudq.cn/gtfgbdqova.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gtynlinbik.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fzhhl.top/gtqkdjqrvk.html

[Q53] 按条件删除
来源：http://hz.chenzaomai.com/gtvhuwenhp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xziqi.cn/gtytxswhyx.html

[Q54] 清空表
来源：http://hz.zhaomingkeji.xyz/gtxxfrwbxo.html

TRUNCATE TABLE logs;
来源：http://hz.zhengqikj.top/gtdscqhpvd.html

[Q55] 排名（并列占位）
来源：http://hz.dashuyun.cn/gtmadfhdhp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.0kj1m.cn/gtgszxbxbq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtrrfvjaop.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pengpengdd.cyou/gtidnfbnkv.html

[Q57] 行号
来源：http://hz.hysaishi.cn/gtbdqmlcse.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.sweek.top/gtdvxmcbld.html

[Q58] 累计求和
来源：http://hz.hnqzz.top/gthvvblexq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zhiwuduotai.top/gtrnonrdpx.html

[Q59] 分组内累计
来源：http://hz.cashguo.top/gtcqecyrjh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yonumen.top/gtdspruiwp.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinqigfzy.top/gtlfikuxcr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.haohaochexian.top/gtolksccxt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgufenzy.top/gtglsqeemg.html

[Q61] 移动平均
来源：http://hz.shangyingyoupin.top/gtdxczrffa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhoulong.xyz/gtjnmyiwbs.html

[Q62] 分组占比
来源：http://hz.jinqigufen.top/gttiznkcwe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtixstwkra.html

[Q63] 开启事务
来源：http://hz.cucudq.cn/gtaopugfnb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhiwuduotai.top/gtmzqsvnlc.html

[Q64] 提交事务
来源：http://hz.wangshuangyany.cn/gtdhsnvrzg.html

COMMIT;
来源：http://hz.nwbrower.top/gtriosduvv.html

[Q65] 回滚事务
来源：http://hz.jinghuilouyu.cn/gtcedvnzcz.html

ROLLBACK;
来源：http://hz.cqqwz.cn/gtymqecdfr.html

[Q66] 行锁查询
来源：http://hz.jyoumei.cn/gtvvihrfpt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.bjfxy.top/gtrdfziwdy.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtmgsaylsw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtintaiqlu.html

[Q68] 保存点
来源：http://hz.gotoacloud.top/gtfzylprqf.html

SAVEPOINT sp1;
来源：http://hz.tanke756.top/gtkxlswsdy.html

ROLLBACK TO sp1;
来源：http://hz.yangfankeji.com/gtnbablzgf.html

[Q69] 查看执行计划
来源：http://hz.iojbl.cn/gthmnwaqsl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shuidangran.top/gturnckqtu.html

[Q70] 更新统计信息
来源：http://hz.xziqi.cn/gtxsoefqnd.html

ANALYZE TABLE users;
来源：http://hz.smart0.xyz/gtapmvdxun.html

[Q71] 查看建表语句
来源：http://hz.52xcode.cn/gtrnzdlcga.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.andypj.xyz/gtkzlmvjpo.html

[Q72] 查看索引
来源：http://hz.snrcjt.cn/gtpxzancby.html

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtfgxfupjy.html

[Q73] 查看表状态
来源：http://hz.guowangkeji.top/gtvddrsllq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xinyue.icu/gthdvzhiph.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gtvrjaoqor.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gttkbyoqrc.html

[Q75] 日期格式化
来源：http://hz.yuxming.cn/gtsnvkbhpb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xinyue.icu/gtqqhvyhpz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sxryk.cn/gtcxckaduh.html

[Q76] 按天统计
来源：http://hz.aibaodan.cn/gtllclcmhq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hysaishi.cn/gtzjishtzx.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gtcpfnycrs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtcckpuucc.html

[Q78] 当前时间
来源：http://hz.jinghuilouyu.cn/gtsybchgrj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xingfuxueyuan.xyz/gtdfnuanqi.html

[Q79] 字符串拼接
来源：http://hz.jinqigufen.top/gthyhfmvwt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnxiangtu.top/gtrormthry.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtiexidvfd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtpoohymgg.html

[Q81] 字符串替换
来源：http://hz.xziqi.cn/gtpfyfghay.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yangfankeji.com/gtmsftrvik.html

[Q82] 字符长度与字节长度
来源：http://hz.yanxiufei.cn/gtmclwrufs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtrteitkyd.html

[Q83] 大小写转换
来源：http://hz.shangyingyoupin.top/gtuqwpenai.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hysaishi.cn/gtrxvxefqa.html

[Q84] 去除首尾空格
来源：http://hz.xylfe.cn/gtiqdvkpss.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtceszzqib.html

[Q85] 数值取整
来源：http://hz.redwolf501.top/gtpporxgbj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.0kj1m.cn/gtagtuyuae.html

[Q86] 读取 JSON 字段
来源：http://hz.jyoumei.cn/gtsftzygrc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xylfe.cn/gtnygenlwm.html

[Q87] JSON 字段做条件
来源：http://hz.xylfe.cn/gttccvcboc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nwbrower.top/gtytfkvang.html

[Q88] 行转列（条件聚合）
来源：http://hz.daria6918.cn/gttbntxxba.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hongshengwenyu.top/gtrpmfwbzn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj202588.top/gtlvkkdtxb.html

[Q89] 判断表是否存在
来源：http://hz.pycfn.com/gtbruzdfno.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dianchejie.cn/gtqstrrhsn.html

[Q90] 生成序号列
来源：http://hz.guowangkeji.top/gttgpwjpqf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnxiangtu.top/gturygqxad.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkieqmzjx.html

R. Bash 专题
来源：http://hz.nanxuanxn.top/gtyatqytzh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmzejondl.html

[R01] shebang 与严格模式
来源：http://hz.gotoacloud.top/gtqwatxvus.html

#!/usr/bin/env bash
来源：http://hz.ivvv.top/gtfdtwvtod.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtqqypymcd.html

[R02] 变量赋值与使用
来源：http://hz.cashguo.top/gtrhbaiqdw.html

name="Tom"; echo "$name"
来源：http://hz.gogol.net.cn/gtjecfprfz.html

[R03] 只读变量
来源：http://hz.yangfankeji.com/gtrmfwumql.html

readonly PI=3.14
来源：http://hz.xziqi.cn/gtpodzpkhr.html

[R04] 位置参数
来源：http://hz.xinyue.icu/gtvouvbbus.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jlsjyb.cn/gtjkltgnsl.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtcphgzaap.html

name="${1:-default}"
来源：http://hz.gotoacloud.top/gtlhyoocrr.html

[R06] 判断命令是否存在
来源：http://hz.jyoumei.cn/gtkakewxwt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.quarkkingdee.top/gtswgthmbx.html

[R07] if 判断文件
来源：http://hz.yuxming.cn/gthvrxllxd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gtcomxddle.html

[R08] 数值比较
来源：http://hz.svipenyu.cn/gtadvjaeje.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtmrlljdsb.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gttmjqztmg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.c1oappe.top/gtezidughs.html

[R10] 正则匹配
来源：http://hz.gzhubu.top/gtlpluedmj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtzhseyuxp.html

[R11] case 多分支
来源：http://hz.c1oappe.top/gtyqccmeuc.html

case "$1" in
来源：http://hz.cheryme.top/gtdkzjdalv.html

start) echo "启动" ;;
来源：http://hz.yongpay.top/gtkbpwfnaj.html

stop)  echo "停止" ;;
来源：http://hz.jqgufenzy.top/gtfqmxbdkb.html

*)     echo "未知命令" ;;
来源：http://hz.yanxiufei.cn/gtareebqxu.html

esac
来源：http://hz.gotoacloud.top/gtbqeemsuq.html

[R12] for 遍历文件
来源：http://hz.jinqigfzy.top/gtnuhaqiyd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuanzx.com/gtwugfdrhi.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtwcvmlawa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangkeji.top/gtdzqjaepo.html

[R14] C 风格 for
来源：http://hz.gaohongyu789.top/gtqbubbulb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jiagoushi.top/gtgyigkinb.html

[R15] while 逐行读文件
来源：http://hz.jiagoushi.top/gthsuhbrif.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.svipenyu.cn/gtvlvobbxg.html

[R16] until 等待条件
来源：http://hz.0kj1m.cn/gtanoptazi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtejkwuias.html

[R17] 数组定义与取值
来源：http://hz.fengsongda.top/gtslsoervo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhoulong.xyz/gtcrzvjsav.html

[R18] 遍历数组
来源：http://hz.ydjk.org.cn/gtnytwnftq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xziqi.cn/gtchbnhsfv.html

[R19] 数组长度
来源：http://hz.xuanzx.com/gtgzfjjqph.html

echo "${#arr[@]}"
来源：http://hz.yonumen.top/gtbemtdttm.html

[R20] 关联数组（字典）
来源：http://hz.gaohongyu789.top/gtrvohdbyj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daria6918.cn/gtqpquxrqz.html

[R21] 字符串长度
来源：http://hz.guowangkeji.top/gtyuuhghxt.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtalnsqcor.html

[R22] 截取子串
来源：http://hz.fzhhl.top/gtqrthqyqh.html

echo "${s:0:5}"
来源：http://hz.daxiang520.top/gtfilmiwwk.html

[R23] 字符串替换
来源：http://hz.hywenlv.cn/gtwcgtdtde.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tanke756.top/gtlrwdotfr.html

[R24] 大小写转换
来源：http://hz.hfpthk.cn/gtkfyhemcj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pengpengdd.cyou/gtazenxdfd.html

[R25] 去后缀 / 去前缀
来源：http://hz.tianlin.xyz/gtkptezzve.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.feifeiyinyue.top/gtodnedxjx.html

[R26] 命令替换
来源：http://hz.yvedp.cn/gtymaxawtc.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gttyexgxug.html

[R27] 算术展开
来源：http://hz.zdqjudy.top/gtqiuzphnp.html

echo $((1 + 2 * 3))
来源：http://hz.xinyue.icu/gtwxixtmys.html

[R28] 浮点运算
来源：http://hz.snrcjt.cn/gtfqajfukk.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtantniqqs.html

[R29] 定义函数
来源：http://hz.zhixingplan.top/gthiwbdhdl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnqzz.top/gtlqzukghf.html

[R30] 函数返回状态码
来源：http://hz.yongpay.top/gthaoygosx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhiwuduotai.top/gtmclqxzxu.html

[R31] 局部变量
来源：http://hz.jyoumei.cn/gtwrtnwzjq.html

f() { local x=1; echo "$x"; }
来源：http://hz.daxiang520.top/gtwrshftna.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gtscvrtqgb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtbcgrdfrc.html

[R33] 捕获错误并提示行号
来源：http://hz.zhiwuduotai.top/gtjeleiaie.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cashguo.top/gtbdnuzhlh.html

[R34] 退出时清理
来源：http://hz.birdmap.top/gtdavwepds.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pengpengdd.cyou/gtgxtonamg.html

[R35] 后台执行并等待
来源：http://hz.zhengqikj.top/gthcajjrja.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.wangdashe.top/gtlrafqtmn.html

[R36] 并发执行多个任务
来源：http://hz.xinyue.icu/gttyyhlkux.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xinyue.icu/gtsynmendv.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtngzwhfef.html

files=$(ls -1)
来源：http://hz.daria6918.cn/gtpigzkkgx.html

[R38] 管道串联
来源：http://hz.zhongyouzk.top/gtqhntisjz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgufenzy.top/gtpdcthrer.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtifdrlela.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gtjtftxrbr.html

[R40] 追加写日志
来源：http://hz.316326.xyz/gtdbfsqmtw.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtjrxdvckv.html

[R41] 丢弃输出
来源：http://hz.ppjwa.cn/gtvbazcqfw.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtjhnbmerw.html

[R42] 输入重定向
来源：http://hz.hywenlv.cn/gtlucmxovu.html

wc -l < a.txt
来源：http://hz.gotoacloud.top/gtibiodayt.html

[R43] 按名字查找文件
来源：http://hz.shzxlz.cn/gtjforywae.html

find . -name "*.log" -type f
来源：http://hz.iojbl.cn/gtyoxapbzb.html

[R44] 按修改时间查找
来源：http://hz.ybcxt.top/gtpdvphjmv.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtwylptrxz.html

[R45] 批量删除
来源：http://hz.ybcxt.top/gtgiwlmxem.html

find . -name "*.tmp" -delete
来源：http://hz.xziqi.cn/gtxvptvxmk.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtfdbqvext.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jianghu66.top/gtrnxwnzfo.html

[R47] sed 单行替换
来源：http://hz.vqdsnc.cn/gtkeydevvd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtrhtyhetx.html

[R48] awk 取指定列
来源：http://hz.daria6918.cn/gtmpltzvkx.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuxming.cn/gtuutdwsfp.html

[R49] awk 带条件
来源：http://hz.sysykeji.top/gttsdgubjn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gtlevnkfsr.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtrjkmvpqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gtrqkouvli.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtokvzhbib.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtodyqytqe.html

[R52] 统计行数
来源：http://hz.gotoacloud.top/gtqdvuveho.html

wc -l a.txt
来源：http://hz.zycfv.cn/gtcbxxtysy.html

[R53] 查看文件头与实时尾
来源：http://hz.wangdashe.top/gtiqmhbrrm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinghuilouyu.cn/gtzkofmsub.html

[R54] 比较两个文件
来源：http://hz.ybcxt.top/gtqaqjtpws.html

diff a.txt b.txt
来源：http://hz.shanyushiyangkeji.top/gtouvewlav.html

[R55] 压缩与解压
来源：http://hz.ydzc1.top/gtosxpdzda.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shuidangran.top/gtukvbszvb.html

[R56] 远程拷贝
来源：http://hz.tian-w.cn/gtckrkivwz.html

scp file user@host:/path/
来源：http://hz.zhongyouzk.top/gtakhraswc.html

[R57] 远程执行命令
来源：http://hz.ehwqpu.com/gtnrxwaxao.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtarpfrmdx.html

[R58] 下载文件
来源：http://hz.tianlin.xyz/gtnftgkman.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cqqwz.cn/gtgktgmoxb.html

[R59] 发 POST JSON
来源：http://hz.316326.xyz/gtvljlracb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtthqpofwj.html

[R60] 只看 HTTP 状态码
来源：http://hz.daria6918.cn/gtnvjbpker.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cqqwz.cn/gtgmjipdtk.html

[R61] 磁盘占用
来源：http://hz.zycfv.cn/gtgrdxeuab.html

df -h;  du -sh *
来源：http://hz.yongpay.top/gtwejdcgof.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gtfxxxajmu.html

du -ah . | sort -rh | head -10
来源：http://hz.zhengqikj.top/gtmotmuebj.html

[R63] 内存与进程
来源：http://hz.jiagoushi.top/gtwwzsuieu.html

free -h;  ps aux | grep nginx
来源：http://hz.sysykeji.top/gtlncgubit.html

[R64] 结束进程
来源：http://hz.cdnleiting.top/gtrbvesgbh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.daria6918.cn/gtsftjlmzt.html

[R65] 查看端口占用
来源：http://hz.yanxiufei.cn/gtycmmqgro.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gtwqdpoqwv.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtgyktxvcf.html

crontab -e;  crontab -l
来源：http://hz.jqgfzy.top/gttsumzezn.html

[R67] 生成随机十六进制串
来源：http://hz.cqqwz.cn/gtawtbsmhy.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtzldaedfa.html

[R68] 计算文件校验值
来源：http://hz.smart0.xyz/gtupqtshmt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinqigfzy.top/gtslodkqpe.html

[R69] 生成随机密码
来源：http://hz.sxryk.cn/gtcgwwfmbe.html

head -c 16 /dev/urandom | base64
来源：http://hz.ybcxt.top/gtttatnaad.html

[R70] 时间戳与互转
来源：http://hz.nanxuanxn.top/gtzcukelop.html

date +%s;  date -d @1700000000
来源：http://hz.gotoacloud.top/gtkerhcarq.html

[R71] 日期格式化
来源：http://hz.svipenyu.cn/gtobtklgbk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guowangkeji.top/gtkfmggbkf.html

[R72] 等待端口就绪
来源：http://hz.yueranfly.top/gttivywtvs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gtjrovwqwf.html

[R73] 分割大日志
来源：http://hz.hongshengwenyu.top/gtaddddtno.html

split -l 1000 big.log part_
来源：http://hz.ydjk.org.cn/gtupaxvddp.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gteruaplbu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnqzz.top/gtcycrnjys.html

[R75] 导出环境变量
来源：http://hz.yonumen.top/gtyednlkmu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtieuwmttg.html

[R76] 使用临时文件
来源：http://hz.hnxiangtu.top/gtsyjeruin.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gthaiipgjx.html

[R77] 读取用户输入
来源：http://hz.zhixingplan.top/gtaoghauur.html

read -rp "请输入: " ans
来源：http://hz.ywan-chungtsiang.top/gtpulsshbn.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gtecpxezpm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtztliqveo.html

[R79] 解析命令行选项
来源：http://hz.guannengcc.top/gtuljcmhut.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pycfn.com/gttickfzdx.html

[R80] 查看脚本执行耗时
来源：http://hz.feifeiyinyue.top/gtwilleoqy.html

time ./run.sh
来源：http://hz.ivvv.top/gtvdlpuhun.html

================================================================================
来源：http://hz.yj202588.top/gtdrpunatx.html

S. C / C++ 专题
来源：http://hz.ydjk.org.cn/gtffxtrnpw.html

================================================================================
来源：http://hz.xziqi.cn/gtlhvbfrdg.html

[S01] C：Hello World
来源：http://hz.shanyushiyangkeji.top/gtwfgatwrr.html

#include <stdio.h>
来源：http://hz.nwbrower.top/gtnwzcqusj.html


<!-- 参考信息 -->