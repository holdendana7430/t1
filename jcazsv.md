代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.guowangkeji.top/gthkyjoqhs.html

JOIN users u ON u.id = o.user_id
来源：http://hz.quarkkingdee.top/gtuchuttkg.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jqgufenzy.top/gtvbexzcfv.html

[Q42] 连接条件附加过滤
来源：http://hz.chenlongwang.top/gtqrkixdic.html

SELECT u.name, o.amount FROM users u
来源：http://hz.redwolf501.top/gtkjmrbnnk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.9152youxi.cn/gtjnhyvwne.html

[Q43] 标量子查询
来源：http://hz.zycfv.cn/gtpnnacklb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.wangshuangyany.cn/gtnhalxvdw.html

[Q44] IN 子查询
来源：http://hz.sxryk.cn/gtisqgtagx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinyuanbaomall.cn/gtihfmgeju.html

[Q45] EXISTS 判断存在
来源：http://hz.fzhhl.top/gtnpxpmkhu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.9152youxi.cn/gthmoxeoaq.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.tian-w.cn/gtzrsgjami.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hnxiangtu.top/gtfukmrrne.html

[Q47] 与平均值比较
来源：http://hz.jinyuanbaomall.cn/gtzpjbwjfb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jinqigfzy.top/gtqwsdnpci.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gtwrztynsu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.andypj.xyz/gtmhrpmwsu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.wangdashe.top/gtyjochqss.html

[Q49] 更新单行
来源：http://hz.nwbrower.top/gtmlrutbdg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shzxlz.cn/gtcqtwywia.html

[Q50] 批量更新
来源：http://hz.fzhhl.top/gtwzzppduz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.fzhhl.top/gtoqpgocxr.html

[Q51] 用子查询更新
来源：http://hz.cqqwz.cn/gtefrfmegb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhengqikj.top/gtwtyzhyze.html

[Q52] 删除指定行
来源：http://hz.hysaishi.cn/gtortjpzmo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gzhubu.top/gtiwedkwfq.html

[Q53] 按条件删除
来源：http://hz.9152youxi.cn/gtibnywlhk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.wangshuangyany.cn/gtczbovngh.html

[Q54] 清空表
来源：http://hz.xylfe.cn/gtogpptjdz.html

TRUNCATE TABLE logs;
来源：http://hz.kuanghao11.cn/gtquiveccl.html

[Q55] 排名（并列占位）
来源：http://hz.daria6918.cn/gtxbuimuoe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.andypj.xyz/gttumhmhte.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258.top/gtihtwmoxp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhaomingkeji.xyz/gtwvvugfvz.html

[Q57] 行号
来源：http://hz.jianghu66.top/gttffjepdx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.vqdsnc.cn/gtdskruhbn.html

[Q58] 累计求和
来源：http://hz.dashuyun.cn/gtwtrtzlta.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.havefunace.top/gthrqodeje.html

[Q59] 分组内累计
来源：http://hz.aibaodan.cn/gtxnffjkan.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yangfankeji.com/gtlqtoadkw.html

[Q60] 取上一行 / 下一行
来源：http://hz.mhx1999.top/gtmhzjwrqi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.svipenyu.cn/gtjdxqcvvm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtsdmoxudf.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtbivlngnj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtcpdzataq.html

[Q62] 分组占比
来源：http://hz.cheryme.top/gtxitxsavk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtjiubsohn.html

[Q63] 开启事务
来源：http://hz.havefunace.top/gtcsobbgys.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.wangdashe.top/gtspwdhvfm.html

[Q64] 提交事务
来源：http://hz.yangfankeji.com/gtdbwpvopf.html

COMMIT;
来源：http://hz.yueranfly.top/gtfbwciaqd.html

[Q65] 回滚事务
来源：http://hz.wangdashe.top/gtguyprjbd.html

ROLLBACK;
来源：http://hz.gzhubu.top/gtbppokbza.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtohitbfzz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.tianlin.xyz/gtfguskaor.html

[Q67] 设置隔离级别
来源：http://hz.jinghuilouyu.cn/gtkppbckgr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenzaomai.com/gtkexvfozj.html

