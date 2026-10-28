代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yonumen.top/gtceqvkxar.html

[Q32] 分组拼接字符串
来源：http://hz.aizwys.cn/gtbodifraf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinqigufen.top/gtanuqppsx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yuxming.cn/gtmtkyzvdc.html

[Q33] 多列分组
来源：http://hz.zhoulong.xyz/gtutfchfwx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.svipenyu.cn/gtkpadulot.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtmkjkmcuh.html

SELECT * FROM (
来源：http://hz.nwbrower.top/gtwwofxckx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jlsjyb.cn/gtnczxkjhr.html

) t WHERE rn = 1;
来源：http://hz.pycfn.com/gtbwztqggq.html

[Q35] 内连接
来源：http://hz.yj202588.top/gtqhijnhaa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yonumen.top/gtftlchyvl.html

[Q36] 左连接
来源：http://hz.fzhhl.top/gtetouktci.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hnxiangtu.top/gtbdzgjcnr.html

[Q37] 右连接
来源：http://hz.dianchejie.cn/gtlmzodtsx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.yuxming.cn/gttmiuleua.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ydjk.org.cn/gtymwseitj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.cucudq.cn/gtvqrgapdd.html

[Q39] 自连接（查上下级）
来源：http://hz.xziqi.cn/gtrhcilwjk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.aizwys.cn/gtsfzjonrh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.fzhhl.top/gtcpeegjgf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.wangshuangyany.cn/gtzfmgvlem.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.mhx1999.top/gtxhqpbitu.html

[Q41] 多表连接
来源：http://hz.shzxlz.cn/gtujsqzopc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.vqdsnc.cn/gtozmmrsto.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yj202588.top/gtrdyhhulu.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jianghu66.top/gtltahttkv.html

[Q42] 连接条件附加过滤
来源：http://hz.cqqwz.cn/gtkablcvbb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yanxiufei.cn/gtwihessla.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yangfankeji.com/gtqbzyuwne.html

[Q43] 标量子查询
来源：http://hz.cdnleiting.top/gtsntedgkb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.gzhubu.top/gtmwdvxfqt.html

[Q44] IN 子查询
来源：http://hz.gaohongyu789.top/gtxzxxqxbt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtogtqinoi.html

[Q45] EXISTS 判断存在
来源：http://hz.daria6918.cn/gtavcdyqza.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj202588.top/gtzrghbukq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jqgfzy.top/gtqcdlipbc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtevcgnuqf.html

[Q47] 与平均值比较
来源：http://hz.yj20258888.top/gtsposaqgb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zdqjudy.top/gtinhaxekt.html

[Q48] CTE 公用表表达式
来源：http://hz.aizwys.cn/gtemeqkybv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.meibo888.top/gtjlkgknhd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.pengpengdd.cyou/gtgulxunfe.html

[Q49] 更新单行
来源：http://hz.fengsongda.top/gtxfsxjmgo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtquiflpqw.html

[Q50] 批量更新
来源：http://hz.yvedp.cn/gtoutulggk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.havefunace.top/gtkgjqmozl.html

[Q51] 用子查询更新
来源：http://hz.chenzaomai.com/gtshtzpgyo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtaowvazck.html

[Q52] 删除指定行
来源：http://hz.cucudq.cn/gtstnxrnet.html

DELETE FROM users WHERE id = 10;
来源：http://hz.chenlongwang.top/gtwnfjrjeg.html

[Q53] 按条件删除
来源：http://hz.zycfv.cn/gtdumbxobc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.sufxvd.cn/gtmhrqcdja.html

[Q54] 清空表
来源：http://hz.tanke756.top/gtpydviddn.html

TRUNCATE TABLE logs;
来源：http://hz.shuidangran.top/gtztxfezum.html

[Q55] 排名（并列占位）
来源：http://hz.shanyushiyangtech.top/gtonbpucse.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.haohaochexian.top/gtvfpnqivw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sufxvd.cn/gtgkozgamr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xziqi.cn/gtiyhdycey.html

