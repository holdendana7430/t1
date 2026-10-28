代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xziqi.cn/gtygwkazgm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.pycfn.com/gtnuyjnkoq.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.birdmap.top/gtpjnegitk.html

[Q42] 连接条件附加过滤
来源：http://hz.jinyuanbaomall.cn/gtvksiifsf.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinqigufen.top/gtjstqpovr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.tian-w.cn/gtlycetlie.html

[Q43] 标量子查询
来源：http://hz.snrcjt.cn/gtpqorcnfp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yuanzhike.top/gttmrxwcxa.html

[Q44] IN 子查询
来源：http://hz.tianlin.xyz/gtsolmgeqr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.316326.xyz/gtpstabven.html

[Q45] EXISTS 判断存在
来源：http://hz.aizwys.cn/gtxyczaptb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hfpthk.cn/gtrlclfbwt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nanxuanxn.top/gtpkjvjcst.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtfwtjzcom.html

[Q47] 与平均值比较
来源：http://hz.yj20258.top/gtlvipxbez.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ehwqpu.com/gturkdkwsi.html

[Q48] CTE 公用表表达式
来源：http://hz.iojbl.cn/gtudxjiiqc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.nwbrower.top/gthstyoxkd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.gaohongyu789.top/gtesfraary.html

[Q49] 更新单行
来源：http://hz.daxiang520.top/gtromtyuse.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.nanxuanxn.top/gtfwvmpznf.html

[Q50] 批量更新
来源：http://hz.9152youxi.cn/gtwrjimekv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yanxiufei.cn/gtfwtqvvim.html

[Q51] 用子查询更新
来源：http://hz.smart0.xyz/gtnatyzwgf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shuidangran.top/gtocqftocf.html

[Q52] 删除指定行
来源：http://hz.jqgfzy.top/gtdqcsuwgl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hfpthk.cn/gttosrficb.html

[Q53] 按条件删除
来源：http://hz.xylfe.cn/gtxppmtqng.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.feifeiyinyue.top/gtsyxjmhqg.html

[Q54] 清空表
来源：http://hz.wangdashe.top/gtynylxiag.html

TRUNCATE TABLE logs;
来源：http://hz.52xcode.cn/gtamwyawyt.html

[Q55] 排名（并列占位）
来源：http://hz.c1oappe.top/gtsdkibstv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuanzhike.top/gtoodartli.html

[Q56] 密集排名（并列不占位）
来源：http://hz.snrcjt.cn/gtnrcqvrhp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxuanxn.top/gtnimgukeg.html

[Q57] 行号
来源：http://hz.zycfv.cn/gtdpfvfwvl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.shzxlz.cn/gtqbiqkrno.html

[Q58] 累计求和
来源：http://hz.cheryme.top/gtbylciqni.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zycfv.cn/gtgleqhnxp.html

[Q59] 分组内累计
来源：http://hz.xylfe.cn/gtvpzneyzn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtqbsnbgud.html

[Q60] 取上一行 / 下一行
来源：http://hz.ppjwa.cn/gtbnpcthcy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinyuanbaomall.cn/gtvkxshvqh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhaomingkeji.xyz/gtjirfrsua.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gttkocjhhs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.jinqigfzy.top/gtkfsyldin.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gtnnivjktr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gttkdzzxdd.html

[Q63] 开启事务
来源：http://hz.316326.xyz/gtwnlmavhp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yuxming.cn/gtxciynhql.html

[Q64] 提交事务
来源：http://hz.ppjwa.cn/gtcwgppucs.html

COMMIT;
来源：http://hz.zhiwuduotai.top/gtrzesmmnq.html

[Q65] 回滚事务
来源：http://hz.fengsongda.top/gtmpwumfou.html

ROLLBACK;
来源：http://hz.hywenlv.cn/gtefkakyzg.html

[Q66] 行锁查询
来源：http://hz.gzhubu.top/gtcdfyfruz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinqigufen.top/gtkdfttasc.html

[Q67] 设置隔离级别
来源：http://hz.pycfn.com/gtjubhrntd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shuidangran.top/gtmwfdfzsc.html

[Q68] 保存点
来源：http://hz.sweek.top/gthzayouww.html

SAVEPOINT sp1;
来源：http://hz.havefunace.top/gtgzshtptt.html

ROLLBACK TO sp1;
来源：http://hz.chenzaomai.com/gthlffamww.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtzyqsjksq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gotoacloud.top/gtddxvfcsn.html

