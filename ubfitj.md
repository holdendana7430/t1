代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.andypj.xyz/gtnoytbgcy.html

[Q32] 分组拼接字符串
来源：http://hz.yj20258.top/gtifkvvkbr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.zhiwuduotai.top/gtgpixwfml.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.pycfn.com/gtvbdktrip.html

[Q33] 多列分组
来源：http://hz.316326.xyz/gtvfjueupz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinyuanbaomall.cn/gtacumieql.html

[Q34] 每组取第一条
来源：http://hz.daria6918.cn/gtxavcnuwm.html

SELECT * FROM (
来源：http://hz.cheryme.top/gtfvfcafbx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yuanzhike.top/gtvavtezad.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtraymrywp.html

[Q35] 内连接
来源：http://hz.ydzc1.top/gtxdudqsby.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.shangyingyoupin.top/gtptyfusvn.html

[Q36] 左连接
来源：http://hz.9152youxi.cn/gttwdrdjde.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.9152youxi.cn/gtzfxuhxxy.html

[Q37] 右连接
来源：http://hz.vqdsnc.cn/gtnjaqhtkn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dashuyun.cn/gtebnjujex.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zycfv.cn/gtzvzkwryn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigufen.top/gtfakiaiwp.html

[Q39] 自连接（查上下级）
来源：http://hz.zhixingplan.top/gtiikxqmgz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.hysaishi.cn/gtkekcnaep.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.hammf.cn/gtunjyuhct.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hnqzz.top/gtgaeunbpw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jiagoushi.top/gtungunapg.html

[Q41] 多表连接
来源：http://hz.hongshengwenyu.top/gtzlldkwqn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.zhijiandao.cn/gtntlxinfe.html

JOIN users u ON u.id = o.user_id
来源：http://hz.iojbl.cn/gtfirvruht.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.9152youxi.cn/gtbhqqwvwg.html

[Q42] 连接条件附加过滤
来源：http://hz.guannengcc.top/gtpccrhelk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.daxiang520.top/gtzofztziu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tianlin.xyz/gtvdfdxnbo.html

[Q43] 标量子查询
来源：http://hz.meibo888.top/gtlnkxpllj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jinghuilouyu.cn/gtqxirsurh.html

[Q44] IN 子查询
来源：http://hz.svipenyu.cn/gtjqdrxnqj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.nanxuanxn.top/gtjsneetgd.html

[Q45] EXISTS 判断存在
来源：http://hz.jinghuilouyu.cn/gtnxgcyozg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.bjfxy.top/gtpqrwmufn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtxeqampxc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.fengsongda.top/gtxysajvkc.html

[Q47] 与平均值比较
来源：http://hz.jlsjyb.cn/gtmdulolou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtdlesyxlf.html

[Q48] CTE 公用表表达式
来源：http://hz.yj20258.top/gtmguhtkth.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.yj20258888.top/gtompwqjhh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenzaomai.com/gtmwemwolx.html

[Q49] 更新单行
来源：http://hz.tanke756.top/gtrvfupmik.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.c1oappe.top/gttfxrybkq.html

[Q50] 批量更新
来源：http://hz.daria6918.cn/gtabapdjww.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.xingfuxueyuan.xyz/gtgwrikpzn.html

[Q51] 用子查询更新
来源：http://hz.guannengcc.top/gteybocyyl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgufenzy.top/gtxqriztvt.html

[Q52] 删除指定行
来源：http://hz.sweek.top/gtcjgadblo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.dashuyun.cn/gtedlyeeak.html

[Q53] 按条件删除
来源：http://hz.cheryme.top/gtfltcreze.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cdnleiting.top/gtgexfahlb.html

[Q54] 清空表
来源：http://hz.snrcjt.cn/gtgbfjadkp.html

TRUNCATE TABLE logs;
来源：http://hz.zhaomingkeji.xyz/gtimpccxns.html

[Q55] 排名（并列占位）
来源：http://hz.aibaodan.cn/gtawxcqwdl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhiwuduotai.top/gtnfmyqdfi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zycfv.cn/gtgxvctudm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gtfgrgdsmj.html

[Q57] 行号
来源：http://hz.tianlin.xyz/gtzcluysfh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yonumen.top/gtlyjmdxdk.html

[Q58] 累计求和
来源：http://hz.zhongyouzk.top/gtrniorieq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shangyingyoupin.top/gtcugsvogt.html

[Q59] 分组内累计
来源：http://hz.yj20258.top/gtbiqnwcob.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sxryk.cn/gtlctgtepn.html

[Q60] 取上一行 / 下一行
来源：http://hz.gogol.net.cn/gtbpwftfoe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sufxvd.cn/gtxmoogjxz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ywan-chungtsiang.top/gttfatbbtp.html

[Q61] 移动平均
来源：http://hz.zhaomingkeji.xyz/gtaxzkxmbu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenzaomai.com/gtjnbdyuuq.html

[Q62] 分组占比
来源：http://hz.shangyingyoupin.top/gtvcqqzozu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtzbjgfbtq.html

[Q63] 开启事务
来源：http://hz.guannengcc.top/gttoeefwrd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhijiandao.cn/gtaddsyfua.html

[Q64] 提交事务
来源：http://hz.haohaochexian.top/gtapcitmwe.html

COMMIT;
来源：http://hz.gzhubu.top/gtlbevfaiy.html

[Q65] 回滚事务
来源：http://hz.bjfxy.top/gtrjhikxoj.html

ROLLBACK;
来源：http://hz.hammf.cn/gtdhhfjait.html

[Q66] 行锁查询
来源：http://hz.gotoacloud.top/gtibflrctx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cdnleiting.top/gttiuovrsy.html

[Q67] 设置隔离级别
来源：http://hz.ehwqpu.com/gtjpoqzgxr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.sufxvd.cn/gtuislcnia.html

[Q68] 保存点
来源：http://hz.andypj.xyz/gtldvyfmet.html

SAVEPOINT sp1;
来源：http://hz.zycfv.cn/gtahfrcleq.html

ROLLBACK TO sp1;
来源：http://hz.guowangkeji.top/gttkgrqujd.html

[Q69] 查看执行计划
来源：http://hz.gotoacloud.top/gtwrpyhoub.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sxryk.cn/gtseeepieq.html

[Q70] 更新统计信息
来源：http://hz.cashguo.top/gtbnsqzqct.html

ANALYZE TABLE users;
来源：http://hz.jinghuilouyu.cn/gtwiwcekbn.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtjditsazj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gttpzofhbl.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtgiplwkth.html

SHOW INDEX FROM users;
来源：http://hz.shanyushiyangtech.top/gtqkydreil.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangtech.top/gtzirgnwke.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hysaishi.cn/gtxmfqaawb.html

[Q74] 强制使用索引
来源：http://hz.daxiang520.top/gtbtqxmpmj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gtjsesgzxu.html

[Q75] 日期格式化
来源：http://hz.jqgufenzy.top/gtkmsrxhya.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sysykeji.top/gtttyammaj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhongyouzk.top/gtewyogtve.html

[Q76] 按天统计
来源：http://hz.nwbrower.top/gtbaawwtey.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtsduusxvc.html

[Q77] 时间加减
来源：http://hz.9152youxi.cn/gtoaunmxzj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hammf.cn/gtxlkosaye.html

[Q78] 当前时间
来源：http://hz.birdmap.top/gtmqnlnpeb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtajrvtpvi.html

[Q79] 字符串拼接
来源：http://hz.guannengcc.top/gtdpquoglh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenlongwang.top/gtoesjipqd.html

[Q80] 字符串截取
来源：http://hz.yangfankeji.com/gtdrvbbcrc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigfzy.top/gtgfjpvgww.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtpyxsfxav.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydzc1.top/gtmxifenat.html

[Q82] 字符长度与字节长度
来源：http://hz.cdnleiting.top/gtftbneqgy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.sufxvd.cn/gtmcusedoe.html

[Q83] 大小写转换
来源：http://hz.gotoacloud.top/gtemxmacdz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.tanke756.top/gtasdppvnd.html

[Q84] 去除首尾空格
来源：http://hz.pengpengdd.cyou/gtuiooboph.html

SELECT TRIM(name) FROM users;
来源：http://hz.jiagoushi.top/gtykhqoalo.html

[Q85] 数值取整
来源：http://hz.ppjwa.cn/gtilnwqdwa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pycfn.com/gtosvhmevj.html

[Q86] 读取 JSON 字段
来源：http://hz.iojbl.cn/gteathgzlk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jiagoushi.top/gtoptsbnxc.html

[Q87] JSON 字段做条件
来源：http://hz.sxryk.cn/gtintrmhdo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.vqdsnc.cn/gturkecqcg.html

[Q88] 行转列（条件聚合）
来源：http://hz.dianchejie.cn/gtaoygwdyb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dianchejie.cn/gtcxucnhln.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydzc1.top/gtgrpwzwvv.html

[Q89] 判断表是否存在
来源：http://hz.yj20258.top/gtdxzqyufn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhixingplan.top/gtwqmlswzz.html

[Q90] 生成序号列
来源：http://hz.cashguo.top/gtrqyfbmlj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.c1oappe.top/gtckgsdndr.html

================================================================================
来源：http://hz.jiagoushi.top/gtjbmspeka.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtyiuhggqp.html

================================================================================
来源：http://hz.hfpthk.cn/gtowdczsor.html

[R01] shebang 与严格模式
来源：http://hz.zdqjudy.top/gtfduqkpdj.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtmflvqvuu.html

set -euo pipefail
来源：http://hz.nanxinkj.top/gttmsyzsnm.html

[R02] 变量赋值与使用
来源：http://hz.tianlin.xyz/gtnrpibzzl.html

name="Tom"; echo "$name"
来源：http://hz.chenjidiqi.icu/gtpvbqjbao.html

[R03] 只读变量
来源：http://hz.dianchejie.cn/gtqjaywbeu.html

readonly PI=3.14
来源：http://hz.svipenyu.cn/gtnahkbeoc.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtdorckihd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pycfn.com/gtivrxsrxa.html

[R05] 参数默认值
来源：http://hz.zycfv.cn/gtdmrlehxy.html

name="${1:-default}"
来源：http://hz.sweek.top/gtzwouzebs.html

[R06] 判断命令是否存在
来源：http://hz.sysykeji.top/gtcwuqgsux.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pengpengdd.cyou/gtrkpsgwvv.html

[R07] if 判断文件
来源：http://hz.ehwqpu.com/gttvajdfxx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shuidangran.top/gtijesyfhd.html

[R08] 数值比较
来源：http://hz.sxryk.cn/gtdzeelgiz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gtnokxrdlr.html

[R09] 字符串比较
来源：http://hz.fengsongda.top/gtwbfvacjv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtsdurrmaz.html

[R10] 正则匹配
来源：http://hz.jianghu66.top/gtcoxryhsj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtzpvyseko.html

[R11] case 多分支
来源：http://hz.meibo888.top/gtuxumgyqa.html

case "$1" in
来源：http://hz.gzhubu.top/gtkpdotubj.html

start) echo "启动" ;;
来源：http://hz.9152youxi.cn/gtinehmiqc.html

