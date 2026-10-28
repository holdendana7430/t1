代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.shanyushiyangtech.top/gtzisjjdkn.html

[Q32] 分组拼接字符串
来源：http://hz.jqgufenzy.top/gtckanovvm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.fzhhl.top/gtwhwilidu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.316326.xyz/gtuleavufu.html

[Q33] 多列分组
来源：http://hz.cdnleiting.top/gtgwmewhyq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.yanxiufei.cn/gtuvpmsnyb.html

[Q34] 每组取第一条
来源：http://hz.cheryme.top/gtavylgtmc.html

SELECT * FROM (
来源：http://hz.birdmap.top/gtfnpedupe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.xziqi.cn/gtddbxuqfa.html

) t WHERE rn = 1;
来源：http://hz.jqgufenzy.top/gtvvkkkqxf.html

[Q35] 内连接
来源：http://hz.cheryme.top/gtxmvkhakw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.iojbl.cn/gtljmxapet.html

[Q36] 左连接
来源：http://hz.meibo888.top/gtfoqyxejy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gttoveiprp.html

[Q37] 右连接
来源：http://hz.c1oappe.top/gtfuqgggfg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xingfuxueyuan.xyz/gteantnsoc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zycfv.cn/gtgggmgxce.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.pengpengdd.cyou/gtacvicdbl.html

[Q39] 自连接（查上下级）
来源：http://hz.yvedp.cn/gtvveeaxrs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tian-w.cn/gtskabjily.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.vqdsnc.cn/gtgxvmlmtl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.shanyushiyangkeji.top/gteveninib.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yangfankeji.com/gtmxkuftjt.html

[Q41] 多表连接
来源：http://hz.gaohongyu789.top/gtkgvbmpzk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnxiangtu.top/gtxtfxlngg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.gaohongyu789.top/gthrsxwktz.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.shangyingyoupin.top/gtlyevwkbl.html

[Q42] 连接条件附加过滤
来源：http://hz.xuanzx.com/gtcbsbshis.html

SELECT u.name, o.amount FROM users u
来源：http://hz.gaohongyu789.top/gtxlccnili.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hfpthk.cn/gtykfcxokt.html

[Q43] 标量子查询
来源：http://hz.52xcode.cn/gttktozrnb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ybcxt.top/gtbdbfoypq.html

[Q44] IN 子查询
来源：http://hz.9152youxi.cn/gtejvhquok.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.zhengqikj.top/gtkjebnffj.html

[Q45] EXISTS 判断存在
来源：http://hz.zdqjudy.top/gtnnrkmvan.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cashguo.top/gtbhgfbpbh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.aizwys.cn/gtnpdhiroo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.pengpengdd.cyou/gtiqhvicbe.html

[Q47] 与平均值比较
来源：http://hz.cqqwz.cn/gtwveyzzky.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.52xcode.cn/gtlhkuchha.html

[Q48] CTE 公用表表达式
来源：http://hz.wangdashe.top/gtpkbmpkjp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.gogol.net.cn/gtowjaqaiv.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.snrcjt.cn/gtolubrhhe.html

[Q49] 更新单行
来源：http://hz.havefunace.top/gtlyytbygx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gogol.net.cn/gtieocrajt.html

[Q50] 批量更新
来源：http://hz.daria6918.cn/gtochmwjuq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yonumen.top/gtpxdnlklz.html

[Q51] 用子查询更新
来源：http://hz.yj202588.top/gtbgrqfbja.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhongyouzk.top/gtavwjwqla.html

[Q52] 删除指定行
来源：http://hz.tianlin.xyz/gtmmlhhfrg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.shzxlz.cn/gtyniqaziu.html

[Q53] 按条件删除
来源：http://hz.xziqi.cn/gtckiebiap.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yvedp.cn/gtwqympdxa.html

[Q54] 清空表
来源：http://hz.yuanzhike.top/gtdjhptfvn.html

TRUNCATE TABLE logs;
来源：http://hz.hywenlv.cn/gtmhqlcoqb.html

[Q55] 排名（并列占位）
来源：http://hz.cashguo.top/gtqqedmxcf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cucudq.cn/gtataxpaga.html

[Q56] 密集排名（并列不占位）
来源：http://hz.havefunace.top/gtcqrltcdu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.wangshuangyany.cn/gtnlyrklgy.html

