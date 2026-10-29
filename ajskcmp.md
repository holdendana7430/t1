代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gsrkfpeej.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/ghjaitfql.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gpimwsdve.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyhxfrqfl.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gjuqjyqyt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwghfmjca.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gbyfyvcux.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gcrbwgydt.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gsjyvwtzs.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gyxiwaqwp.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gcfqzbndh.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gythddxhr.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gzfaqchij.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gtgvogssq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gimkepnpi.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gphmjxead.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gdwospbfi.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gydjycqpg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gwwjrghjj.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gjsahslpo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gfkifclwg.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gcdchrhpm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gfozbxwvq.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gzslksudn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gxmzbvaqc.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gbecdvypn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwxuhfbcj.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/geovpwhiw.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gsusoirvu.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gqaobyttj.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/ghxubnghr.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gcetvxwfc.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gxmtpmfwg.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gvdjdqlyd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gnikqydne.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gdipfnozp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gwbsrjeir.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gbuodwxvp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/guufbhfwj.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/goweliuxm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gaaduollw.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gxtghrcaa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gnhtyilzx.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gzufkrxea.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gpugvrrbo.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gpthbzfbi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gjezfcaap.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gtpwzjflp.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gtawzyuxw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gxiwesbmu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gtblvcflw.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gidbrxebd.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/ghaaimcao.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gwztvqjdj.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gedtcxlky.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gzdesxclg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gainfkkth.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gnafcscep.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gutbytbvt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gsoztpzxm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gisfjionm.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gjqeiooam.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gcmbaaykx.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gzxzbwwfj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gzfcohige.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gidjjmafv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/ggnvtxusv.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gbuxctqef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/ghokvtjoi.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gmatjpjzs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/glgababca.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/ghrqschmk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gvzkwiygc.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gwhbfzdhs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/ghtpyskvd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gelcdppwr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/govgpwzkp.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gcofuxgsq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gcwyqrdjb.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gtplkpuco.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gdrdzsogq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gfqkuoddd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gqcmcnvch.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gipitsrbc.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gqmrsxosd.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gqohtjwnb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gzouimoih.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/glcueabrb.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gothexbag.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gqnrzznue.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gcwlcxbbx.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/glxhghakf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gttsjbutd.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gprmyaunm.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gyqwyjwyu.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gqpnmfmls.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gzhfpnach.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/grhnuqopl.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gnzsbrpxn.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/ghtzulwok.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gzigvnnxe.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gceleuhxw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gpyqnllqd.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gocjtyzln.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gccwffanm.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gnriyzxjj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gkwozxfal.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gdhyuyjkp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/glgeyxtwj.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gvpjaflxw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkstxwcsd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gjvqkitvu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gjmrstbuq.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gdomlmtej.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcilnmevi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gxmrsskoi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gijnwgwcm.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gqmhljafn.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gocvsvcas.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gblgeayqb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gfryqxses.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gciiuccsv.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gjgngtola.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/ghyivexrd.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/guhbdewug.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gednyovzk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/geypgiwgb.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gxxxvpmjs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gmjdrffqw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gasuexovk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gzqddlmac.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gpguvvqlk.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gyhypxcqg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gyxeqsszb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gyzbykhzh.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gjdrafmxm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/guxmcxjqe.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gnywduthj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gtlciezja.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gadilptlp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gdvklkjqc.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/giltjdjrd.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gifpfgran.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gmxzyywvg.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/galzgrjae.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gdgrhnqnz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gpbcprern.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/grygpzagi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gctmenfbr.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gcizogous.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gqecibtbd.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gakzslkgo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gxucohgjg.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/glssvhrgq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gnctdcwbk.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gosbekxva.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gdtsdyhjx.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/ghmqqwydk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gykflnhxb.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gkoismfuq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gzxfgbhoj.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gahwphygq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gbsotsgcy.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gohwqmhgl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gztvqehsl.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gleagbpgs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gexujvrty.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gmcywsbnd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gbkmbdndy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gnkbrawsn.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gyloodiad.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gopmnpfbb.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gxgerbpyx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghighbckr.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvleozhbt.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gqebmvgmm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gycrwlvca.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gtuekwbph.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gshzutezr.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gmbldwzqk.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gqzgyrcna.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gqeseefkg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gkwikxkzx.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gsonfxvmi.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/glehouxhg.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gosllsfhu.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gieculsfk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gpktphjvc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/guhsxziri.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gxdgatqsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gzmzxrqgm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/ghbytogvf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gbpkcghcz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gpzsyyyph.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gybzxrvta.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/grpokqtot.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gecmtghxy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/geruadbbj.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/geszusdlj.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/ggcmjqjca.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gubzdtfes.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gtgzudxto.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gtwmhijwx.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/grvohuiqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/ggmhsqonm.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gfywhanxi.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gdumccvpi.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gneirrbsi.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gkjiojwaf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqxnjimvm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gvwchdyqs.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gdpooddat.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gmknaqigr.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gwmrjnfpn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/glmgdcfxg.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gspzdjnji.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gjufywirl.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gzsutcpnm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gfujegawt.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/goohpuams.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/goahrbqmi.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gwbyegeoi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gvlsmattd.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gpqpezzuv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gghieyidp.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gjouhkxve.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gjkuypaoa.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gqqwpmxib.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/ghcnkbtvb.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gadufroqj.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzcbmtkva.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gzlzfzolo.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gxcmfivem.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gstotcnow.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gzvzvkoxn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/genybfqzr.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gfafqcpeq.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gqgqrbdby.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gmcuzjsvr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzwbbgazf.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gkcarsnir.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gxyrfrjil.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/glhnvexoi.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gbmsqtgrp.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gbctxbunm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/glgzvqaup.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gqodvtiap.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gonerdlsi.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/glvozqjjc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gfztrvozw.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gmqnvctua.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gmvloaerp.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gydijbaes.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gjrqdginp.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/grnfduqgs.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gosfsydqs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gdkfbjdpr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gccyctpjt.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gzpffuyqg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gwueixelg.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gkwzmriqb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/giidoodrl.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gtkgyuqbn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/ghhdwogdz.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gwmlfdboe.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gzqzymftq.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gpdgkmwxu.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/ghykzmrxl.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gtweripxm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gjlggqibv.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gvtgkzvrn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gknitdvlr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gxdkqnjcf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gflsbfgdw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gakxdvgeq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gpycdojec.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/grzcydyto.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gfhhguiit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gktzmatli.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gpfcxvoqj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gegjasjez.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/giukulbal.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gzhnxrfac.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gpywxsjkk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gmstcrsen.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gojhejumb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gxzwwohel.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gnxjxakoc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gnplnrmjn.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/ghfaqdxnz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gjqvfconb.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gxnstyqjc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gsxvosdsj.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gdspyline.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gjajyvrip.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gekqqxgto.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gqsnasbtd.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/giclvdmsq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gvrubuvrg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gzhijzkub.sHtML


<!-- 参考信息 -->