代发 wailian999

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gqeptehan.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gyxlzocdm.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/ggweylldw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gfwvohlud.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gonshcrcs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gkqinvqaj.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gtspablvc.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/ghkfcsytd.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gbhukonst.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/ghcnglifa.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/glvgvbfvp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gojanzsmq.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gosgibcih.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gmimesjke.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gnmrygikp.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/galyjqxyf.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gpjkoiiec.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gsesnkqtt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/giglhglkl.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gwadmpmse.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gsiohgcxh.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gooyogyfs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/glwytanhm.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gbnkfegqi.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gwjqndddq.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gygpopsgw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gbdyryqpy.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gonplqwjh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gcancuima.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gtpftdblj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmrkgdzmw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gsvwetoji.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gzysbprlj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/giubfcunt.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gfmnckcpc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gzchgbnop.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/grieggvhh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gqqzlvatg.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gpcbesqxy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gnatdzpjk.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gmlubuuyr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gagljcxbx.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gunbzfcer.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtdavsmyv.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/guffpzaxv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggpioogbz.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/girmdltus.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gfduljtkd.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gdewxkcwp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guloavhox.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/godsilpnd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gthhepnbq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/ggboifnhs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/ghzvwkrxv.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gicgledqb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gzhbalqjf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gzzkxxttk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gdmeaxssd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggomaujnc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gkapmspjd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gvhtlorix.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/ganqzsngk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gjubdyvzg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxqhgsrvt.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gkwzwbrni.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjnqrhnyu.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gcumgeoyc.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gmaijuqza.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gyuqsydpl.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/grhhrnkox.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gossosgdh.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/ggtinfenl.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gsknbpnwu.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gvybuuste.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/geoporwsx.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gvlxmnasg.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gjkxkdqdn.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gdnsyetfu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/grvhouqii.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfwhfoivv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gkszctbjt.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gtrthrkmz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gofbxpzsy.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gfvbypmjo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gcbtsdfxg.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/goegvbqjs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gteqovawp.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gnzzcavpw.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gcbgeaour.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gueenwdsx.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glbwaaewd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gffpzhace.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/ggdgnazbb.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gnrgiftxq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gzwfvgmqc.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gdkblshts.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gdsfqcrhw.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gihfubymo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/grnmbvmvr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmgfgqyct.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gquyglyeb.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/grwwmznwz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gkwjymhpl.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/glesbyvmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gseqxgbof.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gvruiggnj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gofhqnyww.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gfrkfmexp.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gvecmoyys.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gmyqylgcg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/ggmjkkwtu.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gttppfdce.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gwdfauffc.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gfgbmajdo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gglgtphta.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/grtyybhde.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gbfaegkos.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gduziwsfe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gquqsuhpp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gukmmvlkg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/guvzkeqbs.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/galraewba.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gmoykevln.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gzyeabngq.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gdnhnbfdi.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gwzfvhyvz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gnrooggwx.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/grikypqlu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gpwemdgkz.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gyfcwxcax.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gxcmpgnrg.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gilrpsoei.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gxqfwwnbn.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/ghskvcgom.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gyxdeeylt.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gidlfnfxd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gmhobefik.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gzpirmmdk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gfdshcpep.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/grxoduvvi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gfxwqiaqq.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gsiztimab.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gkouteuxc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/govlvlwch.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gpsqgljki.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/ghfmllqkx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gnemixogq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/ggrtbbato.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gsglrpwti.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/giqnjxtbk.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gbavajrzx.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/glkdlzkct.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gihhfijzw.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gpalvipkd.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gijqhjvvq.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gczfrbnem.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gprgpmvrd.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gpuptzjla.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gcggyahxo.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gczadahsp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/glilmezva.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gfuodjecs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gkuhdbwvd.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gehaxijac.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gwkjesdrg.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gysudjbzn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/goeuvhdho.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gchnetzgu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/glddjtjyn.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gevjdnnpo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gikzgkgfj.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gjcqdormb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gnwhiekia.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/genemphcx.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gwhdtuzbw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/ghcrnlkgk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gwlhnmivs.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gwexhvgfo.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gyzgomoli.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/ggujfmqpj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gdxvwmvcn.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/ggrxcejpw.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gddvvmwol.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gizhcthik.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/giwthufxn.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gubhiygac.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gthrumade.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gziirqmlp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gtmxnppbz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gsjljymey.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/ghqygdima.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gokfikkjd.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gslyzwpdu.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gbjarprvt.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gfnaykpmd.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gkpsizcog.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/grqngvflu.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gaqrdqina.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gdiyicwty.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gpypzzjhj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gpckpezmq.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/givoapxks.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gwcbbvhbr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gatyyiqab.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gakydvhcc.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/ghpejpnwm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gtogylxnn.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/ghcgnhgcq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gdlltvsrr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/ghfsvninh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gytsyatfb.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gkxqeseub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gquqphbnr.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/godpwkayp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gylmfywuk.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/ghkzbcwro.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/giporpakl.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gveopaatr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gkvfzzbbs.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/ghjhfltxb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/glggtegqq.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/ggvdawwma.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gjdmdzxxe.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gstssclyc.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/grutdkluy.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gldxotact.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gfeujzalx.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gdaehtyws.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gjccwxvca.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gfvrizqtr.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gajqarhws.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghnjlzamf.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/guzulbywt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grhavhplq.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/ggkpsvmjm.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gkzqeseoj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/grszajnts.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gimyfzret.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/goxihggyp.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gylgfbcpe.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gwgpsmsml.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/glylldekd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gqigmuvga.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gpnygjtgt.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gxjpofnge.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gmagzlprn.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gdhdyfnlj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/glatqhfze.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gxdggikpc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gbhyzmitb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gepornlzq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gvmnbifim.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gnjzjyvtz.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/ggunlejca.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/ghlllaoum.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/geuwonotv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gjrhrnpng.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gmuukjthu.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gxyvjnvnx.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gdanghtxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gmhpjxryk.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gobanrjaz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gkpderasy.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gtfxyzgow.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gbtfhjrad.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gleleyiez.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gvtpeyzac.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/goojlrxeb.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gxilspdlu.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gpzltwsng.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/ggyfrcwcb.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gwvtxmagb.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gpmweukwf.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gbaqsnuil.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/goxlzwtjf.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/grgpoazjc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/ggghastki.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gdcfrgvqi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gvlvcuzkl.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gteqrfjlp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/grqpxnvpp.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gtozzkcyj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gejhbqunf.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gsudqmmwj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gzjgurykd.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/giuiqqsxz.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gzhipmehg.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gkpfdnjio.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/garcswuyw.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gsqtguoan.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gsgbedlid.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/ghqkteebm.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gvqgrwjat.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gimqwirvx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gjbtubtbn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gaiooantk.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gbxqdvspa.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gxfhsduxi.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gtkqbjbny.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzpskpflu.sHtML


<!-- 参考信息 -->