[Q57] 行号
来源：http://hz.gogol.net.cn/gtxqtnxuek.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgfzy.top/gtojxfiqcc.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gtrgqrepuo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hysaishi.cn/gthjetsnew.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtzfaersur.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.cucudq.cn/gtuooxjkvs.html

[Q60] 取上一行 / 下一行
来源：http://hz.hnqzz.top/gtxxfwlnsl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gtnrbpxqob.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yj20258888.top/gtxdpcalgf.html

[Q61] 移动平均
来源：http://hz.kuanghao11.cn/gtpalnqeac.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtomydtgkp.html

[Q62] 分组占比
来源：http://hz.jianghu66.top/gtyuqzpkmv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ybcxt.top/gtasqzzcwf.html

[Q63] 开启事务
来源：http://hz.feifeiyinyue.top/gtzcnuidwm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nwbrower.top/gtyzapnfvg.html

[Q64] 提交事务
来源：http://hz.shanyushiyangkeji.top/gtzpoqlbgt.html

COMMIT;
来源：http://hz.smart0.xyz/gtbisyixjq.html

[Q65] 回滚事务
来源：http://hz.nanxuanxn.top/gtyzbjiutq.html

ROLLBACK;
来源：http://hz.sufxvd.cn/gtdeuzdiqa.html

[Q66] 行锁查询
来源：http://hz.ybcxt.top/gtzcstytnj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.andypj.xyz/gttpzgwgkc.html

[Q67] 设置隔离级别
来源：http://hz.dianchejie.cn/gtkxuhtgmz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xylfe.cn/gtrzoaqbbt.html

[Q68] 保存点
来源：http://hz.tian-w.cn/gtecuvrivn.html

SAVEPOINT sp1;
来源：http://hz.sufxvd.cn/gtqjlfuxpa.html

ROLLBACK TO sp1;
来源：http://hz.ppjwa.cn/gtarsbxehj.html

[Q69] 查看执行计划
来源：http://hz.daria6918.cn/gtycqcesqn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gogol.net.cn/gthlmtsser.html

[Q70] 更新统计信息
来源：http://hz.vqdsnc.cn/gtmamohvjr.html

ANALYZE TABLE users;
来源：http://hz.0kj1m.cn/gtazvdaoza.html

[Q71] 查看建表语句
来源：http://hz.cqqwz.cn/gtdhsmeeso.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtxwokhgnr.html

[Q72] 查看索引
来源：http://hz.ivvv.top/gtmdhekbrp.html

SHOW INDEX FROM users;
来源：http://hz.meibo888.top/gttvjeakmc.html

[Q73] 查看表状态
来源：http://hz.yj20258.top/gtztezzwhf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtdryplxmw.html

[Q74] 强制使用索引
来源：http://hz.shuidangran.top/gtkgvahcrn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtxfghjyjc.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtzcqhwkxj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.redwolf501.top/gtseseynra.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.quarkkingdee.top/gtgzprrswj.html

[Q76] 按天统计
来源：http://hz.yonumen.top/gtcitqbwir.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ehwqpu.com/gthtgdqsmt.html

[Q77] 时间加减
来源：http://hz.sweek.top/gtejovibee.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yonumen.top/gtuejethvh.html

[Q78] 当前时间
来源：http://hz.aizwys.cn/gttggipugb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigfzy.top/gtgbwgnnbr.html

[Q79] 字符串拼接
来源：http://hz.haohaochexian.top/gtqmolsghu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.9152youxi.cn/gtrkhmsdsg.html

[Q80] 字符串截取
来源：http://hz.xinyue.icu/gtlxmghiyz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yanxiufei.cn/gtllweoagl.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtgzestaiu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jiagoushi.top/gtcigqipqv.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258888.top/gthhskcubf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hammf.cn/gtnoypsvsw.html

[Q83] 大小写转换
来源：http://hz.pengpengdd.cyou/gtboacpihw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dashuyun.cn/gtqlesrwui.html

[Q84] 去除首尾空格
来源：http://hz.cheryme.top/gthpfzgqcb.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtoxvyjlah.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gtkyfcavhh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.52xcode.cn/gtcxkgbqpm.html

