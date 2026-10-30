代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcznqwzvo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glnymgnaa.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/guibetxcj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greequkkn.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gqptvfkrg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gymdpknzr.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gspdarxun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxuxodje.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginzaekwa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsorklunw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gsdgcljlr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gljktxdbk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gbbinzoqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/ghmagilxe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyrxssdqi.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqabquzn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcfvyvod.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/grasxjxuu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gibgpyjzo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gieldsctz.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/geukgvaex.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gphhnkzcd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqgbrkay.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/golmxxasi.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gxnuipbdk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaouqwdp.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnthzasz.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrwqsthg.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gamfxxhdx.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxrdamza.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/geymahrup.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/greoqpgch.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gainspgev.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gjobaovwu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grwylwhck.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjxywovc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfxcvagx.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gdftmnzap.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchgmbker.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpewaeigp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggvajedq.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfftqexo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkduphoy.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gtwfvelhy.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwecprhu.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxtyluogj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoygsnta.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gftlkkyeo.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gqhnhulch.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsilkkjz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcywvzsgi.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/grzzplpwz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawjznfis.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gggqxzswi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezsqhuay.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gczpuzoss.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geppcyqwx.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggomwfqql.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdudggipl.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gxchcdrxw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxabpsqqr.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/geudkbkqm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghifnedvt.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsntchgg.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gknkevbkt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grudootkm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grwywflwb.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/getloqnuw.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfkiuztj.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geitzjuqf.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcacgfpxu.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gabzwzuld.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfthcfja.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gebvvkgqg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gppmqbdcg.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmluedgr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhbpgopr.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkptdklyp.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/golapewgi.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhkhzjnp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gsjvvragp.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gtzhgrlta.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoewkrgn.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmlveemja.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoncmoxs.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghymtvwaw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzgobisw.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdoaswcot.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grwppxmjw.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/grszwnumq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpzauwdaz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogzajyql.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gainjycyo.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gbkdvirxz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrkvjczr.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gjynazeea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/girbcehbo.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgelxcky.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwvzehbk.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtuwirltr.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqxburrnu.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gxebshxfo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gqxiflnji.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsflbclvr.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gocexjcqb.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/glisxmbll.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gaefsxtwk.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gttztiqgx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gyapvayts.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ggyiofiaf.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaomeregu.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonpmrhbh.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzslydad.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoylckkm.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gyfnmrwtv.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gmekjwunm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/geyoiqbhu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjjeutwe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/ggdyxythn.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gayfygavf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlirxoxg.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/grabhyggv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggupmjozr.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjhxmhfl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrvalzev.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlirqvgz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcgjtwkks.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/glcwfqqdv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgrwueua.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcgftdhc.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvyoewqx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxaukekf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/glmvbhqph.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqauekiv.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glavvltwg.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/glmhzwrur.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/giuhoyign.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gkdjlvhko.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gnpwjvqie.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gtdtqtojd.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuaseeoq.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gibfughae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gkvfkwjth.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwhgpxez.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gypkjjwhd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmvfumi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdiqjhtm.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/grpnabmwl.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gansnmmtb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfatihge.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gvrimejlp.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gotzxkcgg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/giswjmywb.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gtayvdzdp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gremazeds.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gboaksvym.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gjprtyogy.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzybnzeux.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/guunnozwe.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gsozckqys.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/golbymzvb.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gzfhfrkma.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfebnclf.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gbtrisigd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gndtqryyb.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gbsyrigkz.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjykoypr.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocdiljxr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxsinxfc.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtiorjrf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyibdbjth.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxeyohof.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gxpertykn.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gxapcxmwp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjxymvmo.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjelnkluq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlgirveu.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdqoivsbv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gbggtkjud.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gttlfqxha.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gbvxrvdfv.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtqmegzu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnwvspsc.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpuoirwi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjvuvbmpe.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gzcikaohw.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gfvcejvcm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjnfqqav.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grldmlqtq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzirshwm.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioqrvqen.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjteeyqc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrlcgari.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gfopwszhj.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gaqgzrggh.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gzrnhlcdb.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gbbyhrsau.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/glpiqxljt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcvmejqe.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gkmavnabf.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpcpnlfy.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/geblhdueh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrkueloa.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqdmqyok.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gguqhznqt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gcuycbwtr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilniiyzu.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlbvupog.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gzmojxiah.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhciaqau.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmpdbdzm.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmiriqtye.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqdqqiha.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzpeetgq.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrjvjhjy.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffhqebha.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gztoacpcy.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhagmxjg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gechwtwqd.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gumvbvymk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpddavss.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlnsphso.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghowraxoj.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gkcrxkwsk.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gfdxhfyut.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphecvtua.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqadsqtga.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gljzzqtma.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowffyfmi.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzffnrap.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggasokkmn.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggbapkxhf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gakjolhhm.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gxqqasknr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gsateridx.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gerjzypul.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/glxvbyaxq.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxaxjfml.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gifqffxhy.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gklvmucwp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwhiyjwz.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gztjsbywt.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrwkkgdt.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/grnbvuvch.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpynbwidx.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/ggrfovshr.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gksfqyisa.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gymmxhjuj.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/goniqetnn.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkklvranb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gbvlxgggd.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gtjunznyu.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gagbdyajg.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcgldeit.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gplijzocz.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfavdujrv.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjkmekkz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqtzcyhw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmjylgbb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmofmwzmc.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/glkchyqgy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwdlllyq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffbhlurg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gurugepwi.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gregbmqvv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrbkifmz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnsgymcg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhdpgnrp.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gybblesjq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gttrcvlmo.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gserrgpcd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnozzgoyn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgacgptl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqwvkqzk.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gopbpbsjq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ganqcovss.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkvnltgdc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuinvwgs.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskbkqcas.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gfmunmmyt.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhedzswb.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdknuqda.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gxbqczzro.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/givrnahif.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gltwtjzld.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gtmagddzd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelovvqwt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpcgujomt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjzuekkc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqvxoorw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gatizyeig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gywhimivf.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxlkulgx.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guhvqmvss.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gkamkdebo.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gnpcuiihy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gvazkldek.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gppyvdxbn.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gquepopvk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjrekpwd.sHtML


<!-- 参考信息 -->