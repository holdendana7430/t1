代发 wailian999

[Q36] 左连接
来源：http://hz.ehwqpu.com/gtpfuysjmi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.redwolf501.top/gtpnwdcahk.html

[Q37] 右连接
来源：http://hz.tian-w.cn/gtoghcdeka.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.svipenyu.cn/gtnpyniupa.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.fzhhl.top/gtvpqnmgwa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.xingfuxueyuan.xyz/gtujkbcltd.html

[Q39] 自连接（查上下级）
来源：http://hz.cucudq.cn/gtxcbvvlue.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.gogol.net.cn/gtljhazwvo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhijiandao.cn/gteqinifzf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhiwuduotai.top/gtdzyfpgob.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hnqzz.top/gtoaffbfzm.html

[Q41] 多表连接
来源：http://hz.xylfe.cn/gtepssctai.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.smart0.xyz/gtxlxwqvpf.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xylfe.cn/gtqnloubwc.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gtgihjajqi.html

[Q42] 连接条件附加过滤
来源：http://hz.zhengqikj.top/gtftzanxox.html

SELECT u.name, o.amount FROM users u
来源：http://hz.fzhhl.top/gtonjgmjjg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtkrdgbqdr.html

[Q43] 标量子查询
来源：http://hz.vqdsnc.cn/gtisulvigf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.vqdsnc.cn/gtuwywodoj.html

[Q44] IN 子查询
来源：http://hz.wangshuangyany.cn/gtgxubhjwg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.9152youxi.cn/gtftqrevga.html

[Q45] EXISTS 判断存在
来源：http://hz.wangdashe.top/gtoxgepuvb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yueranfly.top/gtfocmjjxq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.52xcode.cn/gtockzyank.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinyuanbaomall.cn/gtcvyrusdu.html

[Q47] 与平均值比较
来源：http://hz.bjfxy.top/gtytuzkbhz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.nanxinkj.top/gtdwbyyyoz.html

[Q48] CTE 公用表表达式
来源：http://hz.aizwys.cn/gtchacykaz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtvdizgkzr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.nanxinkj.top/gtbcwackcq.html

[Q49] 更新单行
来源：http://hz.svipenyu.cn/gtmgdmkeku.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cdnleiting.top/gtnxzwoflu.html

[Q50] 批量更新
来源：http://hz.cheryme.top/gtppddiriu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ydzc1.top/gtdckylahu.html

[Q51] 用子查询更新
来源：http://hz.fzhhl.top/gtjphjjmrs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnxiangtu.top/gtsyvuhyox.html

[Q52] 删除指定行
来源：http://hz.yvedp.cn/gtnpoggpen.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sweek.top/gtewzokums.html

[Q53] 按条件删除
来源：http://hz.hywenlv.cn/gtdvkjhyxd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.andypj.xyz/gtofpjirbo.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtrcqjodou.html

TRUNCATE TABLE logs;
来源：http://hz.zycfv.cn/gtatmcymwb.html

[Q55] 排名（并列占位）
来源：http://hz.9152youxi.cn/gtjxmuyxim.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hongshengwenyu.top/gtswfshakd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.xuanzx.com/gtrbnkfzic.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtgekdvoxh.html

[Q57] 行号
来源：http://hz.quarkkingdee.top/gtsjkychrh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shuidangran.top/gthlacnyod.html

[Q58] 累计求和
来源：http://hz.guowangkeji.top/gtcmfatdgc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.shzxlz.cn/gtljvirhql.html

[Q59] 分组内累计
来源：http://hz.meibo888.top/gtmccdcthw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtjfpmfbsz.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhiwuduotai.top/gtspvmniqv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtjvpulnud.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.xuanzx.com/gtzvfauynt.html

[Q61] 移动平均
来源：http://hz.xinyue.icu/gtafschktr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhongyouzk.top/gtnyfkmfis.html

[Q62] 分组占比
来源：http://hz.dianchejie.cn/gtvyjfequj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cucudq.cn/gtewvuwuck.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtjnixdfii.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtocubbgae.html

[Q64] 提交事务
来源：http://hz.xingfuxueyuan.xyz/gtgyqqfdzu.html

COMMIT;
来源：http://hz.sweek.top/gtzusljrpw.html