[Q68] 保存点
来源：http://hz.jiagoushi.top/gtknztnwgw.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtdfbvadsc.html

ROLLBACK TO sp1;
来源：http://hz.iojbl.cn/gtbgjpyojo.html

[Q69] 查看执行计划
来源：http://hz.nwbrower.top/gtmysnbpmt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yangfankeji.com/gtmoxunhos.html

[Q70] 更新统计信息
来源：http://hz.hnqzz.top/gthpgvevqb.html

ANALYZE TABLE users;
来源：http://hz.yuxming.cn/gtefjvmwkt.html

[Q71] 查看建表语句
来源：http://hz.chenzaomai.com/gtmtqcppwp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sxryk.cn/gthhisowsr.html

[Q72] 查看索引
来源：http://hz.ivvv.top/gtqdfcbjxc.html

SHOW INDEX FROM users;
来源：http://hz.haohaochexian.top/gtsnklatqg.html

[Q73] 查看表状态
来源：http://hz.pengpengdd.cyou/gtskjeybzt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yj20258.top/gtankilfxj.html

[Q74] 强制使用索引
来源：http://hz.hywenlv.cn/gtcaubfavg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhengqikj.top/gtuqzlwces.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtwtetsvbq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtnwmzspgd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtztnhxtmw.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtniwrtroi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tianlin.xyz/gtopukblzq.html

[Q77] 时间加减
来源：http://hz.svipenyu.cn/gtbfvduinx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinyuanbaomall.cn/gtczokzfuf.html

[Q78] 当前时间
来源：http://hz.hammf.cn/gtadafulup.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jlsjyb.cn/gtglpuifyi.html

[Q79] 字符串拼接
来源：http://hz.jlsjyb.cn/gtuhxohdwz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tian-w.cn/gtawmvedvh.html

[Q80] 字符串截取
来源：http://hz.bjfxy.top/gttosalhxk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cqqwz.cn/gthwqeeuld.html

[Q81] 字符串替换
来源：http://hz.yongpay.top/gtotfcopuj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ywan-chungtsiang.top/gtjspulstt.html

[Q82] 字符长度与字节长度
来源：http://hz.yueranfly.top/gtdgwuzowt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigufen.top/gtcbukmyde.html

[Q83] 大小写转换
来源：http://hz.ybcxt.top/gtvkqlkzzl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtznwhmjzm.html

[Q84] 去除首尾空格
来源：http://hz.yj20258888.top/gtnxudddqf.html

SELECT TRIM(name) FROM users;
来源：http://hz.redwolf501.top/gtcgdyseyg.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtpxlqieqj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtefdzuyaj.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtcqfomvek.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gotoacloud.top/gtrgxjququ.html

[Q87] JSON 字段做条件
来源：http://hz.chenlongwang.top/gttfcmnwqj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.52xcode.cn/gtujmhqjmq.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtyvpjkplq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pengpengdd.cyou/gtovcsmcmj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jyoumei.cn/gtuglwtbkf.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtdnbwwnlh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sufxvd.cn/gtlfrwudll.html

[Q90] 生成序号列
来源：http://hz.sysykeji.top/gttvzjukmb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ehwqpu.com/gtcglfgemj.html

================================================================================
来源：http://hz.dianchejie.cn/gtghvvltnu.html

R. Bash 专题
来源：http://hz.zhoulong.xyz/gtxocjbrwb.html

================================================================================
来源：http://hz.yj20258888.top/gtpyxrdauq.html

[R01] shebang 与严格模式
来源：http://hz.hongshengwenyu.top/gthmitcbig.html

#!/usr/bin/env bash
来源：http://hz.c1oappe.top/gtwbtsohvx.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtkrraxzwt.html

[R02] 变量赋值与使用
来源：http://hz.zycfv.cn/gtczhjckii.html

name="Tom"; echo "$name"
来源：http://hz.dianchejie.cn/gtcojgmmiy.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtptkaiufz.html

readonly PI=3.14
来源：http://hz.smart0.xyz/gtebzmfekg.html

[R04] 位置参数
来源：http://hz.shangyingyoupin.top/gtbvirdvhn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yvedp.cn/gtvagwxppk.html