stop)  echo "停止" ;;
来源：http://hz.fengsongda.top/gtpkrqlcoz.html

*)     echo "未知命令" ;;
来源：http://hz.birdmap.top/gtokyjfzqb.html

esac
来源：http://hz.cucudq.cn/gtzjmgyvne.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangtech.top/gtjgkyuyfn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.9152youxi.cn/gtxuzefibe.html

[R13] for 计数循环
来源：http://hz.shzxlz.cn/gtqgrvjtoy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.wangdashe.top/gtqmxsbjwk.html

[R14] C 风格 for
来源：http://hz.yongpay.top/gtmkoykokb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtkhfwgyal.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gtnlzwbyqq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.birdmap.top/gtexzyyrhe.html

[R16] until 等待条件
来源：http://hz.wangdashe.top/gtgjnofwoz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtatiatxvn.html

[R17] 数组定义与取值
来源：http://hz.feifeiyinyue.top/gtzlhbutws.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pycfn.com/gtqhmcdvgc.html

[R18] 遍历数组
来源：http://hz.jlsjyb.cn/gtdnspzvva.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.snrcjt.cn/gtwbvqbkbo.html

[R19] 数组长度
来源：http://hz.yj202588.top/gtivjkuxkp.html

echo "${#arr[@]}"
来源：http://hz.fzhhl.top/gtxpufykhy.html