[Q65] 回滚事务
来源：http://hz.haohaochexian.top/gttniavpsg.html

ROLLBACK;
来源：http://hz.yuanzhike.top/gtscyxiwpj.html

[Q66] 行锁查询
来源：http://hz.wangshuangyany.cn/gtfcyyotgi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gtzbhcwyqt.html

[Q67] 设置隔离级别
来源：http://hz.xinyue.icu/gtpcucpvxv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuetiantiany.cn/gtfbjddlfq.html

[Q68] 保存点
来源：http://hz.zdqjudy.top/gtnbgrgqcf.html

SAVEPOINT sp1;
来源：http://hz.yanxiufei.cn/gtahkfknoi.html

ROLLBACK TO sp1;
来源：http://hz.gzhubu.top/gtyriqxggi.html

[Q69] 查看执行计划
来源：http://hz.zhaomingkeji.xyz/gtjhpqjndj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hnqzz.top/gtbrqgaudo.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtemcfxqhi.html

ANALYZE TABLE users;
来源：http://hz.guannengcc.top/gttsenrenf.html

[Q71] 查看建表语句
来源：http://hz.gogol.net.cn/gtsfsgptaa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtdkrnnggw.html

[Q72] 查看索引
来源：http://hz.yj20258.top/gtsdfdcjfy.html

SHOW INDEX FROM users;
来源：http://hz.sweek.top/gtdtmqkprc.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtoenikzvd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dianchejie.cn/gtkrgrujkq.html

[Q74] 强制使用索引
来源：http://hz.ydjk.org.cn/gtzpzdxucp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhaomingkeji.xyz/gtxfernopz.html

[Q75] 日期格式化
来源：http://hz.dianchejie.cn/gtuniodydb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangtech.top/gtcpalmsec.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cqqwz.cn/gteduplxmc.html

[Q76] 按天统计
来源：http://hz.hongshengwenyu.top/gtjaderiph.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.wangdashe.top/gtznugletn.html

[Q77] 时间加减
来源：http://hz.0kj1m.cn/gtnlkapoez.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.feifeiyinyue.top/gtmcdjabeu.html

[Q78] 当前时间
来源：http://hz.xinyue.icu/gtpwomrhxc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sufxvd.cn/gtqziwiqeu.html

[Q79] 字符串拼接
来源：http://hz.ybcxt.top/gtwjccylaa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtegongakb.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gtpkqfhies.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gtmruvccvy.html

[Q81] 字符串替换
来源：http://hz.chenzaomai.com/gtcxpyeerc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.feifeiyinyue.top/gtsamcbrhz.html

[Q82] 字符长度与字节长度
来源：http://hz.chenlongwang.top/gtumpqjkkr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.birdmap.top/gthvznmhbb.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gtlrlwsdjg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtsvhdevhu.html

[Q84] 去除首尾空格
来源：http://hz.jyoumei.cn/gtueyzvlto.html

SELECT TRIM(name) FROM users;
来源：http://hz.hysaishi.cn/gtracazggm.html

[Q85] 数值取整
来源：http://hz.bjfxy.top/gtlimdwwqt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tanke756.top/gtbunrpujg.html

[Q86] 读取 JSON 字段
来源：http://hz.jlsjyb.cn/gtkrxsrrlj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gturezthzz.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gtjcmtfwyt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.redwolf501.top/gtlpqyrbfm.html

[Q88] 行转列（条件聚合）
来源：http://hz.jiagoushi.top/gtgbunncij.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.redwolf501.top/gtsvpirlka.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhiwuduotai.top/gtambfeuqh.html

[Q89] 判断表是否存在
来源：http://hz.jiagoushi.top/gtgszbnsaj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.kuanghao11.cn/gtwjxsbmzb.html

[Q90] 生成序号列
来源：http://hz.hongshengwenyu.top/gtxlbhyzss.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jyoumei.cn/gtjjfbosnw.html

================================================================================
来源：http://hz.andypj.xyz/gtigxxhqwn.html

R. Bash 专题
来源：http://hz.chenlongwang.top/gtotbunbwd.html

================================================================================
来源：http://hz.xuanzx.com/gtejndwnbg.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtswfhpbvh.html

#!/usr/bin/env bash
来源：http://hz.aibaodan.cn/gtvxbitkbp.html