[R05] 参数默认值
来源：http://hz.cdnleiting.top/gtmgiiiaax.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtsrmdqvqh.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangkeji.top/gtolturonv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guannengcc.top/gtthhnfovt.html

[R07] if 判断文件
来源：http://hz.shangyingyoupin.top/gtzyryidag.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daxiang520.top/gtywtziqwm.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtfthhpipe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daria6918.cn/gtswbdmckw.html

[R09] 字符串比较
来源：http://hz.ehwqpu.com/gtsamldlpl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtvxenstrl.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtwsszkdgx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.52xcode.cn/gtvixelpsm.html

[R11] case 多分支
来源：http://hz.zhijiandao.cn/gtshsodyar.html

case "$1" in
来源：http://hz.dianchejie.cn/gtmokhwnst.html

start) echo "启动" ;;
来源：http://hz.tian-w.cn/gtcwjpueen.html

stop)  echo "停止" ;;
来源：http://hz.hfpthk.cn/gtblbwnruk.html

*)     echo "未知命令" ;;
来源：http://hz.xylfe.cn/gtizsnczel.html

esac
来源：http://hz.zdqjudy.top/gtsbwfxfcw.html

[R12] for 遍历文件
来源：http://hz.cucudq.cn/gttzoyflic.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhiwuduotai.top/gtutagoiix.html

[R13] for 计数循环
来源：http://hz.0kj1m.cn/gtipooxulp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxinkj.top/gtqlrefprx.html

[R14] C 风格 for
来源：http://hz.hammf.cn/gtmmfowjwq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yongpay.top/gtvcdcojjr.html

[R15] while 逐行读文件
来源：http://hz.cdnleiting.top/gtzjhjmkqa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sweek.top/gtlcyrebjh.html

[R16] until 等待条件
来源：http://hz.cashguo.top/gtgyhznctv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fzhhl.top/gtyjlbuulv.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtikzndldk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.fzhhl.top/gtfeiotglx.html

[R18] 遍历数组
来源：http://hz.9152youxi.cn/gtjbduqndr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cucudq.cn/gtvjhfvrzx.html

[R19] 数组长度
来源：http://hz.sxryk.cn/gtvkoktorz.html

echo "${#arr[@]}"
来源：http://hz.jianghu66.top/gtjkzndina.html

[R20] 关联数组（字典）
来源：http://hz.316326.xyz/gthidpzolb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuanzhike.top/gtgmlacbpw.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtrctjyvvc.html

echo "${#s}"
来源：http://hz.nanxinkj.top/gtgwobdaqs.html

[R22] 截取子串
来源：http://hz.mhx1999.top/gtuxheudrb.html

echo "${s:0:5}"
来源：http://hz.jianghu66.top/gtsgksbvkk.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtmgrubolb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenzaomai.com/gtwkmuisgc.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gttleyjrdv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cashguo.top/gtyrebpptf.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhaomingkeji.xyz/gtnhgjjwhd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtyjuxqwhy.html

[R26] 命令替换
来源：http://hz.snrcjt.cn/gtpusausgp.html

now=$(date +%F); echo "$now"
来源：http://hz.sysykeji.top/gtiqxfsrfe.html

[R27] 算术展开
来源：http://hz.ivvv.top/gtkxoiffrz.html

echo $((1 + 2 * 3))
来源：http://hz.quarkkingdee.top/gtmubqfqnw.html

[R28] 浮点运算
来源：http://hz.haohaochexian.top/gtkcesrpil.html

echo "scale=2; 10/3" | bc
来源：http://hz.c1oappe.top/gtqurhtmbn.html

[R29] 定义函数
来源：http://hz.birdmap.top/gtzcoitinz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuanzx.com/gtwgbsywdz.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtknliyesr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sxryk.cn/gtanuxysis.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtvcxnvyam.html

f() { local x=1; echo "$x"; }
来源：http://hz.pengpengdd.cyou/gtaiowdtft.html

[R32] 参数个数校验
来源：http://hz.sxryk.cn/gtjxwjxriw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtwiqaqkst.html

[R33] 捕获错误并提示行号
来源：http://hz.gogol.net.cn/gtkvghswmc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gtkmxwqlgd.html