[Q70] 更新统计信息
来源：http://hz.hysaishi.cn/gthgnlacro.html

ANALYZE TABLE users;
来源：http://hz.dianchejie.cn/gttntwaezf.html

[Q71] 查看建表语句
来源：http://hz.sysykeji.top/gthhcarxuh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xylfe.cn/gtzjnvnrlf.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtgrxaatne.html

SHOW INDEX FROM users;
来源：http://hz.chenjidiqi.icu/gtzycikfdj.html

[Q73] 查看表状态
来源：http://hz.ydzc1.top/gtqxlmpeij.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhongyouzk.top/gtkbsijsyr.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gtucxoecvd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pengpengdd.cyou/gtonrmoksm.html

[Q75] 日期格式化
来源：http://hz.fengsongda.top/gtcqczghps.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shuidangran.top/gtejdorzkv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hammf.cn/gtretmraso.html

[Q76] 按天统计
来源：http://hz.yj20258888.top/gtxazyqjim.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xylfe.cn/gtmyatuofx.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtiskvvfxp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydzc1.top/gtsdxumrke.html

[Q78] 当前时间
来源：http://hz.pengpengdd.cyou/gtqqobmfns.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sweek.top/gtahaabnvj.html

[Q79] 字符串拼接
来源：http://hz.xuetiantiany.cn/gtsrhmrjie.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtsphvztfp.html

[Q80] 字符串截取
来源：http://hz.yongpay.top/gtcfnwhmsu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gtqrvronrz.html

[Q81] 字符串替换
来源：http://hz.vqdsnc.cn/gtlfmjwktc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shangyingyoupin.top/gtkxiqnhms.html

[Q82] 字符长度与字节长度
来源：http://hz.aizwys.cn/gttejcmhtf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangtech.top/gtetkqilkt.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtjxfynsdb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhixingplan.top/gtkujgehrt.html

[Q84] 去除首尾空格
来源：http://hz.daria6918.cn/gtrjkajpsf.html

SELECT TRIM(name) FROM users;
来源：http://hz.fzhhl.top/gtirfliyhc.html

[Q85] 数值取整
来源：http://hz.guannengcc.top/gtckiszoda.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ivvv.top/gtpqahxvim.html

[Q86] 读取 JSON 字段
来源：http://hz.mhx1999.top/gtanhhifeb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gzhubu.top/gtofpstrch.html

[Q87] JSON 字段做条件
来源：http://hz.shanyushiyangtech.top/gtexeexary.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jiagoushi.top/gtgbjwjnyi.html

[Q88] 行转列（条件聚合）
来源：http://hz.svipenyu.cn/gtzgufncvm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gtujnxrwmj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.tianlin.xyz/gttgaookoh.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtdwnbhuqb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhongyouzk.top/gtecuxdgbl.html

[Q90] 生成序号列
来源：http://hz.svipenyu.cn/gtybqtwrds.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenjidiqi.icu/gtjpdotefq.html

================================================================================
来源：http://hz.zhixingplan.top/gtusrufpkz.html

R. Bash 专题
来源：http://hz.pengpengdd.cyou/gtwhseyzzs.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtsifadajr.html

[R01] shebang 与严格模式
来源：http://hz.chenlongwang.top/gtjurkwsbb.html

#!/usr/bin/env bash
来源：http://hz.zhengqikj.top/gtdoxfhroa.html

set -euo pipefail
来源：http://hz.bjfxy.top/gtyglvnrkp.html

[R02] 变量赋值与使用
来源：http://hz.jlsjyb.cn/gtrnmphpwi.html

name="Tom"; echo "$name"
来源：http://hz.zhiwuduotai.top/gtzgixuryc.html

[R03] 只读变量
来源：http://hz.nanxinkj.top/gtfhobebjm.html

readonly PI=3.14
来源：http://hz.ydjk.org.cn/gtmkzqnzil.html

[R04] 位置参数
来源：http://hz.shanyushiyangkeji.top/gtovocuwhs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shangyingyoupin.top/gtwjaqnfto.html

[R05] 参数默认值
来源：http://hz.cheryme.top/gtiuogappw.html

name="${1:-default}"
来源：http://hz.feifeiyinyue.top/gtqimmkhmj.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtfyjzfllf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xuetiantiany.cn/gtdnbjmjba.html