[R20] 关联数组（字典）
来源：http://hz.zhiwuduotai.top/gtcceqggkc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yongpay.top/gtmbmxadfn.html

[R21] 字符串长度
来源：http://hz.c1oappe.top/gttupfmotj.html

echo "${#s}"
来源：http://hz.wangdashe.top/gttadhlmqq.html

[R22] 截取子串
来源：http://hz.nanxinkj.top/gtxrslwpbf.html

echo "${s:0:5}"
来源：http://hz.ivvv.top/gttbfdteou.html

[R23] 字符串替换
来源：http://hz.shuidangran.top/gtovflizvt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtesgscojn.html

[R24] 大小写转换
来源：http://hz.yonumen.top/gtoyydsljc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangdashe.top/gtooammtvn.html

[R25] 去后缀 / 去前缀
来源：http://hz.cucudq.cn/gtdqnjcrds.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.52xcode.cn/gthttmzuru.html

[R26] 命令替换
来源：http://hz.9152youxi.cn/gtairnjtlf.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtctqsszxh.html

[R27] 算术展开
来源：http://hz.haohaochexian.top/gtocccpczo.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtsjzhukrr.html

[R28] 浮点运算
来源：http://hz.xuanzx.com/gtomfissit.html

echo "scale=2; 10/3" | bc
来源：http://hz.hysaishi.cn/gtebusucah.html