[Q57] 行号
来源：http://hz.vqdsnc.cn/gtyfnrhmwv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.9152youxi.cn/gtdytgubgf.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtkzfymmpb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hnxiangtu.top/gtttdaczbi.html

[Q59] 分组内累计
来源：http://hz.tianlin.xyz/gtepyhzzsy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.birdmap.top/gtxqgrxafi.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhoulong.xyz/gtmfpklawe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hnqzz.top/gtxedpvfml.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cqqwz.cn/gtpenjtgzh.html

[Q61] 移动平均
来源：http://hz.hammf.cn/gtscgzkvrk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gtqspwhlxs.html

[Q62] 分组占比
来源：http://hz.xylfe.cn/gtktjvsfxq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtlqvkabmo.html

[Q63] 开启事务
来源：http://hz.wangdashe.top/gtxyswzyhw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhiwuduotai.top/gtgzdswtez.html

[Q64] 提交事务
来源：http://hz.ppjwa.cn/gtjwdpwtoc.html

COMMIT;
来源：http://hz.sweek.top/gtqxjpoazt.html

[Q65] 回滚事务
来源：http://hz.ydjk.org.cn/gtirubtgqh.html

ROLLBACK;
来源：http://hz.fengsongda.top/gtaapgsohe.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtsgzckkzz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj202588.top/gteeqgclyr.html

[Q67] 设置隔离级别
来源：http://hz.aibaodan.cn/gtkismgslc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gogol.net.cn/gtitgjkimx.html

[Q68] 保存点
来源：http://hz.yueranfly.top/gtrjkqcami.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gtzqjbhmjo.html

ROLLBACK TO sp1;
来源：http://hz.xingfuxueyuan.xyz/gtflywgiwh.html

[Q69] 查看执行计划
来源：http://hz.hammf.cn/gtlgnfdexp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gttfwobkvd.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gtddvbeawr.html

ANALYZE TABLE users;
来源：http://hz.bjfxy.top/gtukwxuast.html

[Q71] 查看建表语句
来源：http://hz.jinyuanbaomall.cn/gtkxvwyydl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.shzxlz.cn/gtpbegpipa.html

[Q72] 查看索引
来源：http://hz.fzhhl.top/gtamnxfpgk.html

SHOW INDEX FROM users;
来源：http://hz.jinyuanbaomall.cn/gtwsnewzyu.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtdkwvckon.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jinqigfzy.top/gtciesqmqw.html

[Q74] 强制使用索引
来源：http://hz.havefunace.top/gtokvmtngn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pengpengdd.cyou/gtshjgpdcf.html

[Q75] 日期格式化
来源：http://hz.daria6918.cn/gtbtuvfrqt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.kuanghao11.cn/gtggdpbbbh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtfgowiile.html

[Q76] 按天统计
来源：http://hz.xuetiantiany.cn/gtlhlsqujb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.havefunace.top/gtxtxjbkbh.html

[Q77] 时间加减
来源：http://hz.iojbl.cn/gtpxfmwufj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yuxming.cn/gtokeqykku.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtkblhoxbz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xinyue.icu/gtxzdtavbv.html

[Q79] 字符串拼接
来源：http://hz.jlsjyb.cn/gtnngtpmhw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cqqwz.cn/gtuymfincn.html

[Q80] 字符串截取
来源：http://hz.hnqzz.top/gtgdbcnqjk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zycfv.cn/gttcrirwbs.html

[Q81] 字符串替换
来源：http://hz.zhiwuduotai.top/gtcqykchhq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zhiwuduotai.top/gtfzlvtrgm.html

[Q82] 字符长度与字节长度
来源：http://hz.fengsongda.top/gtfmtarxgn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhoulong.xyz/gtootdidgx.html

[Q83] 大小写转换
来源：http://hz.cashguo.top/gtphzmwicj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.fzhhl.top/gteccoziet.html

[Q84] 去除首尾空格
来源：http://hz.316326.xyz/gtpbmwqmjp.html

SELECT TRIM(name) FROM users;
来源：http://hz.bjfxy.top/gtoezunbwd.html

[Q85] 数值取整
来源：http://hz.316326.xyz/gtspfpuhxs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.316326.xyz/gtammashjm.html