[R07] if 判断文件
来源：http://hz.jinyuanbaomall.cn/gtnqtxzfry.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydzc1.top/gtrgslttwl.html

[R08] 数值比较
来源：http://hz.sweek.top/gtnkibybqn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.smart0.xyz/gtjhwpkbva.html

[R09] 字符串比较
来源：http://hz.cheryme.top/gtgldiswol.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258888.top/gtpwlpttil.html

[R10] 正则匹配
来源：http://hz.fengsongda.top/gtdfjrdfko.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sxryk.cn/gtckplgspl.html

[R11] case 多分支
来源：http://hz.meibo888.top/gtegxezvjo.html

case "$1" in
来源：http://hz.cucudq.cn/gtigcwbrff.html

start) echo "启动" ;;
来源：http://hz.hfpthk.cn/gtzrgexqzg.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangtech.top/gtwwusfuin.html

*)     echo "未知命令" ;;
来源：http://hz.aibaodan.cn/gtoyvemmyk.html

esac
来源：http://hz.yongpay.top/gtpdicjpju.html

[R12] for 遍历文件
来源：http://hz.snrcjt.cn/gtuyyxzmvm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenzaomai.com/gtxgmyhjbr.html

[R13] for 计数循环
来源：http://hz.hnxiangtu.top/gtupebxwkd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtsmfevorw.html

[R14] C 风格 for
来源：http://hz.mhx1999.top/gtnsubwlny.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yanxiufei.cn/gtmywgiprq.html

[R15] while 逐行读文件
来源：http://hz.zhixingplan.top/gtuxvxtnpw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtunwpnylf.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtkjiueyet.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydzc1.top/gtjaaorlhb.html

[R17] 数组定义与取值
来源：http://hz.jianghu66.top/gteyvgsaex.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtuzbsddyx.html

[R18] 遍历数组
来源：http://hz.nanxinkj.top/gtbrsstqia.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.andypj.xyz/gtjtnalinh.html

[R19] 数组长度
来源：http://hz.fzhhl.top/gtahsusyxp.html

echo "${#arr[@]}"
来源：http://hz.zycfv.cn/gtcbpybzdk.html

[R20] 关联数组（字典）
来源：http://hz.jiagoushi.top/gtdhkbafii.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sufxvd.cn/gthjsebhgt.html

[R21] 字符串长度
来源：http://hz.sweek.top/gtufxxzxbq.html

echo "${#s}"
来源：http://hz.snrcjt.cn/gtdkqtrmkd.html

[R22] 截取子串
来源：http://hz.jiagoushi.top/gtxhlhfjze.html

echo "${s:0:5}"
来源：http://hz.ywan-chungtsiang.top/gthtljxigd.html

[R23] 字符串替换
来源：http://hz.zhongyouzk.top/gtfugrzvbu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gtowktozzz.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gthjkurjmb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aizwys.cn/gtlmairciu.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhixingplan.top/gtxsggnzti.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuetiantiany.cn/gtgnfyahva.html

[R26] 命令替换
来源：http://hz.nanxuanxn.top/gtixikfkab.html

now=$(date +%F); echo "$now"
来源：http://hz.sxryk.cn/gtjholmhpo.html

[R27] 算术展开
来源：http://hz.xziqi.cn/gtlpmcgtgo.html

echo $((1 + 2 * 3))
来源：http://hz.zdqjudy.top/gtqnnouojx.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gttpmgmjtz.html

echo "scale=2; 10/3" | bc
来源：http://hz.cucudq.cn/gtgnbmrcxw.html

[R29] 定义函数
来源：http://hz.jinqigufen.top/gtqlwwkyji.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gtcqmmoqhp.html

[R30] 函数返回状态码
来源：http://hz.yj20258888.top/gtrxlzyqgu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gogol.net.cn/gtopxvoxom.html

[R31] 局部变量
来源：http://hz.yj202588.top/gtopphppjx.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinghuilouyu.cn/gtgyoheqsu.html

[R32] 参数个数校验
来源：http://hz.hfpthk.cn/gtwcipyupj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xinyue.icu/gtzyewijtt.html

[R33] 捕获错误并提示行号
来源：http://hz.zhijiandao.cn/gtoofbazaw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sweek.top/gtbcxkrzls.html

[R34] 退出时清理
来源：http://hz.zhaomingkeji.xyz/gtomocmsyc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gtbuvztbqr.html