[Q86] 读取 JSON 字段
来源：http://hz.yanxiufei.cn/gtgfnsnars.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.redwolf501.top/gtojfetdnc.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gtjkquyfvg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cucudq.cn/gtjkfcrbve.html

[Q88] 行转列（条件聚合）
来源：http://hz.tian-w.cn/gtirjjpmzv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hfpthk.cn/gtbeukaeyc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ehwqpu.com/gtopmhamfk.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangkeji.top/gttwzvbjet.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jyoumei.cn/gtwumrfxbp.html

[Q90] 生成序号列
来源：http://hz.nanxinkj.top/gtgwhyxfsh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtxrtxemtz.html

================================================================================
来源：http://hz.ydzc1.top/gtpqrndenb.html

R. Bash 专题
来源：http://hz.jyoumei.cn/gturkhflcn.html

================================================================================
来源：http://hz.gotoacloud.top/gtpqqhtswd.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtuknjpypb.html

#!/usr/bin/env bash
来源：http://hz.feifeiyinyue.top/gtzajjpebm.html

set -euo pipefail
来源：http://hz.hfpthk.cn/gtozlwmacf.html

[R02] 变量赋值与使用
来源：http://hz.guannengcc.top/gtgpwpvapa.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtpzmnssdp.html

[R03] 只读变量
来源：http://hz.yangfankeji.com/gtqzgyqdfg.html

readonly PI=3.14
来源：http://hz.xylfe.cn/gtahzrleve.html

[R04] 位置参数
来源：http://hz.xuanzx.com/gtrxezwcfj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jlsjyb.cn/gtsyzpydlm.html

[R05] 参数默认值
来源：http://hz.chenzaomai.com/gtyzhwtejj.html

name="${1:-default}"
来源：http://hz.fzhhl.top/gtyapvhsoc.html

[R06] 判断命令是否存在
来源：http://hz.hysaishi.cn/gtofmniwyy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gotoacloud.top/gtdvznmyna.html

[R07] if 判断文件
来源：http://hz.shanyushiyangtech.top/gtqjpughdv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigfzy.top/gttrboxlum.html

[R08] 数值比较
来源：http://hz.ppjwa.cn/gtkosfkaeg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgfzy.top/gtguyfzfst.html

[R09] 字符串比较
来源：http://hz.xziqi.cn/gtvdvfdwhq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sysykeji.top/gttsimrtna.html

[R10] 正则匹配
来源：http://hz.sxryk.cn/gtqwbdsnhv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.haohaochexian.top/gtbahmsqkp.html

[R11] case 多分支
来源：http://hz.xinyue.icu/gteyujkoev.html

case "$1" in
来源：http://hz.yongpay.top/gtrazdihbb.html

start) echo "启动" ;;
来源：http://hz.haohaochexian.top/gtfglcdlot.html

stop)  echo "停止" ;;
来源：http://hz.smart0.xyz/gtyqcvljal.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gtvhcgplep.html

esac
来源：http://hz.birdmap.top/gtkfoxlikq.html

[R12] for 遍历文件
来源：http://hz.daria6918.cn/gtnuboqgzv.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shuidangran.top/gtqjolrgmw.html

[R13] for 计数循环
来源：http://hz.hfpthk.cn/gtlwtenlyy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtgcgylsgf.html

[R14] C 风格 for
来源：http://hz.nwbrower.top/gtmbwkyaha.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.snrcjt.cn/gtkepjdepk.html

[R15] while 逐行读文件
来源：http://hz.sweek.top/gtkzdtxnzz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.andypj.xyz/gtejcyzozf.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtstwqpaol.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtmfnuuvww.html

[R17] 数组定义与取值
来源：http://hz.tanke756.top/gtxddttzic.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hnxiangtu.top/gtpvnqxwca.html

[R18] 遍历数组
来源：http://hz.zdqjudy.top/gtqwjttvxu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.haohaochexian.top/gtxvczptmm.html

[R19] 数组长度
来源：http://hz.ivvv.top/gtqpopoyah.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtzxbotgtm.html

[R20] 关联数组（字典）
来源：http://hz.kuanghao11.cn/gtebmxyzni.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.chenzaomai.com/gtcdlbliui.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtgzqbowap.html