[Q86] 读取 JSON 字段
来源：http://hz.shzxlz.cn/gtdvuwlldu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ybcxt.top/gtxrquzfue.html

[Q87] JSON 字段做条件
来源：http://hz.yonumen.top/gtcatkejle.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.0kj1m.cn/gttwnyutno.html

[Q88] 行转列（条件聚合）
来源：http://hz.52xcode.cn/gtfjcrztqa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guowangkeji.top/gtpjcblsbb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gtotikdvnd.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangtech.top/gthadiizvt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ehwqpu.com/gtwydkakjz.html

[Q90] 生成序号列
来源：http://hz.yangfankeji.com/gtpchibayb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhaomingkeji.xyz/gtparenxaz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtpngcleqr.html

R. Bash 专题
来源：http://hz.chenzaomai.com/gtudzrdvsx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtxtwxlmiy.html

[R01] shebang 与严格模式
来源：http://hz.fengsongda.top/gtxfekmlwr.html

#!/usr/bin/env bash
来源：http://hz.hammf.cn/gtaifypbnc.html

set -euo pipefail
来源：http://hz.hongshengwenyu.top/gtxmqjvkqm.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gtwydnbivl.html

name="Tom"; echo "$name"
来源：http://hz.haohaochexian.top/gtzzctnokp.html

[R03] 只读变量
来源：http://hz.hywenlv.cn/gtprmuakme.html

readonly PI=3.14
来源：http://hz.yj202588.top/gtbvomhqfx.html

[R04] 位置参数
来源：http://hz.nanxinkj.top/gtvzrywjkf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.pycfn.com/gtmkqdfwvl.html

[R05] 参数默认值
来源：http://hz.snrcjt.cn/gtxbctnooh.html

name="${1:-default}"
来源：http://hz.smart0.xyz/gtzueomdsl.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtnfjamkbt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hammf.cn/gtgwftmyvl.html

[R07] if 判断文件
来源：http://hz.cheryme.top/gtfvcyogxm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tanke756.top/gtztvahjgj.html

[R08] 数值比较
来源：http://hz.pycfn.com/gtxlbsvbro.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuanzhike.top/gtlvrvkrgw.html

[R09] 字符串比较
来源：http://hz.316326.xyz/gtyqbmevrs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtulsolwwd.html

[R10] 正则匹配
来源：http://hz.fengsongda.top/gtzfyucneo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ywan-chungtsiang.top/gtlonfluol.html

[R11] case 多分支
来源：http://hz.sxryk.cn/gtggujwgxi.html

case "$1" in
来源：http://hz.52xcode.cn/gtezshztro.html

start) echo "启动" ;;
来源：http://hz.zhiwuduotai.top/gtodujfebq.html

stop)  echo "停止" ;;
来源：http://hz.hywenlv.cn/gtldtfcpvi.html

*)     echo "未知命令" ;;
来源：http://hz.316326.xyz/gtjtmfouxy.html

esac
来源：http://hz.zhengqikj.top/gtowsblfes.html

[R12] for 遍历文件
来源：http://hz.cucudq.cn/gtbkqicyuj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dashuyun.cn/gthxzctmql.html

[R13] for 计数循环
来源：http://hz.havefunace.top/gtsbcixmqf.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtpbgkchqi.html

[R14] C 风格 for
来源：http://hz.smart0.xyz/gtggwowzbo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gtuvwfpelo.html

[R15] while 逐行读文件
来源：http://hz.kuanghao11.cn/gtiqykdgir.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtjoejcyfa.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gttlnccudd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.meibo888.top/gtuenyuqwy.html

[R17] 数组定义与取值
来源：http://hz.chenlongwang.top/gtgqocmopm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gtxfrtefiu.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtyzjyjpsq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gaohongyu789.top/gteuvsnyay.html

[R19] 数组长度
来源：http://hz.jinqigfzy.top/gtgiunrgww.html

echo "${#arr[@]}"
来源：http://hz.gzhubu.top/gteandxsim.html

[R20] 关联数组（字典）
来源：http://hz.shuidangran.top/gtedkwjkcr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.52xcode.cn/gtdnqxytdk.html

[R21] 字符串长度
来源：http://hz.wangdashe.top/gtteccalki.html