[R35] 后台执行并等待
来源：http://hz.316326.xyz/gtltodxqtp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gtaeirkkyw.html

[R36] 并发执行多个任务
来源：http://hz.xziqi.cn/gtclupkuwm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhaomingkeji.xyz/gtklfavcpu.html

[R37] 把输出赋给变量
来源：http://hz.hammf.cn/gtpsxqfrwg.html

files=$(ls -1)
来源：http://hz.jiagoushi.top/gtgpnbcxoc.html

[R38] 管道串联
来源：http://hz.yonumen.top/gtaaczmxlq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xinyue.icu/gtatsqnwrb.html

[R39] 重定向标准输出与错误
来源：http://hz.chenjidiqi.icu/gtyxooiqzk.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtogajchlv.html

[R40] 追加写日志
来源：http://hz.nanxinkj.top/gtcdydbczy.html

echo "log" >> out.log
来源：http://hz.ywan-chungtsiang.top/gtxkooqzev.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gtcpeshvcc.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigufen.top/gtmlivkfjd.html

[R42] 输入重定向
来源：http://hz.yj20258.top/gtmtngwugf.html

wc -l < a.txt
来源：http://hz.xziqi.cn/gtsrrlhjaa.html

[R43] 按名字查找文件
来源：http://hz.jqgufenzy.top/gtknpmbeno.html

find . -name "*.log" -type f
来源：http://hz.jqgufenzy.top/gtajxfsxis.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangkeji.top/gtlpogfqqc.html

find . -mtime -7 -type f
来源：http://hz.yonumen.top/gtyfttewtv.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gticmifwot.html

find . -name "*.tmp" -delete
来源：http://hz.dianchejie.cn/gtbhbwetal.html

[R46] 递归替换文件内容
来源：http://hz.chenjidiqi.icu/gtoeldoddu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ehwqpu.com/gtotufycuy.html

[R47] sed 单行替换
来源：http://hz.zhengqikj.top/gtlysvvplz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zdqjudy.top/gtogzsfmhb.html

[R48] awk 取指定列
来源：http://hz.hysaishi.cn/gtclfgbmdp.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gtvubijffw.html

[R49] awk 带条件
来源：http://hz.0kj1m.cn/gtmgdkymjq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shangyingyoupin.top/gtasokraqe.html

[R50] awk 求和
来源：http://hz.yj202588.top/gtbmxzslrz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ivvv.top/gtrmgymqkd.html

[R51] 排序去重取前几
来源：http://hz.gotoacloud.top/gtutclmjve.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guowangkeji.top/gtgpezfxeo.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtxhrniixp.html

wc -l a.txt
来源：http://hz.shanyushiyangkeji.top/gtvjwehajn.html

[R53] 查看文件头与实时尾
来源：http://hz.zhijiandao.cn/gtyfpviqks.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.iojbl.cn/gtsvhwfyov.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtewvawitl.html

diff a.txt b.txt
来源：http://hz.tianlin.xyz/gtatboftay.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtkxkafmic.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tanke756.top/gtsgytchsa.html

[R56] 远程拷贝
来源：http://hz.cheryme.top/gtrxwbjjak.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gtthijwrgk.html

[R57] 远程执行命令
来源：http://hz.yj202588.top/gtjuhzvqkz.html

ssh user@host 'uptime'
来源：http://hz.xinyue.icu/gtgjmiswal.html

[R58] 下载文件
来源：http://hz.cqqwz.cn/gtnofuilbs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sweek.top/gtffemazdm.html

[R59] 发 POST JSON
来源：http://hz.zhongyouzk.top/gtwnbxoqjy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtbuqgbvlv.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gtqzdicbqa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jyoumei.cn/gtzdepiaia.html

[R61] 磁盘占用
来源：http://hz.yj20258.top/gtsshwvnes.html

df -h;  du -sh *
来源：http://hz.cdnleiting.top/gtmoguqawj.html

[R62] 找最占空间的文件
来源：http://hz.shzxlz.cn/gtuivkmdzu.html

du -ah . | sort -rh | head -10
来源：http://hz.gzhubu.top/gtymnopkws.html

[R63] 内存与进程
来源：http://hz.zhoulong.xyz/gtnmsqzglx.html

free -h;  ps aux | grep nginx
来源：http://hz.tianlin.xyz/gtkohlcwkm.html

