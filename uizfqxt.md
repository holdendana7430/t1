代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/ghgvprykp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gatxaiwaw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzylmpeur.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/giwzorlca.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gxsqodhst.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/ggqxodmsd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gwqmwsqrh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyowmgrxm.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gocvhnaui.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glnaogbpo.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/glbagwklr.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gqbpnfuhe.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/ghteeotao.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/ghamzvsvj.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gtutvehdj.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gkhkxwxdx.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gbnnxzwyo.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gcbxevrvk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gqqdknmfz.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gzsnotddo.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gstatffvs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gziabsnpo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/grrnlhkwh.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/ggumelfwk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gtzljzmly.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/giaklhzna.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpbugmesa.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gjstzqwkd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gmjxkqqex.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gpctfpuba.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gduauoeqo.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gxhktytox.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/ggtsasxsz.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gnctvmpxr.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gmcnyxzvk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gdxycmsew.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/ghbqajfkm.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gzinujonu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gjehmkfit.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gmqnckmoe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gnwzqdlgi.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gpqvdrxtv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gjucjrgrv.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gqidhmeuv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gucyhcunz.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gfxmohqgw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/glypaabcq.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gxdkxrzxy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gfwcscmlt.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gnyjzzjww.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gpxfsxgdn.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gnkobapzi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gymsvnhrk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/grwoqkjsn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gtcioknbz.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gibfxxeht.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gfsbfzzau.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/glxtmhphg.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gidqckwip.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gnvtuikrx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gxhzvpopw.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gzlupwwsn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gyvzrnvcb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gepmksoku.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gzuaetgkf.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gstexnbnt.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gyavfguvr.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gmyvmjifq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gyshwmhez.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/grbomclbv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gacjoodlq.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gtmbthyhf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/grzcxfssx.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gycljssgi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gdgrpdwxz.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gputvbdka.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/guafejcex.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gewmyexsj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gwkuudove.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gjnciioed.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gbhrdzcop.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gigayrcyc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gawwbyaiq.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gmnqmpthq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gasqmiusb.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gbdgburen.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/grbqntojy.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gnieqkvaz.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gpalqylcq.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gqpedpilj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gkcnsfubi.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gihegaynd.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gsscahesb.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gireonqgg.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gqxqoganh.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/geywvtxjh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gkzrailxy.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/grcfklzev.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/grrlxjwtf.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gsdsyeeqg.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gvkzxjpgf.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gmcdjamwk.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gnvnmnuxs.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gqulelery.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gshkvqrkc.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gqhrtfrrn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gmcvseunr.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gkxaxqlkf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/guebnwduw.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gbsmdpyqj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/grxbusrjj.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gjyxgdgyh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gsuwefdbl.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/glqkecdgu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gimhexher.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gnepdseie.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/geubsdulo.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gdehdknju.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggbbnxmiw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/ghuvyyqfi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gppfczqzq.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gtdhkbfuc.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gdmdrisru.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gefbbahzk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gsgxloadh.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gpdopsmsc.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/grgvrdmgn.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gupblhqdq.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gadmhmido.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gjxmqchhy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gkphmwstu.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gzanimjjo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gcvshsdhe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gsufejqtg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/guajnwoxo.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gxbjjutge.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/glbegblvp.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/geqlnqvyz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gbvenipns.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gyokxhwaz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gmqtbkvwb.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gujjhzxpj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gbzyapmoe.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gnsmcqpqz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gtrqybupw.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gxrgcnwxy.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/giaamwasr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gflpvspdb.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gstviyjlk.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gdummqfrm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjfgyhqxc.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/ghdwahjww.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gvfuholtg.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gzaruaszg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gnptpoyah.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gfxwafkvz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gmzkmzlsu.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gygzxlmwq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtnodqroj.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gnawvchkf.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gvqbbnlbh.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gochrcpat.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gbbtwywjb.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gvprzfodo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/givzbozww.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gmpnzwvqx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gtxqogqtf.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gmhvhsrmy.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gjrwnvbqi.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gvgyzbopo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gbvfkqbim.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gfbjzumro.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gzwfqoffw.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gdwymkghy.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gupigrgkb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guynqsbwn.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gydjofvhu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gacwopedb.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/giuwtqdof.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gakwfhkoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gmfvrzuvw.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/giwhqwjjf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/ggttocjok.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gcwylbaax.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gofmdsofg.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gsmjbvudm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gsnymrsjv.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ghruiywdw.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/guxernjzf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gxlivnewz.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gczmvsabd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gdqbyezhj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/glbaqhtww.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gvkzltkdo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gijrsalcy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gqemsdvxm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gqxjcfzhw.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gnpjsfyvq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/ggtyzixco.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxlgdiqaw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/ggwqfdcyf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/glntdglre.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gcknpirjq.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gyzxwhdrv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gqcabplho.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gbyqszwlh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gxopvczge.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gwnhbiadc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gaegwooka.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/guobyldcp.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/guzzlweqf.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gbwvfgyyp.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxmfefdta.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwqeqzghn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gdcrfvygh.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gnvrmntuv.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gmmoynaem.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/ggksbnanb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gpxsptmwz.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gjyurqldp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gbqponhlw.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gzenxyajs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gwfshphfc.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/grprkeovs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gvufgmgpo.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gtzkpbemf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gkgnqhmze.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gxznmwimf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/getaijrjg.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gffzwemtt.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/grhdumfrx.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/ggtviailg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gezcakrwf.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gpuzbsxip.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtlqrwfrd.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gmswxbkxn.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/grnmgdtkb.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gmedrrjso.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gyrjjjrsv.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/grydinrkw.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gqtbqeoym.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/glsgvakyt.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gfpjdfabg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggpzdvofr.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/grfnfirqf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhijfjho.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggizgwwqt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gsbaclajx.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gbgkipkjb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqxavpijq.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gvrsdcess.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gepbcgueg.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gqvzpvibv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gujsbiigx.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gahppferj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gotzhvtcz.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/ghiazfgdz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gbjlaibfk.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/grwvsetso.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gusvqpxrm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/grueoufmy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gwyehsoao.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gyvcytaom.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gzwwcfixo.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gjvbzsqmc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gjsnuunau.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/grvojbdfz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gxypagkek.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/ggouyujbu.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gqixyujgj.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gtpbzrzij.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gzrpplgms.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gqlycpsei.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gazkxthbs.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gntbhkabf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gmttpxnpa.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gagyrmbsy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/grhhcbejv.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gyxifrwkk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gogbpncky.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gsdevtqos.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gludrkpmu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gakckzkpw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gpygckjrz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gwkmqhiyw.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gktztyani.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/goddkvzzy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gshiuxrzm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/geiufzbyj.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gdivvumbh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdvashxu.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/glvfmkqru.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gujmmozaf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gubpgowks.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gvrsqybve.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gkhzkdela.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gtqrbbnop.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gcoffbfiv.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/ggkmkpbxl.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gajhtloir.sHtML


<!-- 参考信息 -->