echo "${#s}"
来源：http://hz.52xcode.cn/gthwfjhqwe.html

[R22] 截取子串
来源：http://hz.andypj.xyz/gtptscclqc.html

echo "${s:0:5}"
来源：http://hz.zhixingplan.top/gtzshmegkd.html

[R23] 字符串替换
来源：http://hz.smart0.xyz/gtruvemvyq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yueranfly.top/gtwvarmdbi.html

[R24] 大小写转换
来源：http://hz.feifeiyinyue.top/gtcjpgvoqk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhengqikj.top/gtlkxzmqtg.html

[R25] 去后缀 / 去前缀
来源：http://hz.daria6918.cn/gtncfmotbn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.gzhubu.top/gthrpmcapa.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtwbjrmnhp.html

now=$(date +%F); echo "$now"
来源：http://hz.sysykeji.top/gtmmsyidbk.html

[R27] 算术展开
来源：http://hz.daxiang520.top/gtnpzyaqto.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtqnfszycc.html

[R28] 浮点运算
来源：http://hz.chenzaomai.com/gtvfzockuq.html

echo "scale=2; 10/3" | bc
来源：http://hz.birdmap.top/gtemozxpag.html

[R29] 定义函数
来源：http://hz.jinghuilouyu.cn/gtubekrrya.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gtsexigubh.html

[R30] 函数返回状态码
来源：http://hz.wangshuangyany.cn/gtvovrccas.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gtqhubwxpv.html

[R31] 局部变量
来源：http://hz.hysaishi.cn/gtatlsmosp.html

f() { local x=1; echo "$x"; }
来源：http://hz.vqdsnc.cn/gtecgvlshd.html

[R32] 参数个数校验
来源：http://hz.52xcode.cn/gtqjgdhtfu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtrnxsqnwd.html

[R33] 捕获错误并提示行号
来源：http://hz.zhoulong.xyz/gtnpxwwlnv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tian-w.cn/gtmedditdq.html

[R34] 退出时清理
来源：http://hz.ywan-chungtsiang.top/gtpkjohdoj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtidngtxxw.html

[R35] 后台执行并等待
来源：http://hz.hammf.cn/gtjqyytrvi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yueranfly.top/gtbopwfbix.html

[R36] 并发执行多个任务
来源：http://hz.dashuyun.cn/gtyomjtlcp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pycfn.com/gtsadjnduw.html

[R37] 把输出赋给变量
来源：http://hz.chenzaomai.com/gtwevssgca.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtarnpjawh.html

[R38] 管道串联
来源：http://hz.yj20258888.top/gtoxkgvlzm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.fengsongda.top/gtvioonnaq.html

[R39] 重定向标准输出与错误
来源：http://hz.dianchejie.cn/gtpzebnyai.html

cmd > out.log 2>&1
来源：http://hz.shuidangran.top/gtsulsgked.html

[R40] 追加写日志
来源：http://hz.shzxlz.cn/gthqlgoeqz.html

echo "log" >> out.log
来源：http://hz.tian-w.cn/gtgdztmeby.html

[R41] 丢弃输出
来源：http://hz.sweek.top/gtzzbwdmbj.html

cmd >/dev/null 2>&1
来源：http://hz.jlsjyb.cn/gtywnnuahm.html

[R42] 输入重定向
来源：http://hz.meibo888.top/gtgmivhvim.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtmnlucqrq.html

[R43] 按名字查找文件
来源：http://hz.kuanghao11.cn/gtbodqluwp.html

find . -name "*.log" -type f
来源：http://hz.xziqi.cn/gthvkegibf.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtuwwisusm.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtvhmpvlbk.html

[R45] 批量删除
来源：http://hz.nanxinkj.top/gtyfpbjdno.html

find . -name "*.tmp" -delete
来源：http://hz.meibo888.top/gteaoeclet.html

[R46] 递归替换文件内容
来源：http://hz.hnxiangtu.top/gtyrhqvzti.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtcotcqrxa.html

[R47] sed 单行替换
来源：http://hz.hysaishi.cn/gtfnstpuvu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtsggptrtn.html

[R48] awk 取指定列
来源：http://hz.zhongyouzk.top/gtxqcsjhbb.html