set -euo pipefail
来源：http://hz.xylfe.cn/gtdwbderfz.html

[R02] 变量赋值与使用
来源：http://hz.zhiwuduotai.top/gttrepogrf.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gtwprkpvqa.html

[R03] 只读变量
来源：http://hz.snrcjt.cn/gtmwccxdjm.html

readonly PI=3.14
来源：http://hz.sysykeji.top/gtzlnabrhd.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtyccoogxq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hywenlv.cn/gtoacwbfpj.html

[R05] 参数默认值
来源：http://hz.redwolf501.top/gtduaybsrl.html

name="${1:-default}"
来源：http://hz.fengsongda.top/gtcdnkiknu.html

[R06] 判断命令是否存在
来源：http://hz.dianchejie.cn/gtmkaqmnct.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtvxncemhc.html

[R07] if 判断文件
来源：http://hz.ppjwa.cn/gtardyadhh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtlfugcqrz.html

[R08] 数值比较
来源：http://hz.ybcxt.top/gtcfoxhmdk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtdudhknav.html

[R09] 字符串比较
来源：http://hz.yangfankeji.com/gtwtpyluau.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zdqjudy.top/gtuyuffzzt.html

[R10] 正则匹配
来源：http://hz.jlsjyb.cn/gtfhyhlogb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258888.top/gtnjjxslyh.html

[R11] case 多分支
来源：http://hz.ivvv.top/gtotxmuoez.html

case "$1" in
来源：http://hz.snrcjt.cn/gtnkezhuwq.html

start) echo "启动" ;;
来源：http://hz.yanxiufei.cn/gtqvqumngo.html

stop)  echo "停止" ;;
来源：http://hz.yueranfly.top/gtzomvmdit.html

*)     echo "未知命令" ;;
来源：http://hz.chenjidiqi.icu/gtvvvtepff.html

esac
来源：http://hz.meibo888.top/gtkpqbkkot.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtuntggqyv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.wangshuangyany.cn/gtqeipucar.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtmtqagvwo.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gtjcyyocyc.html

[R14] C 风格 for
来源：http://hz.tanke756.top/gtxutabmkr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cqqwz.cn/gtqwkdinjd.html

[R15] while 逐行读文件
来源：http://hz.ivvv.top/gtwncbocpr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxuanxn.top/gttrxngrwx.html

[R16] until 等待条件
来源：http://hz.hnqzz.top/gteawidnjq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj202588.top/gtxaztdcwb.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gtxlbluira.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigufen.top/gtrqcyaehd.html

[R18] 遍历数组
来源：http://hz.andypj.xyz/gtqvczbcui.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gotoacloud.top/gtucxctfyk.html

[R19] 数组长度
来源：http://hz.chenzaomai.com/gtnzawzkee.html

echo "${#arr[@]}"
来源：http://hz.dashuyun.cn/gtlrzhwize.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gtjgbgppoi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gzhubu.top/gtxcrumxke.html

[R21] 字符串长度
来源：http://hz.zhengqikj.top/gtkmebzuio.html

echo "${#s}"
来源：http://hz.yanxiufei.cn/gtjhfezuyu.html

[R22] 截取子串
来源：http://hz.zhaomingkeji.xyz/gtglafhehn.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gttomibkol.html

[R23] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtlmdkrwwz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtrplvdvjc.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtlzcvnwki.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nwbrower.top/gtkgqpkwgj.html

[R25] 去后缀 / 去前缀
来源：http://hz.fzhhl.top/gtsdpgxrrk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtwiidhpps.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtbfjvrjtg.html

now=$(date +%F); echo "$now"
来源：http://hz.havefunace.top/gtfhmwtkwc.html

[R27] 算术展开
来源：http://hz.jiagoushi.top/gtmkvrrsoe.html

echo $((1 + 2 * 3))
来源：http://hz.vqdsnc.cn/gtkeuucpee.html

[R28] 浮点运算
来源：http://hz.guowangkeji.top/gtsydydzzg.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtyrxgukyc.html

[R29] 定义函数
来源：http://hz.aizwys.cn/gtxyszaxbo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cqqwz.cn/gtwnvldduu.html

[R30] 函数返回状态码
来源：http://hz.feifeiyinyue.top/gtzoxxmolm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.daxiang520.top/gthedyjzgr.html