[R34] 退出时清理
来源：http://hz.zhongyouzk.top/gtcuezvbqy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtdludovtn.html

[R35] 后台执行并等待
来源：http://hz.yj202588.top/gtzjqrodvl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnxiangtu.top/gtyxhapzis.html

[R36] 并发执行多个任务
来源：http://hz.jqgufenzy.top/gtvgeehxbn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.andypj.xyz/gtvnsalzqh.html

[R37] 把输出赋给变量
来源：http://hz.jqgfzy.top/gtydefpdvl.html

files=$(ls -1)
来源：http://hz.fzhhl.top/gttviolxgb.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtnlxqvicb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dianchejie.cn/gtncleqyoe.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258888.top/gtmgxoynph.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gtuvqszhjx.html

[R40] 追加写日志
来源：http://hz.cheryme.top/gttjtzqbtd.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtsjibkqyb.html

[R41] 丢弃输出
来源：http://hz.yuxming.cn/gtnsweoftf.html

cmd >/dev/null 2>&1
来源：http://hz.ehwqpu.com/gtclblsmpm.html

[R42] 输入重定向
来源：http://hz.ydzc1.top/gtabgtqhvc.html

wc -l < a.txt
来源：http://hz.hysaishi.cn/gtgovujoxp.html

[R43] 按名字查找文件
来源：http://hz.chenzaomai.com/gtsfilfduu.html

find . -name "*.log" -type f
来源：http://hz.wangdashe.top/gtggzrdvje.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtvvwdmude.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtnumuyyjl.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtvltidvil.html

find . -name "*.tmp" -delete
来源：http://hz.zhixingplan.top/gtrxccgzti.html

[R46] 递归替换文件内容
来源：http://hz.ydzc1.top/gtaptntfos.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtchvktmmb.html

[R47] sed 单行替换
来源：http://hz.snrcjt.cn/gtacrwkoaj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigfzy.top/gtuowakncc.html

[R48] awk 取指定列
来源：http://hz.guannengcc.top/gtxbqshryk.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhoulong.xyz/gthpktyzvg.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtrdgddffk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.andypj.xyz/gtnkfybhgf.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtsypnjale.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gtjyoutaeo.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtdmhfirbh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ybcxt.top/gtowmcpewv.html

[R52] 统计行数
来源：http://hz.shanyushiyangtech.top/gtbuwjhltv.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gtiepvtjmv.html

[R53] 查看文件头与实时尾
来源：http://hz.svipenyu.cn/gtsokhdnpt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtrqznjaht.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangkeji.top/gtsjeflimx.html

diff a.txt b.txt
来源：http://hz.xinyue.icu/gtqajeypjo.html

[R55] 压缩与解压
来源：http://hz.gzhubu.top/gtczvnrdmi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhengqikj.top/gtdbreshda.html

[R56] 远程拷贝
来源：http://hz.chenzaomai.com/gtgbhcuwkl.html

scp file user@host:/path/
来源：http://hz.quarkkingdee.top/gtquqdfpdx.html

[R57] 远程执行命令
来源：http://hz.hnxiangtu.top/gtdilwpltu.html

ssh user@host 'uptime'
来源：http://hz.fzhhl.top/gtnaccmlbc.html

[R58] 下载文件
来源：http://hz.yj20258.top/gtgynhqaod.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gtlylklhcn.html

[R59] 发 POST JSON
来源：http://hz.daria6918.cn/gtfocceyjk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhaomingkeji.xyz/gtdifdclke.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtwluzmubi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtouiokmkg.html

[R61] 磁盘占用
来源：http://hz.xziqi.cn/gtpyuwypmj.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtbezdsckm.html

[R62] 找最占空间的文件
来源：http://hz.hammf.cn/gttmnlimlt.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gteextfazm.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtuplrwuri.html

free -h;  ps aux | grep nginx
来源：http://hz.yonumen.top/gtkcjqdxbj.html

[R64] 结束进程
来源：http://hz.ppjwa.cn/gtbryopsyn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xylfe.cn/gtzjhkzrgb.html

[R65] 查看端口占用
来源：http://hz.xinyue.icu/gtalgzcddz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj202588.top/gtxrvylosi.html

