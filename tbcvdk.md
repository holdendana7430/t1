代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.zhoulong.xyz/gtxpkboist.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jlsjyb.cn/gtzopmzcei.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhoulong.xyz/gtzznvuwah.html

[Q41] 多表连接
来源：http://hz.xuanzx.com/gtahqmuccv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.yvedp.cn/gtbbivbawu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cheryme.top/gtbkforxml.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.fzhhl.top/gtojnuylzx.html

[Q42] 连接条件附加过滤
来源：http://hz.guowangkeji.top/gtqirfnsir.html

SELECT u.name, o.amount FROM users u
来源：http://hz.smart0.xyz/gtrgfoitlu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hfpthk.cn/gtllyiqucy.html

[Q43] 标量子查询
来源：http://hz.havefunace.top/gtsrocvxid.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jiagoushi.top/gttaijwlau.html

[Q44] IN 子查询
来源：http://hz.iojbl.cn/gtnawsbgeh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.guowangkeji.top/gtxxfozlwy.html

[Q45] EXISTS 判断存在
来源：http://hz.chenzaomai.com/gtdsuutsye.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jiagoushi.top/gtoekeqqwi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.vqdsnc.cn/gtqcvfkzqn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ybcxt.top/gtkvjupjxm.html

[Q47] 与平均值比较
来源：http://hz.aibaodan.cn/gtzpgmrzjc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xylfe.cn/gtbbxxzlri.html

[Q48] CTE 公用表表达式
来源：http://hz.xuetiantiany.cn/gtoivpbjgq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.tanke756.top/gtjcriccvt.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ppjwa.cn/gtgpkdvwoj.html

[Q49] 更新单行
来源：http://hz.52xcode.cn/gtkbsizzzd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.yangfankeji.com/gtooogxruw.html

[Q50] 批量更新
来源：http://hz.jlsjyb.cn/gtpzbuvgtq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gzhubu.top/gtpjkdyfqm.html

[Q51] 用子查询更新
来源：http://hz.tian-w.cn/gtmmzjedax.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cashguo.top/gtetadcjsl.html

[Q52] 删除指定行
来源：http://hz.hnqzz.top/gtsbekyijw.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sufxvd.cn/gtcqihpwrs.html

[Q53] 按条件删除
来源：http://hz.iojbl.cn/gtihuqthpr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yueranfly.top/gtzdqnpleg.html

[Q54] 清空表
来源：http://hz.iojbl.cn/gtahudtpme.html

TRUNCATE TABLE logs;
来源：http://hz.havefunace.top/gtcjxcqxgg.html

[Q55] 排名（并列占位）
来源：http://hz.jinghuilouyu.cn/gtwdfahhhr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hywenlv.cn/gtxctkflme.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yanxiufei.cn/gtydsetdvm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.pengpengdd.cyou/gtrjfuaudi.html

[Q57] 行号
来源：http://hz.nanxinkj.top/gtjdqbphla.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.nanxinkj.top/gtmhgdyquh.html

[Q58] 累计求和
来源：http://hz.ppjwa.cn/gtgfsrpvad.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daxiang520.top/gtabiajwtp.html

[Q59] 分组内累计
来源：http://hz.ehwqpu.com/gtkzhxjijk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258.top/gthujnnddl.html

[Q60] 取上一行 / 下一行
来源：http://hz.yanxiufei.cn/gtiqdvbjtb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.havefunace.top/gtuckrqewd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.shanyushiyangtech.top/gtgsavwkyp.html

[Q61] 移动平均
来源：http://hz.cheryme.top/gtieswnnou.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daxiang520.top/gtfrvedzld.html

[Q62] 分组占比
来源：http://hz.c1oappe.top/gtkyqrbmxi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.dianchejie.cn/gtxtiodsbg.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtsdwpiyan.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daxiang520.top/gtatencaqq.html

[Q64] 提交事务
来源：http://hz.havefunace.top/gtzyuazcaw.html

COMMIT;
来源：http://hz.nwbrower.top/gttezovyhs.html

[Q65] 回滚事务
来源：http://hz.c1oappe.top/gtgeuzzdjy.html