[R29] 定义函数
来源：http://hz.ydzc1.top/gtpdemgfjg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aizwys.cn/gtcxnbkeda.html

[R30] 函数返回状态码
来源：http://hz.yanxiufei.cn/gtjftnsvay.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtzvrfcvck.html

[R31] 局部变量
来源：http://hz.snrcjt.cn/gtaxbhgsqr.html

f() { local x=1; echo "$x"; }
来源：http://hz.pycfn.com/gteiywlyag.html

[R32] 参数个数校验
来源：http://hz.shuidangran.top/gtighofvky.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtmywfxhlh.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangtech.top/gtoynyzalm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhongyouzk.top/gtjdwbkltg.html

[R34] 退出时清理
来源：http://hz.nwbrower.top/gttqdeuxbh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtxrologcl.html

[R35] 后台执行并等待
来源：http://hz.wangdashe.top/gtzphxyyxj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhijiandao.cn/gtjxnrhbex.html

[R36] 并发执行多个任务
来源：http://hz.yanxiufei.cn/gtpxtahgyz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtaagsrmzz.html

[R37] 把输出赋给变量
来源：http://hz.daxiang520.top/gteephmfxn.html

files=$(ls -1)
来源：http://hz.ydjk.org.cn/gtrbyikeqo.html

[R38] 管道串联
来源：http://hz.yanxiufei.cn/gtdgkhgxde.html

cat a.txt | grep -i error | wc -l
来源：http://hz.smart0.xyz/gtvzbsfcap.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtkckyfgiv.html

cmd > out.log 2>&1
来源：http://hz.wangshuangyany.cn/gtcuqkqhey.html

[R40] 追加写日志
来源：http://hz.ydjk.org.cn/gtxeakrlap.html

echo "log" >> out.log
来源：http://hz.xylfe.cn/gtnbbmszlr.html

[R41] 丢弃输出
来源：http://hz.bjfxy.top/gtkydwondj.html

cmd >/dev/null 2>&1
来源：http://hz.zhijiandao.cn/gtlkwzxehx.html

[R42] 输入重定向
来源：http://hz.yj202588.top/gtengezsnh.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtanvprflo.html

[R43] 按名字查找文件
来源：http://hz.hfpthk.cn/gtwxsnyaga.html

find . -name "*.log" -type f
来源：http://hz.aizwys.cn/gtblhpplwn.html

[R44] 按修改时间查找
来源：http://hz.fengsongda.top/gtapcotqvp.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtdvsfkhls.html

[R45] 批量删除
来源：http://hz.jinyuanbaomall.cn/gtzqckuxsv.html

find . -name "*.tmp" -delete
来源：http://hz.9152youxi.cn/gtftrpbkbc.html

[R46] 递归替换文件内容
来源：http://hz.zdqjudy.top/gtzytufdko.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cashguo.top/gtjcsfalkr.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtwkzoghzp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxinkj.top/gtzbftkwgs.html

[R48] awk 取指定列
来源：http://hz.zhiwuduotai.top/gtujmjvfmc.html

awk '{print $1, $3}' a.txt
来源：http://hz.shzxlz.cn/gtqakzmlxw.html

[R49] awk 带条件
来源：http://hz.haohaochexian.top/gtqknttlgt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnxiangtu.top/gtlauedtqy.html