echo "${#s}"
来源：http://hz.fengsongda.top/gtdeyiriqa.html

[R22] 截取子串
来源：http://hz.quarkkingdee.top/gtmujsnpme.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gttimuhtpu.html

[R23] 字符串替换
来源：http://hz.ydzc1.top/gtycnygnfg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.feifeiyinyue.top/gtyjwogvxa.html

[R24] 大小写转换
来源：http://hz.redwolf501.top/gtdphhickl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jianghu66.top/gtjwhqnooe.html

[R25] 去后缀 / 去前缀
来源：http://hz.gogol.net.cn/gtnculemgy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtmabptpvo.html

[R26] 命令替换
来源：http://hz.cheryme.top/gtfdfwloix.html

now=$(date +%F); echo "$now"
来源：http://hz.zhoulong.xyz/gtzbuacrxn.html

[R27] 算术展开
来源：http://hz.pengpengdd.cyou/gtclrerbxm.html

echo $((1 + 2 * 3))
来源：http://hz.fengsongda.top/gtisjtbtkq.html

[R28] 浮点运算
来源：http://hz.yangfankeji.com/gtuyyixegm.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtvwkxabjw.html

[R29] 定义函数
来源：http://hz.jqgufenzy.top/gtmahvonsm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxinkj.top/gtrexjprsj.html

[R30] 函数返回状态码
来源：http://hz.sweek.top/gtgzpluvnl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258.top/gtvqelkizb.html

[R31] 局部变量
来源：http://hz.yangfankeji.com/gtcgmyyydm.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangdashe.top/gtpkivkmla.html

[R32] 参数个数校验
来源：http://hz.gaohongyu789.top/gthsemiofd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xinyue.icu/gtlsdajxxy.html

[R33] 捕获错误并提示行号
来源：http://hz.hywenlv.cn/gtbwfjgjif.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxinkj.top/gtxxobmamd.html

[R34] 退出时清理
来源：http://hz.nwbrower.top/gttpuhzhlk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhixingplan.top/gthelxmkbl.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtgmmnyewf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtopeasynz.html

[R36] 并发执行多个任务
来源：http://hz.aizwys.cn/gtspafblkb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cucudq.cn/gtmtspewci.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtiqneteyz.html

files=$(ls -1)
来源：http://hz.snrcjt.cn/gtdcyxajug.html

[R38] 管道串联
来源：http://hz.shanyushiyangtech.top/gtkanodjpd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtzttledai.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgfzy.top/gtxvgkbjyc.html

cmd > out.log 2>&1
来源：http://hz.hfpthk.cn/gtehkxbrcg.html

[R40] 追加写日志
来源：http://hz.yangfankeji.com/gtkgqqtlif.html

echo "log" >> out.log
来源：http://hz.hongshengwenyu.top/gtxjiwdqdj.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtwhsyxmyw.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtakmkvzhe.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gtewoiedlq.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gthirntawt.html

[R43] 按名字查找文件
来源：http://hz.yj202588.top/gtwevscrts.html

find . -name "*.log" -type f
来源：http://hz.shangyingyoupin.top/gtzzszczcs.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtmcjwrkbx.html

find . -mtime -7 -type f
来源：http://hz.jqgfzy.top/gtnuxfrinv.html

[R45] 批量删除
来源：http://hz.zhoulong.xyz/gtjrrcdjas.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtiohfhjqr.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtnjfegiwu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.pycfn.com/gtstmukvwy.html

[R47] sed 单行替换
来源：http://hz.chenzaomai.com/gtmoshevdb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gtgadbjugq.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtwmdcxfob.html

awk '{print $1, $3}' a.txt
来源：http://hz.yueranfly.top/gtzplfmxel.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtacoldksp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hongshengwenyu.top/gtglpteprs.html

[R50] awk 求和
来源：http://hz.zhongyouzk.top/gtcedhjujr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nwbrower.top/gtcryqfxig.html

[R51] 排序去重取前几
来源：http://hz.feifeiyinyue.top/gteicbinxz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangtech.top/gtqsitepoa.html

[R52] 统计行数
来源：http://hz.vqdsnc.cn/gtzbdegxan.html