ROLLBACK;
来源：http://hz.redwolf501.top/gtkmzakdzn.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtxnnyehmc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hnxiangtu.top/gtesbxkynv.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gtpiiaqnmt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daxiang520.top/gtstcbaoax.html

[Q68] 保存点
来源：http://hz.jqgfzy.top/gtpiakcsxk.html

SAVEPOINT sp1;
来源：http://hz.daria6918.cn/gtmsuqjdjj.html

ROLLBACK TO sp1;
来源：http://hz.nanxuanxn.top/gtmrmekoyg.html

[Q69] 查看执行计划
来源：http://hz.jqgufenzy.top/gtiagumhjl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xziqi.cn/gtqhfsnstc.html

[Q70] 更新统计信息
来源：http://hz.hongshengwenyu.top/gtrxqqpqdm.html

ANALYZE TABLE users;
来源：http://hz.tianlin.xyz/gtigujzvsv.html

[Q71] 查看建表语句
来源：http://hz.jianghu66.top/gtlbkxzcmd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jlsjyb.cn/gtkvoybqru.html

[Q72] 查看索引
来源：http://hz.vqdsnc.cn/gtreaethol.html

SHOW INDEX FROM users;
来源：http://hz.yongpay.top/gtvlmvufwu.html

[Q73] 查看表状态
来源：http://hz.xingfuxueyuan.xyz/gtslcfalxb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xylfe.cn/gtsrhapwsm.html

[Q74] 强制使用索引
来源：http://hz.havefunace.top/gtmnebswvg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gzhubu.top/gtznruxkbd.html

[Q75] 日期格式化
来源：http://hz.yonumen.top/gtyvfclwrt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zdqjudy.top/gtndhrzooz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.redwolf501.top/gtqrqtqijc.html

[Q76] 按天统计
来源：http://hz.birdmap.top/gtrbrtvuqv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gtajzilkzg.html

[Q77] 时间加减
来源：http://hz.nwbrower.top/gtdhomweoi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtdncolfve.html

[Q78] 当前时间
来源：http://hz.yj20258.top/gtphwqfozh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tanke756.top/gtpjryfflt.html

[Q79] 字符串拼接
来源：http://hz.iojbl.cn/gthxhehvcw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.gzhubu.top/gtmcdytrlz.html

[Q80] 字符串截取
来源：http://hz.yvedp.cn/gtzgyqlely.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.iojbl.cn/gtfoehuron.html

[Q81] 字符串替换
来源：http://hz.smart0.xyz/gtndwwmybn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jiagoushi.top/gtmaufcget.html

[Q82] 字符长度与字节长度
来源：http://hz.kuanghao11.cn/gtomcpqqso.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tanke756.top/gtirabaneb.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtcrvuzcog.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jinqigufen.top/gtwnzardtt.html

[Q84] 去除首尾空格
来源：http://hz.fzhhl.top/gtwuheimut.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtwqdinwwb.html

[Q85] 数值取整
来源：http://hz.zhixingplan.top/gtxgxjucfv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gtmfnjmhka.html

[Q86] 读取 JSON 字段
来源：http://hz.jqgufenzy.top/gtpwvqdvrd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydzc1.top/gtvxzdsceu.html

[Q87] JSON 字段做条件
来源：http://hz.hammf.cn/gtijlwrbdb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yueranfly.top/gtkqtxibfw.html

[Q88] 行转列（条件聚合）
来源：http://hz.jiagoushi.top/gtfewkasdm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhiwuduotai.top/gtvatuqxtc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtgrcfdbfk.html

[Q89] 判断表是否存在
来源：http://hz.jiagoushi.top/gtansgxdmy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.52xcode.cn/gtlucvhdfx.html

[Q90] 生成序号列
来源：http://hz.shuidangran.top/gtrahrmaef.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhoulong.xyz/gtpagtbrxf.html

================================================================================
来源：http://hz.ivvv.top/gtogxidjdq.html

R. Bash 专题
来源：http://hz.jqgfzy.top/gtzarzxdrl.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzgeagflf.html

[R01] shebang 与严格模式
来源：http://hz.yangfankeji.com/gtwtuxhzpb.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtrkyqcrsf.html

set -euo pipefail
来源：http://hz.guowangkeji.top/gtewihnewo.html