[R31] 局部变量
来源：http://hz.shanyushiyangtech.top/gthwnixdgd.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhiwuduotai.top/gteptisfyn.html

[R32] 参数个数校验
来源：http://hz.sysykeji.top/gthyacksdq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yueranfly.top/gthrmcamdo.html

[R33] 捕获错误并提示行号
来源：http://hz.bjfxy.top/gtqjemkrhv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtrcdmlaus.html

[R34] 退出时清理
来源：http://hz.yangfankeji.com/gtytlcfkst.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtlvpldhjd.html

[R35] 后台执行并等待
来源：http://hz.jqgfzy.top/gtvqprznee.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtybfbfaig.html

[R36] 并发执行多个任务
来源：http://hz.guowangkeji.top/gtceuyraro.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtnoggwdfn.html

[R37] 把输出赋给变量
来源：http://hz.bjfxy.top/gtrmbguxox.html

files=$(ls -1)
来源：http://hz.ydzc1.top/gtwyhyqxar.html

[R38] 管道串联
来源：http://hz.ydzc1.top/gtrslfobqq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxuanxn.top/gtfrbyzrwr.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtwjkzqlwk.html

cmd > out.log 2>&1
来源：http://hz.chenlongwang.top/gttjgsnzgy.html

[R40] 追加写日志
来源：http://hz.smart0.xyz/gtcngqanbn.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gttmaadpkq.html

[R41] 丢弃输出
来源：http://hz.meibo888.top/gtzjacnncm.html

cmd >/dev/null 2>&1
来源：http://hz.feifeiyinyue.top/gtutmulaxy.html

[R42] 输入重定向
来源：http://hz.zhaomingkeji.xyz/gtqqmbipim.html

wc -l < a.txt
来源：http://hz.bjfxy.top/gtetcenmij.html

[R43] 按名字查找文件
来源：http://hz.xingfuxueyuan.xyz/gtktbkwxav.html

find . -name "*.log" -type f
来源：http://hz.cheryme.top/gtgkqkbimh.html

[R44] 按修改时间查找
来源：http://hz.jianghu66.top/gtiisevfvq.html

find . -mtime -7 -type f
来源：http://hz.shuidangran.top/gtopbtqafb.html

[R45] 批量删除
来源：http://hz.hfpthk.cn/gtxdwiprft.html

find . -name "*.tmp" -delete
来源：http://hz.dashuyun.cn/gtfkkfcftd.html

[R46] 递归替换文件内容
来源：http://hz.gogol.net.cn/gtlvnwtpth.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtpyfcmwpt.html

[R47] sed 单行替换
来源：http://hz.tanke756.top/gtnyisoksq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtmrledhex.html

[R48] awk 取指定列
来源：http://hz.daxiang520.top/gtqncnyfsp.html

awk '{print $1, $3}' a.txt
来源：http://hz.wangdashe.top/gtgnkmwbby.html

[R49] awk 带条件
来源：http://hz.gaohongyu789.top/gtolzccdmt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cdnleiting.top/gtmrhziala.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtgvtuygzc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fengsongda.top/gtvodxcsbh.html

[R51] 排序去重取前几
来源：http://hz.quarkkingdee.top/gtezcvbigg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnqzz.top/gtdgjadvht.html

[R52] 统计行数
来源：http://hz.birdmap.top/gtrqgffxrg.html

wc -l a.txt
来源：http://hz.xziqi.cn/gtzooqprhv.html

[R53] 查看文件头与实时尾
来源：http://hz.cqqwz.cn/gtuuomcnui.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigufen.top/gtcqsuebrs.html

[R54] 比较两个文件
来源：http://hz.xuetiantiany.cn/gtkdynalas.html

diff a.txt b.txt
来源：http://hz.nwbrower.top/gtxlnwzjgt.html

[R55] 压缩与解压
来源：http://hz.hammf.cn/gtpyqmdxwk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gtbhixksnk.html

[R56] 远程拷贝
来源：http://hz.cheryme.top/gtmrtakjvu.html

scp file user@host:/path/
来源：http://hz.andypj.xyz/gtegcyaqjo.html

[R57] 远程执行命令
来源：http://hz.jinqigufen.top/gtzycqdmhx.html

