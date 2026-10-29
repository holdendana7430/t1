代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gevlzpwyc.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gkqrdvyst.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/grbdtyqta.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/grocufhxe.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/grtuuwovj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkivdkuun.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gjjyjmlzq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqdybafqj.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gfznhijxp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gzimcwbsp.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gvyhggdqs.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gfmwmypxm.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gdxzslavz.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/ghhofnfvo.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gyzzhnydn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gchvdkzcn.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gpuefxqds.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gwrusfwvy.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gffjsjluk.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/glgkwnnoz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gwggffzgy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/ggzqsksqs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gyradrxeo.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/ghqomorlc.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdepcqwn.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gvqdduewh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gmxohigfq.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gdhhkxoex.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gepigbjpc.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gifkqnsny.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gjjosrfce.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/ghnibmhmi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gkdwlkisf.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxkzckiws.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkakdauxk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gzvbzecdt.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/ggxwlsbje.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gzunayrmh.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/ggvtcepmi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gmipnaehw.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/guicdujco.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gmaesxnlw.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gjehwgipp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gwmfhozzx.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gayvfiwup.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkwgsnezo.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gqvrmgszf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzkhiodsh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/glzqmnrhv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/goqglvlop.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/ggqswouxr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/geqxxurxb.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gxjpmjxgf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gemfjsbwb.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/ggsrvvozj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gtteyjioz.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gzjzrvqwt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gayorxhmi.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gfzcvmowp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/goirddunv.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gpxnceqga.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gghrvsboq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzkznrtud.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gqfslejmx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gwladkbrc.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/ggzvyarjy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gzlqwhwod.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxzicjrgn.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gndkuqfia.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaksqrwzo.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/guneldnpw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/ggsxejjtu.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gvhdtzfix.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gzqkoiezs.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gxdntuajt.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gxtlrtbqp.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/ggpamjksj.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gkjwcbway.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/goeojqnwj.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gsrqjaxsw.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gzhpinyzq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/ghtdsdkqf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gnyqggytv.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gxfkjqzde.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gjvktcdog.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gpukkodfd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/ggzolgops.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gegyrsthw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gsglhaeax.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gaotgzbrt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gmvdhjnba.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gqfbhcmvx.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/getbmvmdy.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gjcwszazs.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gzwxkqemu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/ggqooqcpi.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gtolzwyfh.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gzoqzifzo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gzxfaehga.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gpgehhggv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gazwloftl.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gfqrtsxee.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gymharpoq.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gtnfujpbt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/grmefxreb.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gjdlyxoaq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gnulecazf.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gaesexwys.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gcpcxayys.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gnicqdgku.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gnfpkrzkr.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gcqfewdho.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gbomdygrr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gwbsxagpl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gaqromsgg.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gjrxgkuei.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/grhmcirwr.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgunfqt.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gvstjtgsi.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gpklizhla.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/ghobcgmbq.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gttvdctst.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gzydlxdrj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gjmfwvrfr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/glwmpqdmq.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gfsmihxog.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gtacjtphk.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gnhvkvuzl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gwivldwlg.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gurriqwly.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/ggxrlzzqr.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gqssogjpv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gvhmiggfx.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gkxrlmtrp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gionfrsml.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/grrhgeiab.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/govhlvkni.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/ghkrzrpbq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gcyibxdrw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gygbcfkhy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/glolysaxd.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gakqqcrgc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gccodoepq.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gdylbvenn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/ggwroedyc.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/grbacwgzv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gbgrgwqfp.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gzuamjxal.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gmvappcks.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/geevglisi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gypwlgpht.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gopusmfbn.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gzzbnevcy.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gteltrvvd.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/grovylnvs.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gqxknmnlt.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gafeyfwsl.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/ghzprzjll.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gmavdrdhw.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gzcgiktxo.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gvigkbank.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gcrlcxeub.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gqwbsuyrk.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gsbyxwyhv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/ggjemizlc.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gxnrmxmdb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gwnjqcpbg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gxiurgokr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gixdtgxao.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gghmsbuoc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gusiuxgds.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gvfutetaz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gdlqvvvto.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/ghynddder.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ganvehein.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/grfmswilc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gyvgtnuix.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gldnvtdio.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gopjzerrx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gvpnadozn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gwcjcfidl.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gvkdpklao.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gltlsrsue.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gxaivuysr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gasxwmsok.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/glwaxalug.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gqqznudrm.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gkjewrvxa.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gruvmmstx.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/glfrrvflh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/glyupvlzv.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gqxvdrixf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gpgffeuwi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gcbsfdjyk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/glwoyjopn.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gextorkbu.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gwhddmuaj.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gjnzfnaij.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gllbskgqd.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gshckjnco.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gqwrcytvq.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gqzhqymje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gxawngmqv.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gqzyrvgzd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gyllguuaw.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gwqwxxngc.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gdcfpaple.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gixidzyol.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gaswnuqpq.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gzosziyxu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnvhckkod.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gjmjmulny.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gqapmjwhd.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gfninfkwf.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gmzvshhql.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gaaukycja.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gnarwgkln.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gdwyfucgs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gwdtpebft.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gaymosulj.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gppeggjkv.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/galtypycn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/grlxxpnez.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gffvkfuuk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gevlbvxmh.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/glfibcluq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gbpdexdcm.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gmguxyvei.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gsxicyrse.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gfdxfudos.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gsonspepm.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/glyseirnz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gwpoplmqo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gdwsgninz.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gddkzpucy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmssxuqmf.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gyssbxmov.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxxljmrxb.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxddopnhl.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/goyineayf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gvdxzsrzi.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gmxyjoyzw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/ghndjgvzm.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gxyhdpnam.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/ggorhwojg.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/glempjzcm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gpkmmcaae.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gcfkjndhn.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gtntmbjxg.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gfugegkci.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gsgttitgj.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gyttbitmq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gbbhvyhjo.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gcyercvjo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/ghhztnzfq.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gprsedzkh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gfyxtcqbl.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gjqljkjsm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gbibowesa.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gqkolkqyg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gidnbjrjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gteruqatq.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gsyivazqx.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gfegswbsd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gayzrgprr.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gcedrtcog.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/grehumvyh.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ghptrmreu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gouqprbiu.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/glusppqfn.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gstpbcgml.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gonkbdjbi.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/grckcktau.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gntyanokh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/guoacdycw.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/giaudxzum.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gcznbpjbk.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gpiqqfsme.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/grmdomwtx.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gkknmlumd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gjxldnnjd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gkfiejrma.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gmuffcdjn.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/ginkkajmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gregjknbu.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gqosrrvsz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gteivlnnn.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gdxflxzcv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gcgvnprsr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gtkikxslf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/ghtdchmzn.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gzkbpcdfg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gaczxwdcv.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gtzxqqfii.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gjjtrfenq.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gevfxboli.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gtovacwsq.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/ggnmrkxln.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gybmsgnta.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gjocwhbvh.sHtML


<!-- 参考信息 -->