wc -l a.txt
来源：http://hz.cheryme.top/gtuiaekpgc.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtnvbbwqcv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.fengsongda.top/gtnbwubngu.html

[R54] 比较两个文件
来源：http://hz.wangshuangyany.cn/gtkukfssiq.html

diff a.txt b.txt
来源：http://hz.bjfxy.top/gtyiupvpjf.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtitackblj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinyuanbaomall.cn/gtveaumbsm.html

[R56] 远程拷贝
来源：http://hz.jinqigfzy.top/gtptdxdxlq.html

scp file user@host:/path/
来源：http://hz.sufxvd.cn/gtiyfjrjff.html

[R57] 远程执行命令
来源：http://hz.dashuyun.cn/gtixdqhwbb.html

ssh user@host 'uptime'
来源：http://hz.chenlongwang.top/gtadqbowam.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtramwprjw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.havefunace.top/gtvfsfndxi.html

[R59] 发 POST JSON
来源：http://hz.zhiwuduotai.top/gtrjkixyll.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pengpengdd.cyou/gthvofdoja.html

[R60] 只看 HTTP 状态码
来源：http://hz.jyoumei.cn/gtybnqjgiv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenlongwang.top/gtuycqfxqx.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtmabhorsx.html

df -h;  du -sh *
来源：http://hz.yuanzhike.top/gtjgyebbxk.html

[R62] 找最占空间的文件
来源：http://hz.haohaochexian.top/gtthzqrtyq.html

du -ah . | sort -rh | head -10
来源：http://hz.meibo888.top/gtwgqadvie.html

[R63] 内存与进程
来源：http://hz.meibo888.top/gtfqyklgbr.html

free -h;  ps aux | grep nginx
来源：http://hz.birdmap.top/gtyqigkubf.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtutrajzrx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hysaishi.cn/gtcuwypowp.html

[R65] 查看端口占用
来源：http://hz.xuanzx.com/gtlfarwihh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.nwbrower.top/gtpdhsizmd.html

[R66] 定时任务
来源：http://hz.ivvv.top/gtoiewqojj.html

crontab -e;  crontab -l
来源：http://hz.jyoumei.cn/gtjdhrsvsf.html

[R67] 生成随机十六进制串
来源：http://hz.9152youxi.cn/gtndwtxcfx.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtthpbovkk.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gtzcejmhli.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhaomingkeji.xyz/gtvfpcojiv.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtezluhwsh.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gttvesxoxw.html

[R70] 时间戳与互转
来源：http://hz.haohaochexian.top/gtyxzkayjp.html

date +%s;  date -d @1700000000
来源：http://hz.jiagoushi.top/gtlpygnecu.html

[R71] 日期格式化
来源：http://hz.zhongyouzk.top/gtcabnukit.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zdqjudy.top/gthdiyajfp.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gteyaagxqg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuxming.cn/gtfzttoghi.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtcqsylawn.html

split -l 1000 big.log part_
来源：http://hz.c1oappe.top/gtctseityg.html

[R74] 批量重命名
来源：http://hz.wangdashe.top/gtvrjdhvxi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shzxlz.cn/gtfhtfqalk.html

[R75] 导出环境变量
来源：http://hz.pengpengdd.cyou/gtjrxgxlsg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jlsjyb.cn/gtratlpbxz.html

[R76] 使用临时文件
来源：http://hz.kuanghao11.cn/gtwtzkoxqe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gttubcwenk.html

[R77] 读取用户输入
来源：http://hz.ehwqpu.com/gtgvzliook.html

read -rp "请输入: " ans
来源：http://hz.haohaochexian.top/gtmmwasqcn.html

[R78] 交互式菜单
来源：http://hz.dianchejie.cn/gtkylhxymy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cheryme.top/gtpdeixlkp.html

[R79] 解析命令行选项
来源：http://hz.quarkkingdee.top/gtagfkrtfx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangkeji.top/gtcrdupajc.html

[R80] 查看脚本执行耗时
来源：http://hz.yonumen.top/gtcpndimjo.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtiifghiip.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gthacrkjhv.html


<!-- 参考信息 -->