[R64] 结束进程
来源：http://hz.kuanghao11.cn/gtylcexxmr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.mhx1999.top/gtkazxtnac.html

[R65] 查看端口占用
来源：http://hz.nanxinkj.top/gtgydsqlfy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ehwqpu.com/gtbwlyyzdo.html

[R66] 定时任务
来源：http://hz.jinyuanbaomall.cn/gtoilezdci.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtgvwyjmfx.html

[R67] 生成随机十六进制串
来源：http://hz.andypj.xyz/gtsoscegip.html

openssl rand -hex 16
来源：http://hz.xziqi.cn/gthhbhuyld.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtvsdjdzlw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangkeji.top/gttzyblepw.html

[R69] 生成随机密码
来源：http://hz.fzhhl.top/gtzwuhasvi.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhongyouzk.top/gtmdhvvkqu.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtudxxnrec.html

date +%s;  date -d @1700000000
来源：http://hz.zycfv.cn/gtipdpxdsg.html

[R71] 日期格式化
来源：http://hz.shangyingyoupin.top/gtubutpdzm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.smart0.xyz/gtgxmtgrrw.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtfuaabyoq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtlgtcjxez.html

[R73] 分割大日志
来源：http://hz.chenlongwang.top/gtppdkmplp.html

split -l 1000 big.log part_
来源：http://hz.fengsongda.top/gtjygqrfrx.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtpibnvshu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtdebmbfxb.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtrxmevjke.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.vqdsnc.cn/gtjxgabezh.html

[R76] 使用临时文件
来源：http://hz.vqdsnc.cn/gttgilomnt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtjnkoaoob.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gtmtieaarb.html

read -rp "请输入: " ans
来源：http://hz.zhoulong.xyz/gtsprqmmya.html

[R78] 交互式菜单
来源：http://hz.jinghuilouyu.cn/gtopxuashn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gogol.net.cn/gtcsofetoo.html

[R79] 解析命令行选项
来源：http://hz.feifeiyinyue.top/gtbntozfye.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pycfn.com/gtknoreart.html

[R80] 查看脚本执行耗时
来源：http://hz.cdnleiting.top/gtccyaqiig.html

time ./run.sh
来源：http://hz.jyoumei.cn/gtwiledkpf.html

================================================================================
来源：http://hz.haohaochexian.top/gtfvjqdlos.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtjpqhytjx.html

================================================================================
来源：http://hz.52xcode.cn/gtptksjgwu.html

[S01] C：Hello World
来源：http://hz.zycfv.cn/gtgwdyyvau.html

#include <stdio.h>
来源：http://hz.yvedp.cn/gthnyhifep.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ehwqpu.com/gtjsykknyt.html

[S02] C：变量与格式化输出
来源：http://hz.shzxlz.cn/gtwmionhkk.html

int a = 10; printf("%d\n", a);
来源：http://hz.aibaodan.cn/gtvwnofnge.html

[S03] C：读入整数
来源：http://hz.birdmap.top/gtqyrzwzaf.html

int x; scanf("%d", &x);
来源：http://hz.jiagoushi.top/gtloacupzc.html

[S04] C：字符串复制
来源：http://hz.hongshengwenyu.top/gtgrybpvmj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtnewfvudd.html

[S05] C：字符串长度
来源：http://hz.hammf.cn/gtwwdcsjle.html

strlen(s)
来源：http://hz.316326.xyz/gtutpprqkn.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gthulcosmr.html

strcmp(a, b) == 0
来源：http://hz.0kj1m.cn/gtzuavqqxc.html

[S07] C：数组遍历求和
来源：http://hz.dianchejie.cn/gtlzexatle.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jlsjyb.cn/gtmezzpsei.html

[S08] C：动态内存分配与释放
来源：http://hz.yanxiufei.cn/gtbvoptqtm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hywenlv.cn/gtzbqtloql.html

[S09] C：结构体定义与初始化
来源：http://hz.sweek.top/gtpkspbhka.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sufxvd.cn/gtjhxiernq.html

[S10] C：指针与解引用
来源：http://hz.aizwys.cn/gtkqwjaiad.html

int *p = &a;  *p = 5;
来源：http://hz.zhixingplan.top/gtdbctxvmo.html

[S11] C：逐行读文件
来源：http://hz.yuxming.cn/gtuvmrnpvo.html


<!-- 参考信息 -->