[R02] 变量赋值与使用
来源：http://hz.yuanzhike.top/gtcmiaamgc.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gttlscomrw.html

[R03] 只读变量
来源：http://hz.ydjk.org.cn/gtcikicddp.html

readonly PI=3.14
来源：http://hz.sweek.top/gtgajaqzyo.html

[R04] 位置参数
来源：http://hz.pengpengdd.cyou/gtkoeitevl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtdwzobjdh.html

[R05] 参数默认值
来源：http://hz.yuanzhike.top/gtkbhlllii.html

name="${1:-default}"
来源：http://hz.aizwys.cn/gtpispvvpc.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gtnpbgnenb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnxiangtu.top/gtpygmqvte.html

[R07] if 判断文件
来源：http://hz.zhoulong.xyz/gtszkedark.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.0kj1m.cn/gteqfmqzzm.html

[R08] 数值比较
来源：http://hz.jianghu66.top/gtahvebxri.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtwkuvitsr.html

[R09] 字符串比较
来源：http://hz.gotoacloud.top/gtwvpdimpj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.316326.xyz/gtuybhrzld.html

[R10] 正则匹配
来源：http://hz.ydzc1.top/gtoqbobpon.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.0kj1m.cn/gtvoslwzpl.html

[R11] case 多分支
来源：http://hz.dashuyun.cn/gtpmdhgiuq.html

case "$1" in
来源：http://hz.gzhubu.top/gtythodzka.html

start) echo "启动" ;;
来源：http://hz.ywan-chungtsiang.top/gtrngofpoq.html

stop)  echo "停止" ;;
来源：http://hz.jiagoushi.top/gtkeqyfaji.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtwfpkqmpc.html

esac
来源：http://hz.zycfv.cn/gtfpnwbqhc.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangkeji.top/gttimfluwq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtoyscqdqm.html

[R13] for 计数循环
来源：http://hz.kuanghao11.cn/gtjafvikbx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtdegewafs.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtdeddzoas.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hammf.cn/gtgmziphne.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtanrtaynp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gtpeqllpeo.html

[R16] until 等待条件
来源：http://hz.zhengqikj.top/gtkrnpcirt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtspgfzamq.html

[R17] 数组定义与取值
来源：http://hz.jqgufenzy.top/gthjdocbhg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydjk.org.cn/gtcpexhtqc.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtqvdbkvfd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.c1oappe.top/gtioibeuog.html

[R19] 数组长度
来源：http://hz.zhongyouzk.top/gtcqjkueyn.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtiueaajva.html

[R20] 关联数组（字典）
来源：http://hz.yuxming.cn/gthvpyvfdt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtbugmglhx.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtrfyslljw.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtpkppnguk.html

[R22] 截取子串
来源：http://hz.yj202588.top/gtttisenxg.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gthximxkvq.html

[R23] 字符串替换
来源：http://hz.gaohongyu789.top/gtjpkdioxf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.316326.xyz/gtsawjfqln.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtgpmjoqrf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtybmagwmh.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtoazvfbez.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gthfuijzsd.html

[R26] 命令替换
来源：http://hz.sweek.top/gtoudumrit.html

now=$(date +%F); echo "$now"
来源：http://hz.bjfxy.top/gtbpahkmgq.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gthzqfaisy.html

echo $((1 + 2 * 3))
来源：http://hz.cdnleiting.top/gtkgvjtqit.html

[R28] 浮点运算
来源：http://hz.cheryme.top/gtaboicdmh.html

echo "scale=2; 10/3" | bc
来源：http://hz.tianlin.xyz/gtrleetgii.html

[R29] 定义函数
来源：http://hz.sweek.top/gtxbvrcfef.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tian-w.cn/gtulisknej.html

[R30] 函数返回状态码
来源：http://hz.tian-w.cn/gtwshjyxvp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtjwaxdynr.html

[R31] 局部变量
来源：http://hz.yueranfly.top/gtddinfwvr.html

f() { local x=1; echo "$x"; }
来源：http://hz.sxryk.cn/gtzorrzbrl.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtvtaiweya.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gtwhewwcsm.html

[R33] 捕获错误并提示行号
来源：http://hz.vqdsnc.cn/gtupompjsl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hysaishi.cn/gtcamvqktm.html