[R50] awk 求和
来源：http://hz.dianchejie.cn/gtyjdmauds.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtvhysytsk.html

[R51] 排序去重取前几
来源：http://hz.pengpengdd.cyou/gtxjevtkmr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.dashuyun.cn/gtstxeecdz.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtnsaygyyi.html

wc -l a.txt
来源：http://hz.birdmap.top/gtcvoltywj.html

[R53] 查看文件头与实时尾
来源：http://hz.sxryk.cn/gtlldivdjo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.mhx1999.top/gtwmelcdvq.html

[R54] 比较两个文件
来源：http://hz.tanke756.top/gtyfarmojo.html

diff a.txt b.txt
来源：http://hz.316326.xyz/gtgzqxohcm.html

[R55] 压缩与解压
来源：http://hz.birdmap.top/gthnjiojpi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.52xcode.cn/gtnvlekbbg.html

[R56] 远程拷贝
来源：http://hz.gzhubu.top/gtqitwbadx.html

scp file user@host:/path/
来源：http://hz.andypj.xyz/gtraraxfbl.html

[R57] 远程执行命令
来源：http://hz.gogol.net.cn/gtuonyvenl.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gthnrcurdk.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gtpllgpxmd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhiwuduotai.top/gtzhgubzbe.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gteguhfoql.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ppjwa.cn/gtjkoijmyt.html

[R60] 只看 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtkgcakses.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gturrdbegg.html

[R61] 磁盘占用
来源：http://hz.chenjidiqi.icu/gtxnzdfdjp.html

df -h;  du -sh *
来源：http://hz.zdqjudy.top/gtdbkykxus.html

[R62] 找最占空间的文件
来源：http://hz.yonumen.top/gtxrnynzhx.html

du -ah . | sort -rh | head -10
来源：http://hz.zhijiandao.cn/gtfqziudit.html

[R63] 内存与进程
来源：http://hz.nanxuanxn.top/gtnvzaujhv.html

free -h;  ps aux | grep nginx
来源：http://hz.yj202588.top/gtyizunvfa.html

[R64] 结束进程
来源：http://hz.ivvv.top/gthsdzehhu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gtogazrimg.html

[R65] 查看端口占用
来源：http://hz.xingfuxueyuan.xyz/gtyhroliag.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtzlummvas.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gtefflkbuw.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtfxkitcka.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gtxintomnk.html

openssl rand -hex 16
来源：http://hz.bjfxy.top/gtotxdknts.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtzccslfvp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.birdmap.top/gtqzwfiqvd.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtxclqlkgl.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangkeji.top/gtfwlqvbgb.html

[R70] 时间戳与互转
来源：http://hz.jlsjyb.cn/gtrwhitybp.html

date +%s;  date -d @1700000000
来源：http://hz.aizwys.cn/gtqxtzwjxx.html

[R71] 日期格式化
来源：http://hz.aibaodan.cn/gtfzqizcfi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.svipenyu.cn/gtdcejxekt.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gteljjrdcd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shzxlz.cn/gtdynuvkgc.html

[R73] 分割大日志
来源：http://hz.sufxvd.cn/gtxfwlxfvh.html

split -l 1000 big.log part_
来源：http://hz.hammf.cn/gtkrgpotut.html

[R74] 批量重命名
来源：http://hz.zdqjudy.top/gtqrptaikp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigfzy.top/gtribftdyp.html

[R75] 导出环境变量
来源：http://hz.jyoumei.cn/gtcqtivhwe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhongyouzk.top/gtdslcheir.html

[R76] 使用临时文件
来源：http://hz.gzhubu.top/gtqmycllzi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtiynxxwfd.html

[R77] 读取用户输入
来源：http://hz.tanke756.top/gtgaifxyap.html

read -rp "请输入: " ans
来源：http://hz.nwbrower.top/gtdstseiso.html

[R78] 交互式菜单
来源：http://hz.andypj.xyz/gtsdbsamfz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydzc1.top/gtqyfqnunr.html

[R79] 解析命令行选项
来源：http://hz.ivvv.top/gtltwszcca.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gzhubu.top/gtrfvtbdjw.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtljtvjvky.html

time ./run.sh
来源：http://hz.yonumen.top/gtjmlfoirw.html

================================================================================
来源：http://hz.ppjwa.cn/gtbcvxxeql.html


<!-- 参考信息 -->