ssh user@host 'uptime'
来源：http://hz.jinqigufen.top/gtweintwgl.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtdqqthyuk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hfpthk.cn/gtywlauzdk.html

[R59] 发 POST JSON
来源：http://hz.zhiwuduotai.top/gtdshfbysr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtyijifwrl.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtoyznpjgu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.quarkkingdee.top/gthdgevgcs.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtrchluxgx.html

df -h;  du -sh *
来源：http://hz.hongshengwenyu.top/gtmsulridv.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gtuhdqzdzm.html

du -ah . | sort -rh | head -10
来源：http://hz.fengsongda.top/gtjbszhqjv.html

[R63] 内存与进程
来源：http://hz.yj20258.top/gtxjpdnwvh.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtdopuerbc.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtgmzhajlf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtnipeyndf.html

[R65] 查看端口占用
来源：http://hz.xinyue.icu/gtkjmjdaoi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.havefunace.top/gtstmhdqzc.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gtywylgmmd.html

crontab -e;  crontab -l
来源：http://hz.ivvv.top/gtkujrsira.html

[R67] 生成随机十六进制串
来源：http://hz.yonumen.top/gtojimwuag.html

openssl rand -hex 16
来源：http://hz.zhaomingkeji.xyz/gtqfziyoml.html

[R68] 计算文件校验值
来源：http://hz.redwolf501.top/gtfvbhoggg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.haohaochexian.top/gtyojavmcq.html

[R69] 生成随机密码
来源：http://hz.ehwqpu.com/gteejrgptv.html

head -c 16 /dev/urandom | base64
来源：http://hz.316326.xyz/gtajiapuqp.html

[R70] 时间戳与互转
来源：http://hz.0kj1m.cn/gtbtrlyltw.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtgcybspxr.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtrrvmtjgy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxinkj.top/gtrnlehjan.html

[R72] 等待端口就绪
来源：http://hz.xylfe.cn/gtduyuqxpf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gotoacloud.top/gtgozliqti.html

[R73] 分割大日志
来源：http://hz.meibo888.top/gtxdilhpdh.html

split -l 1000 big.log part_
来源：http://hz.pycfn.com/gthxcdydqw.html

[R74] 批量重命名
来源：http://hz.zhijiandao.cn/gtnrypdhqg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ybcxt.top/gtozwioqcq.html

[R75] 导出环境变量
来源：http://hz.zhixingplan.top/gtpmxwpcma.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.quarkkingdee.top/gtydncyctr.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtcffxrcgm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtrxvhglgh.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gtyjpgnstl.html

read -rp "请输入: " ans
来源：http://hz.gotoacloud.top/gtcbfcsylb.html

[R78] 交互式菜单
来源：http://hz.kuanghao11.cn/gtoxizhmld.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xuanzx.com/gtuzolkqgw.html

[R79] 解析命令行选项
来源：http://hz.gogol.net.cn/gtikrbpbhd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sxryk.cn/gtzsppfhce.html

[R80] 查看脚本执行耗时
来源：http://hz.chenzaomai.com/gtvohruavr.html

time ./run.sh
来源：http://hz.fzhhl.top/gtiznductm.html

================================================================================
来源：http://hz.bjfxy.top/gtxwnuftwh.html

S. C / C++ 专题
来源：http://hz.jqgufenzy.top/gtmrzfwmku.html

================================================================================
来源：http://hz.316326.xyz/gtbsjfpkqb.html

[S01] C：Hello World
来源：http://hz.wangshuangyany.cn/gtusjpoaxx.html

#include <stdio.h>
来源：http://hz.cqqwz.cn/gtirzdbugl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258888.top/gtlaggizhy.html

[S02] C：变量与格式化输出
来源：http://hz.ywan-chungtsiang.top/gtaehprohn.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtuvonczbr.html

[S03] C：读入整数
来源：http://hz.sweek.top/gtqrptlwfp.html

int x; scanf("%d", &x);
来源：http://hz.zhongyouzk.top/gtbgbtdtcu.html

[S04] C：字符串复制
来源：http://hz.xingfuxueyuan.xyz/gtpawzewiy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sufxvd.cn/gtnqogdpwa.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangkeji.top/gtccoboefm.html


<!-- 参考信息 -->