[R34] 退出时清理
来源：http://hz.gotoacloud.top/gtjrnjlqzb.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtfytijklu.html

[R35] 后台执行并等待
来源：http://hz.gotoacloud.top/gtveuxpfhj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhijiandao.cn/gtyrkxuirx.html

[R36] 并发执行多个任务
来源：http://hz.jinqigufen.top/gtdmpwvjkm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yueranfly.top/gtyppmxybv.html

[R37] 把输出赋给变量
来源：http://hz.hammf.cn/gtsqwwvtcg.html

files=$(ls -1)
来源：http://hz.guowangkeji.top/gteavtynki.html

[R38] 管道串联
来源：http://hz.andypj.xyz/gtsqfyqnrx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtmaghqyab.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtfdddzfbp.html

cmd > out.log 2>&1
来源：http://hz.jinghuilouyu.cn/gttuijwkxt.html

[R40] 追加写日志
来源：http://hz.yonumen.top/gtphxqvovi.html

echo "log" >> out.log
来源：http://hz.jlsjyb.cn/gtyttjhhng.html

[R41] 丢弃输出
来源：http://hz.nanxuanxn.top/gtiwjsiusa.html

cmd >/dev/null 2>&1
来源：http://hz.yangfankeji.com/gttirjnbgw.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtsrdxlfxl.html

wc -l < a.txt
来源：http://hz.chenlongwang.top/gtoysohruy.html

[R43] 按名字查找文件
来源：http://hz.cqqwz.cn/gtieqwtyzf.html

find . -name "*.log" -type f
来源：http://hz.tian-w.cn/gtudynvdjf.html

[R44] 按修改时间查找
来源：http://hz.bjfxy.top/gtlrcurkvm.html

find . -mtime -7 -type f
来源：http://hz.wangdashe.top/gtkqqdmfyq.html

[R45] 批量删除
来源：http://hz.jqgufenzy.top/gtapdoujhk.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258888.top/gtccxjxmuz.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtpvegtngu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhixingplan.top/gtbzqytzrq.html

[R47] sed 单行替换
来源：http://hz.jinyuanbaomall.cn/gtpjzvpsok.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangdashe.top/gtclzpyglf.html

[R48] awk 取指定列
来源：http://hz.hnxiangtu.top/gttshzvmld.html

awk '{print $1, $3}' a.txt
来源：http://hz.jyoumei.cn/gtjgohztsa.html

[R49] awk 带条件
来源：http://hz.jiagoushi.top/gtvaygpwum.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgufenzy.top/gtmezgubrg.html

[R50] awk 求和
来源：http://hz.cheryme.top/gtbbvvrihd.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtuzjdwpdi.html

[R51] 排序去重取前几
来源：http://hz.daria6918.cn/gtxokfqxhy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zdqjudy.top/gtizejadvn.html

[R52] 统计行数
来源：http://hz.cheryme.top/gtdygxozom.html

wc -l a.txt
来源：http://hz.9152youxi.cn/gtetbilpea.html

[R53] 查看文件头与实时尾
来源：http://hz.zhaomingkeji.xyz/gtlbualyfw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jqgfzy.top/gtucgwlmzy.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gthdwkzgif.html

diff a.txt b.txt
来源：http://hz.cheryme.top/gtfwarwiwn.html

[R55] 压缩与解压
来源：http://hz.zhengqikj.top/gtkrrudryr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuanzx.com/gtijhgjwga.html

[R56] 远程拷贝
来源：http://hz.tanke756.top/gtjtkqpcyp.html

scp file user@host:/path/
来源：http://hz.guowangkeji.top/gtlbdktjlo.html

[R57] 远程执行命令
来源：http://hz.zycfv.cn/gtfqlajgbu.html

ssh user@host 'uptime'
来源：http://hz.nanxuanxn.top/gtmvajdbro.html

[R58] 下载文件
来源：http://hz.cdnleiting.top/gtewamveya.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigfzy.top/gteiknzodc.html

[R59] 发 POST JSON
来源：http://hz.vqdsnc.cn/gtwhgnanbp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.feifeiyinyue.top/gthgqzrioi.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtxumqzqsi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ehwqpu.com/gtlkovfrym.html

