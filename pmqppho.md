代发 wailian999

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/guvnrqcrb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpdonjbtd.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gbxslgroa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gqsaoyusj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/ggesvsnpd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gxonvtycp.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gwlhwlkax.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gdaamrnpx.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/giwinpekd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gqnqjjqnn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/glgbiexxl.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/grccdveev.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/grsdmeutx.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/ggmvocjrj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gqbvlfopm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkzhziomj.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gitpwcvgt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpqvvsefs.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gisrbbjzw.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gyadaztwe.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gzzkokldu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gejtviwvu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gwymcwvnn.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gqlmyyvnf.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gfwocgqld.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/grldcmxdi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gyxfryhib.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gcpokrpou.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnyvvxrxi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzcwmjgxi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gdejnapdx.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/ghcsbbciv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/glzemofok.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gsbguezth.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gexbbevxw.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gpmikaitq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gikdgvsya.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/grjfwclnn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/guviivisd.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gtfzmdfox.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/ghqwtenma.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gfieogqcr.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gdkaqrqrw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gzkuriujg.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gyuhdmvoi.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/garvihqtm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/guzwxtiee.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gplsuwtgk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gwwamjrby.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gxgddnxlp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gqxtvhiuj.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gmqlbsfzg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/ghcakpbta.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gtxyjfcnu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghijuerzc.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gtuarluel.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gwwmpxwyw.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpmoxdeft.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/ghgdthgkw.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gpizehlil.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtjekitar.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gwotuckgu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gsigsubkl.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/grhflfiqo.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gpzbeqxfd.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gjrqeflis.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gxkqelejk.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gvumiknlg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gmqosiwdf.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gbafcfcgi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gsrdpymuf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gqqudynxa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gaecctmgr.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gsrsyicyv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/giiyygiha.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/glajgckdf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gxinfgfmx.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gxggtrlrt.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/ghicxpwob.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gosrtfili.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gspzvyvpo.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/giwbcyzfv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gnqxkzdjn.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gonvaskwl.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gduayrnpp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gfrvkmmbo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gqnclgvqt.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/ggaylpssk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gzhxzhynl.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gbxxpohgz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gxxdtdcvj.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gsgtbvmln.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gxpgkhdms.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gikdtdnjj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gyqdyyopv.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gbrkxprwj.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gduigwukn.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gkkyluhdw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gkugjhvug.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/ghncbkavb.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gvngwdqab.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gqhgscdzl.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/grlkuqdsd.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/grqnjqcba.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/ghwzurjrl.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gahexugnv.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gkvlmjmhi.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gsqlisaoe.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gttchlgzr.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gbewnlklf.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gqzgkyfto.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdwqorv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gkzuaobta.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/godxzbvyd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/ggatkcjhm.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/giqturuht.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gnkmgrtju.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gqxdrmyqk.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gynthlabq.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gjciubhgo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/goefmcgmg.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gwosgqntt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gjvjmxfrl.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/geyeysshr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/glwzotops.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gzqvsecwu.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gyjakccap.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gwfiflfal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gqghufgmn.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gpxniytbg.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwxhmnzun.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/ghpdutyxg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gfdnzoqke.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/grnicelmy.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gttaardee.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gmywwwglh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gclshbguc.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gzqkditwn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gfgzhahdu.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gxrycdmnb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gphzxrjnw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gsbikinqi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gmjjhzsat.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gwhzzgxwr.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gpfhbzuwj.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gvbcaswwo.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gsuhrsizj.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gkncorvik.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/ghaeudpcu.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gfmnspahl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/ginrjsvbt.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gutcmqdnm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gitnluhva.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gtfniudfv.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/grunbsgsm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gsnwesnrw.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gxtsnqyhd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/grpsmzmkp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/grqlymlgn.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gqfwjbzrv.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gfegdirxv.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/ghrtuzket.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/glhehrhfl.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/grnxrvnmn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gverubpbi.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gksdrpsbo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gafnxtsdc.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gtjaeilhw.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/ggsstyezn.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/girbvdpji.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gzgiyiesp.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gmzlrdusa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gmqmlpoto.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gemhuwqky.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/glkfqygth.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gmfwdwuax.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gnszfklln.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gmprnkgrx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gkldlxikz.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gsdedpkqz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/guiylnzhu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/ghjkffypm.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/galmzjqvl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyrlqgybl.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/ghgrgjuyz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gldijskal.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggzeyxfjr.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gklxzinjk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/girvknxqz.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gjlkxpbhs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gndyzoylw.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gnpzvxtlj.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gwfdgqzpq.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gcnndbrjn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gdcyonndg.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gzijeudim.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gduynpktr.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gjvtfzcxh.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gvnkltjfs.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gbsdielha.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/ggfjbkjas.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gxsjhcinw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/glprczlzj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gzbwnyvva.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gbdubgqae.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gvibbkauh.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gjasokhiq.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gfbrznvmt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/grvyhqtfq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/ggwwlcply.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gmdirgqht.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gyzjcwhpb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gjaqqlxjq.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gzmsmwlqs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gmztoecrq.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gmzayddvs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gvwnwtkbi.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gmcosxiix.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gypznfmpj.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gderlfudv.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbnrtovol.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gsfixvebm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gaektykks.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gacjwllsd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gnponkmer.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gmtadcddg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/guecolvmu.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gcxdfesre.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gnkahbrss.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gmrvyrfvg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gtmvdagna.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/geixsrhsy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/ghxbboxdq.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gvkvbvlrq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/girlsultc.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gwryirqfl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/giewdvxpm.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gyzsoxmpo.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/ghwsmxhkj.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gxhotvvhm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gytsuhyow.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gpbnhyjlq.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggbivjnkk.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/goaaxozkq.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gfnmafqcz.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/ghvqtdomv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gnwyankug.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/ggvtobako.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gzdkzrbxe.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gzoecnomy.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gabnjxxma.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkrozrjou.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gwzgljtci.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/glujzyjfv.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gmgtmlwwa.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/glgfbuwgy.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gvzhnmcdz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/ggisjncxr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gbbjystbh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/ggytvhvcp.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gqbjdohqa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gsvlwxtop.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/ggfhxnqmh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggcfnymzu.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gxmnnukdp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gahygsutb.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gjdqngvmh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gnbjbgblo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gfztvyivm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gnnzajavs.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/grwioeuim.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gdlucazgk.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gjypsqgrm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gshkspuea.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gryqthxgi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gnrruwonx.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gclnsriuv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/grjbytmfj.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gavsyaewp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gqukowntf.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gpbxfephn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gaxfssdre.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gdneqsbpa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gnphuhqla.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gwgjzjcac.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gdbwzjrdw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ggewppsxt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/giasrpgaf.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gyhcmgglq.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/grwzcvxke.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gcsuwxlkx.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gajvqkbje.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwrmjtpnk.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gkjxgtukb.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gdzuwcsjr.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gzetrpqbq.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gyhrtqbeh.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gghdhwjcg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gsihhxptd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/glsgshvph.sHtML


<!-- 参考信息 -->