[R66] 定时任务
来源：http://hz.fengsongda.top/gtpkotlolc.html

crontab -e;  crontab -l
来源：http://hz.ywan-chungtsiang.top/gtsfugpjdy.html

[R67] 生成随机十六进制串
来源：http://hz.ppjwa.cn/gtaliqlywi.html

openssl rand -hex 16
来源：http://hz.yueranfly.top/gtrijthveo.html

[R68] 计算文件校验值
来源：http://hz.bjfxy.top/gtiiebfagd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtadddaoan.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gtauqmzeqh.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenjidiqi.icu/gtekxfnruw.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtaflhiukv.html

date +%s;  date -d @1700000000
来源：http://hz.zhixingplan.top/gtkhdawfjn.html

[R71] 日期格式化
来源：http://hz.shzxlz.cn/gtzfbezjrx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yangfankeji.com/gthnjpepoh.html

[R72] 等待端口就绪
来源：http://hz.yuanzhike.top/gtqngeohnx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigfzy.top/gtqqqxdoqo.html

[R73] 分割大日志
来源：http://hz.cdnleiting.top/gtcvbpdebk.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gthyvbmvww.html

[R74] 批量重命名
来源：http://hz.jianghu66.top/gtrswkntdx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shuidangran.top/gtkydfsyyc.html

[R75] 导出环境变量
来源：http://hz.pengpengdd.cyou/gtfxdkzufc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtubfyaxfy.html

[R76] 使用临时文件
来源：http://hz.52xcode.cn/gttszpzihh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtehiojvoq.html

[R77] 读取用户输入
来源：http://hz.hfpthk.cn/gtncfmehmj.html

read -rp "请输入: " ans
来源：http://hz.cashguo.top/gtvjoyadrg.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gtjmeyrufp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangshuangyany.cn/gtxadwwnmr.html

[R79] 解析命令行选项
来源：http://hz.dianchejie.cn/gtxgfhzlbu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtdmeztast.html

[R80] 查看脚本执行耗时
来源：http://hz.ybcxt.top/gtdeoysbuz.html

time ./run.sh
来源：http://hz.jyoumei.cn/gtaauxjtkw.html

================================================================================
来源：http://hz.chenzaomai.com/gttcnjnixs.html

S. C / C++ 专题
来源：http://hz.guowangkeji.top/gtrwiikuys.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxetcwuxi.html

[S01] C：Hello World
来源：http://hz.cucudq.cn/gtrdbzxuus.html

#include <stdio.h>
来源：http://hz.smart0.xyz/gtwxriprfx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigfzy.top/gtrmntckpv.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtxkzsgxmw.html

int a = 10; printf("%d\n", a);
来源：http://hz.tanke756.top/gtxpfixsoe.html

[S03] C：读入整数
来源：http://hz.daria6918.cn/gtbtzzvaii.html

int x; scanf("%d", &x);
来源：http://hz.hammf.cn/gtuamfffhp.html

[S04] C：字符串复制
来源：http://hz.xziqi.cn/gtppgnqphp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yanxiufei.cn/gthrzwshoi.html

[S05] C：字符串长度
来源：http://hz.guannengcc.top/gtefhqxzti.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtsoxdhuap.html

[S06] C：字符串比较
来源：http://hz.bjfxy.top/gtibtyanev.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gtycjkqysy.html

[S07] C：数组遍历求和
来源：http://hz.hywenlv.cn/gtxlarsxbw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtnjtcphiu.html

[S08] C：动态内存分配与释放
来源：http://hz.xingfuxueyuan.xyz/gtngikexrf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shzxlz.cn/gtmbruhncg.html

[S09] C：结构体定义与初始化
来源：http://hz.ybcxt.top/gtdhwmhjxr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gtmurypaty.html

[S10] C：指针与解引用
来源：http://hz.quarkkingdee.top/gtbjanxqgh.html

int *p = &a;  *p = 5;
来源：http://hz.xziqi.cn/gtlnpsapou.html

[S11] C：逐行读文件
来源：http://hz.daxiang520.top/gthkfneyqu.html


<!-- 参考信息 -->