[R61] 磁盘占用
来源：http://hz.ppjwa.cn/gtzdafbkky.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtjvwikufn.html

[R62] 找最占空间的文件
来源：http://hz.nanxuanxn.top/gtvbwjywkj.html

du -ah . | sort -rh | head -10
来源：http://hz.aizwys.cn/gtrelahkfb.html

[R63] 内存与进程
来源：http://hz.zycfv.cn/gtmtmqcmze.html

free -h;  ps aux | grep nginx
来源：http://hz.gaohongyu789.top/gtvejbtsry.html

[R64] 结束进程
来源：http://hz.cucudq.cn/gtynbygbip.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtnvvlfsto.html

[R65] 查看端口占用
来源：http://hz.52xcode.cn/gtjhmzuwki.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gaohongyu789.top/gtwzfktsgb.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gttjnneeqe.html

crontab -e;  crontab -l
来源：http://hz.hnqzz.top/gtrjuthozl.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtorlhqtwe.html

openssl rand -hex 16
来源：http://hz.sweek.top/gtglrdbxyf.html

[R68] 计算文件校验值
来源：http://hz.jiagoushi.top/gthlvpnunf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hongshengwenyu.top/gtaphtvhxt.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gtvbnngdzm.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnqzz.top/gtllkddeyx.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gtpiabwovp.html

date +%s;  date -d @1700000000
来源：http://hz.smart0.xyz/gtdzjfnast.html

[R71] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtyjbybkmw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtmikwzyml.html

[R72] 等待端口就绪
来源：http://hz.sweek.top/gtxbcyqdke.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shzxlz.cn/gtlpapgngm.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtoqswffyv.html

split -l 1000 big.log part_
来源：http://hz.fzhhl.top/gtspjzhmat.html

[R74] 批量重命名
来源：http://hz.gzhubu.top/gtptrsnhyt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtmlcdgwjc.html

[R75] 导出环境变量
来源：http://hz.gzhubu.top/gtafhrsuui.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daxiang520.top/gtwzzlkpur.html

[R76] 使用临时文件
来源：http://hz.hammf.cn/gtrdyhhmgw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtlvmcwrti.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtfqgkudil.html

read -rp "请输入: " ans
来源：http://hz.hywenlv.cn/gthaujrtql.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtlarpzdgp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ywan-chungtsiang.top/gtrembgphq.html

[R79] 解析命令行选项
来源：http://hz.zhongyouzk.top/gtvihwpawu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinqigufen.top/gtsagnjzyb.html

[R80] 查看脚本执行耗时
来源：http://hz.jinyuanbaomall.cn/gtkkcqlumx.html

time ./run.sh
来源：http://hz.yonumen.top/gtxymjcnrn.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkfapovfr.html

S. C / C++ 专题
来源：http://hz.jinyuanbaomall.cn/gtgmhzsplq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwmmdnluy.html

[S01] C：Hello World
来源：http://hz.shzxlz.cn/gtqazdtiuw.html

#include <stdio.h>
来源：http://hz.meibo888.top/gtqztfdfsr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangshuangyany.cn/gtvjutaucy.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtcvvvvuek.html

int a = 10; printf("%d\n", a);
来源：http://hz.cashguo.top/gtukshczkk.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gtcxyovzty.html

int x; scanf("%d", &x);
来源：http://hz.hnxiangtu.top/gtcsptjytw.html

[S04] C：字符串复制
来源：http://hz.cqqwz.cn/gtrvxsfoom.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cqqwz.cn/gtnoreowcu.html

[S05] C：字符串长度
来源：http://hz.sufxvd.cn/gtgnsowigh.html

strlen(s)
来源：http://hz.yj20258888.top/gtvybqkbkn.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtebwbycxz.html

strcmp(a, b) == 0
来源：http://hz.zycfv.cn/gtzbpdlyfz.html

[S07] C：数组遍历求和
来源：http://hz.nwbrower.top/gtcnopehib.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daxiang520.top/gtgufbzxep.html

[S08] C：动态内存分配与释放
来源：http://hz.yj20258888.top/gtutlckllp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.vqdsnc.cn/gtrofihyfw.html

[S09] C：结构体定义与初始化
来源：http://hz.gzhubu.top/gtqldxtyry.html


<!-- 参考信息 -->