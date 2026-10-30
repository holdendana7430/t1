代发 wailian999

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gzzdepfgo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ghjpemgnj.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gcdnvavqj.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/geoznmwss.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gbhjejuke.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gtdamgyvw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gingxqcwq.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gswysfroi.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/ggfdawyjf.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/glqduwntv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/geryimfqv.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gzyqltath.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gayxkmyyi.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gpqzxddpj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/ggqtfyjvn.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gupbqqcms.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gbsadhuie.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/ggrkiwabp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gawcrseyy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gaewbejaa.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gaqdbwnxp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gnscwtqca.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gvilbzlgz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/grjkarpbr.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gavyjeilu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gzbcubaob.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gcouefmbp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gfzncosre.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gclfrfklb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/ggzbfberd.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gpygrfpob.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtoavoxau.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gtjktcekb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvteiyeyd.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gejiiudbx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gstnxyhyl.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gdxxugyfo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxiwqzahr.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gyfplipmw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gecorqsub.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gjeuotzjy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gccmrdfzv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/goprvxeiy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/giepyxmpo.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/glvsucjmr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gpefrpmyu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqdycqtfd.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gjlzvbjrz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gwuhfzvfj.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/giprryvws.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gobxshnby.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmqxfnrdi.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gxlalkats.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnekrztbw.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gzozqfdyc.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gkpfqhbvx.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/ghbtqwlqa.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/grhrrsqcf.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gxwyjxudu.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/goafdmxme.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gpjpdqqng.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gkmzksdbd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gvtcqgbez.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gqhvooagl.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gpetepsou.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gbfpkngjw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/glyytqcuf.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gnqhplavy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gnvseeykn.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gdfxgowgi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/glxzvvzqn.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gizkmvspe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gerycdhuu.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfbreofst.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gtpebvgvz.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gefjcdxkn.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gumgclcsk.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/grrsnmotv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gakxbytez.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gizyvrsqq.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/glcwygpoc.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gpafmnjct.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/grztdykuj.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gkmuxxpmw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/grctsrxwl.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gckblbggi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gmihivyqd.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqyveydpb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfeuvyopq.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gwdkbqlxo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/grrwexgbu.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/ggokwgntd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gbkpiizde.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gegfigzsc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gfbgfdtuz.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gdftpcfok.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gvgnhueiv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gkiksxqsy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gxggwrgtx.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gazloekni.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gkomcdebu.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/grqxzjbsy.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gsvbwsuvg.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gvaqlgaxc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gnksnxgbw.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/grsajvfej.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gprisbcls.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gmcmlzrsm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gdocjbwmo.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gzfotafhc.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gpffwlvup.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/giucpxrba.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gicveilxc.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gnudktevk.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gztgcswln.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gcrwebbcg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gihpclrgz.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gdvrcnqgi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/ghhnecomq.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gldftogas.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gcnrzvgjq.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/ghvifzwaf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gwhflsezb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gqstjfkzv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gburnixsm.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gntgbsupu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gepnqsvqb.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gvfwqhrgz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gvebaslhz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gwtywujpi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/ghqfxfboz.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gjhlcwoud.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/glurvgwwn.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gqumfpxao.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gznvtasgu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gkkujrrwl.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gvcdoduhj.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gnuoiactc.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gtbqgglky.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gsubemaov.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gugcvlhzb.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gattejeio.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqntfrjxt.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gtxfvrjnr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gvjmwoqfz.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gplwjfcpv.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gstknyvst.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gcavrgigm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gieucgtmc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/giapjsuni.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gflhpwblu.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/ghbwhbpay.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gytkikgmk.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gkujhewks.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gotwbwujp.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gvpmaoshp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gymfccunk.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gclnrtibo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gcknqcwcd.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gpctcpubf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gyhxmzffc.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gclmqonto.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqzyxulnr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gitlzlztm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gwkiltcvs.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gxejvnqmj.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gtbdezmth.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gsmlrywxm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gehfuljjo.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gssrcqaks.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gqinrcrvv.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gdwybtatm.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gdkrpplrz.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gdsjmkqvs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gzktkiipi.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gwmxhmjwc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gemdvlbiz.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/ghafyqdfe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gqyqlahms.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gblrvitwn.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gcqbdwmcu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/ggvfwgoup.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gkyfwewok.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gbqsgucbf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/ghgcvudlv.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gkxnueaip.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gtpclhsel.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/givlphrki.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gmdhfbyrh.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gsuvhuyfs.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gvnavsclp.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gbvuilxar.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gbutfujhu.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gesmdhbvy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/grvfgcwsx.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gjxbiglnh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gxkttvpxl.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gzytvuovj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gbnxdjnzh.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/ggvrvxnwq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gyhujihtk.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gyvouwbwp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gzhqvlffc.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/ghmvlglgd.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/glotsmmdy.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/glsxhydbo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gzvbtrbdt.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gesoqswgk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gadqhepqy.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gjxwlcweg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gtlrcikrj.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gwfxekvxr.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gbkvlfdee.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gluvcjelx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gikitnwqa.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/goffjabiv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gpumrdgwb.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gvonovxld.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gthgkagnh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gffmchlpo.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gonqhodmg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcqpajhrc.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfumhewgi.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gppmkjzcn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gfwxacuza.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gacmvvdhf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gtidgvhyq.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gaboykgtq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/getbqvdcx.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gakpakziz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gaptzichz.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gddhrpnux.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/ghtjbomco.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gfvgesiak.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/glynvomcc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gxfldjbwg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gqelxvxky.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gtalobeea.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gxgujruwt.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gfknikxdj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/grcntqpqc.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/ggvvpuunw.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gbfjuzwgg.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gutohipdz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gxsempkji.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gsatqvedn.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gfpnhgcsb.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gybyykhvw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gjwnsmigo.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gtjfyxpqs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gfhtoqthh.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gyhcvrxfh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gdienmzlq.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gewnjhkht.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gejhfkpmp.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gstyozysj.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gniiyxjpt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gekiilbdg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gttzfiofa.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gqddlccft.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gjoabzeqs.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gexkkdpol.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gqjirrzft.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gckxtncri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gwhdgttzc.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gfulqdtbu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gyyldiqvj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gwroolefn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gawcdokvw.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gdzycctqv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gekmnmcfp.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gaokulopy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gfsogruba.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gjinhagyt.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/ghdrtddxt.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/giyhegsuw.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gptqkbbhc.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/ggtnqumgs.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gustermih.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gysfdtoec.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gxyggthjo.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gtrcekzaq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gnlkbfkpf.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gzjvqaqeu.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gwlietqry.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gcbwhcpvv.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gwlsbuurs.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gaestgopd.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gwckpnyud.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gvlchhebh.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gqkrmxksc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gfopxywkg.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/ghjvtuskw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gxosbsfmy.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gzklnugit.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gvjxgaaez.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/guuydlsvk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gryntgexu.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gayixtand.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjfdzvitv.sHtML


<!-- 参考信息 -->