awk '{print $1, $3}' a.txt
来源：http://hz.cashguo.top/gtxcsjnazl.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gttzcuypcz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jiagoushi.top/gtvxjdygmw.html

[R50] awk 求和
来源：http://hz.yuanzhike.top/gtgbzndtcn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtfcpbohwy.html

[R51] 排序去重取前几
来源：http://hz.sxryk.cn/gtfqitaifq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gtarrpdcie.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtzhvfwocv.html

wc -l a.txt
来源：http://hz.ppjwa.cn/gtlaingext.html

[R53] 查看文件头与实时尾
来源：http://hz.cdnleiting.top/gtmovlthmw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhijiandao.cn/gtouvdcjdm.html

[R54] 比较两个文件
来源：http://hz.chenzaomai.com/gtmtbnvoic.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gtyukgofjo.html

[R55] 压缩与解压
来源：http://hz.snrcjt.cn/gtekgjsgui.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.fzhhl.top/gtoznefjta.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtrsdaqccl.html

scp file user@host:/path/
来源：http://hz.zhongyouzk.top/gtazdfqekn.html

[R57] 远程执行命令
来源：http://hz.ydjk.org.cn/gtvqwlfvef.html

ssh user@host 'uptime'
来源：http://hz.jqgfzy.top/gtahtlqqrf.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtsdefzxyy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gtoeacbvqv.html

[R59] 发 POST JSON
来源：http://hz.zhiwuduotai.top/gtncmnciiv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtqtzbipjb.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtiucsutac.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gtxrogutda.html

[R61] 磁盘占用
来源：http://hz.dianchejie.cn/gtbketolue.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtaveknboc.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gttfjslmul.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtcfrjodhk.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtisydfttt.html

free -h;  ps aux | grep nginx
来源：http://hz.xuanzx.com/gtfieuhprc.html

[R64] 结束进程
来源：http://hz.shangyingyoupin.top/gtgpplkkuf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.meibo888.top/gtsrzktgyu.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtoflfgvpz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ehwqpu.com/gtcukeqdmu.html

[R66] 定时任务
来源：http://hz.birdmap.top/gtheubwgnk.html

crontab -e;  crontab -l
来源：http://hz.jinqigfzy.top/gtkvwmvtdo.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gtlmmqpgxe.html

openssl rand -hex 16
来源：http://hz.hfpthk.cn/gtwrdzeebh.html

[R68] 计算文件校验值
来源：http://hz.sweek.top/gtzzciqzjy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hongshengwenyu.top/gtdfvypmbk.html

[R69] 生成随机密码
来源：http://hz.ywan-chungtsiang.top/gtodujoeny.html

head -c 16 /dev/urandom | base64
来源：http://hz.guannengcc.top/gtbceuutrs.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gtmfalbnhq.html

date +%s;  date -d @1700000000
来源：http://hz.zycfv.cn/gtlpuvzfsm.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gttnoqsjem.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtvhoqguap.html

[R72] 等待端口就绪
来源：http://hz.havefunace.top/gtynetlmlo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.haohaochexian.top/gtdylzumnl.html

[R73] 分割大日志
来源：http://hz.hongshengwenyu.top/gtjsybrurj.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtkdkqofrd.html

[R74] 批量重命名
来源：http://hz.guannengcc.top/gtyjjznthr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtehsyldiy.html

[R75] 导出环境变量
来源：http://hz.svipenyu.cn/gtyyymqhrm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.fengsongda.top/gtgpsjugkg.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtyqxasuba.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtidvxoitj.html

[R77] 读取用户输入
来源：http://hz.xziqi.cn/gtjfxhlgly.html

read -rp "请输入: " ans
来源：http://hz.meibo888.top/gtkcfmxams.html

[R78] 交互式菜单
来源：http://hz.nanxinkj.top/gtxtubevvs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hammf.cn/gtbiktqvjm.html

[R79] 解析命令行选项
来源：http://hz.hfpthk.cn/gtujsloafy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxinkj.top/gtzphuachy.html

[R80] 查看脚本执行耗时
来源：http://hz.smart0.xyz/gtdwffwbds.html

time ./run.sh
来源：http://hz.shanyushiyangtech.top/gtosfmpmef.html

================================================================================
来源：http://hz.sufxvd.cn/gtxdcdorel.html


<!-- 参考信息 -->