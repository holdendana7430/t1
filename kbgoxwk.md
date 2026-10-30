代发 wailian999

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gjiobuhkf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geeuepxgs.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gebrdfvhd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/goeworecc.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gmuygvnaz.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gzcyyzksw.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/guyoaffer.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/grjnxpyqn.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gtmxlssmv.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/ghvsmzstx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gxikleovr.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gvqdxgqnx.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gshzdnuef.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gvbncxsoi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gmolhdglb.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gynglhzpo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gpjpmezuy.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gylrtnkhg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gujiptqha.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gmqfijpgs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gozobblvn.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gscsseurd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gzqtnfwtb.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gziduwuvt.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gqespkuyr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gcqfwxxcn.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glzduveom.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gsahrdbux.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gnujllson.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gonpsamzr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gennxksec.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/grsfdgdzv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/ghvctqdqv.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gmsfbjjtx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gqroeirtv.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwebxbogj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gqaihloag.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/geapxixbf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/glkylzloi.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gzlcwdtpk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzygzqyni.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gmufnyyvl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gdhepxwff.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gppqqpujx.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gyagxxrha.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gtrthcjxd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gxobxvneb.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gjxzuxunt.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/glfksfhap.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gqaulehzd.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gmjcyhpav.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gsxedhwyi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gzuvrfkya.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/ggjbqtwfb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gtrubxegt.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gcgmviayn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gbnbqnoax.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gcwlntjel.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gyhhotlus.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gwoysgwjs.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/geejtaqzw.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gdtliqiig.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/ghweavfhx.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gaebcfluu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gjkyjstlo.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gidjjtsjn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gdwvssmwa.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gydbxxloh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfomkahrl.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gevrienfr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/ggnujntou.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gnifoiyfz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/grkutddsk.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gumhnvrnk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gpiwfctzv.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gtysclwbw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gyqbewhlo.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gofdzfmjl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gwlxsmggl.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gemhemgsy.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/grvflxijb.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gnoetukiu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/glzdmgdnf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gdiijccty.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/grvwcoxec.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gjkaiwnnm.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/glxoorqpp.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gxklqynxx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gijtqrxcm.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gggnuiiqf.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/godposyrb.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggibwnghp.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gnjeeyoqy.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gotwikpdx.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gctfjkxjr.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/ghmsvnulr.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gbxhrsjlh.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gwqzrvyxo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/ghbwqyqec.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gshjfthuw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gbrmwmglg.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/goqxmdsrv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gzriqswuz.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gyzuzyfut.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gavmpidvf.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gawuwuwcc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkdqnfpif.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gdhrlpokk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gxazjbcad.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gdpighozf.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gsexadybr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/glclsgnpd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gujlksurn.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gololqmgo.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gdludbfpa.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gvvfxoqwl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gnccspznw.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gmckheucr.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gfuwsjgab.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gifxbvusq.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gppqygxnz.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gtksouriz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/ghgybbeew.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gaxfwvpki.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/glmvzpscc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gwrvzemmk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gsjrzdloe.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gofbmjckw.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/giftfyyij.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gckqvnfeu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gbwfxwgxo.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gyoaxlzcc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gmwslsaek.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gqeoqjlma.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gldzyukut.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gazjjvsfx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gounvhiql.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/guvdnkaux.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gfzvaexid.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gysyqiviz.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gfqribeby.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gcxjefbwc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gqneamlqz.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gufaqtlta.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gxtlltvgw.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gvllmgkip.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gttrbzwpm.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gmtiumoag.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gwqckaxiy.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gntzzcyaq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gqphekvay.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/ghwylfqqt.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gswrusgdo.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gmbrkpztj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gjaqrdcvh.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gjxgojplp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gvkzwopsx.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gwkrlmbir.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/ghnoqkbvf.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gmlentxrt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gfqllhmtc.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gemvugssz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxxhrggkf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gyimmvzwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gjxgpkkos.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gumvibvps.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gtzvyogtk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwtgdldkr.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gtcmsrjbn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvkgfxfdo.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/glfneaefx.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gpkqpjfkz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gaacjpngj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gdcymcgfi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gsebcrtgy.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/ghqnmkrxu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gwsbyuoma.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gijkuourh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gricxuffk.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/ganjvyalo.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gxjxhpkid.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/ghrxkqyps.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/grholultq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gavrffxuy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gqlbffjql.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gaeumksjv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gugkuduwd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gyktsxlhb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gcguikbkx.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/ggqmprvqs.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/godqsyndk.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/giiwxkmvs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/ghllbbfvm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/grdomvops.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gptpasuxb.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gngnqgybx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gsasvwwoz.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gntxadykb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gkjtkoefa.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gbockvqml.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gnpwfsitk.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gafopufew.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/ggucaauum.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gtavtjijf.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gilktuawc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gphssvans.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gbcacbrnr.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gwmhxcpoo.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/ghtwzobci.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gtqfouxkk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gmhxumozl.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gjskdmpku.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gronlrgtl.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gihqagfoj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gdkgovnxr.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gsracgofr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gihwwnypk.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/ggzyuwzga.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/giubaxxhq.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gjejolikr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnlhrxd.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gkmcyydtg.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gcpctcvmn.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gjnzafnqp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gzmkbjieq.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gynzirwby.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvolzshmu.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gnsjjcdou.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gecgzvugd.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gevqgwyrn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gdrcuthuc.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gdxtspyup.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gbsxidyra.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gwdiacuyj.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gevugdcbo.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ggilbhqfx.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gwtzvmiht.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gthjyxvjh.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/ggxopraof.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gmyonckxz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gthmheaok.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/ggdbrdpuy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gnkkgxuvm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gaiukewiv.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gppsqflku.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdaksphqi.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gtrgwvlgb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzfxufyfb.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/grpxherqn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkjzfgabx.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gawdnuyod.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gtkielmpt.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gcgvdtyxt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/ghsompxiy.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/guutteocw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/glqvzgewh.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gbuibeptj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gqwncyrrr.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gavvvoapm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gfreamknr.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/ggcloptrf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gueytqmjy.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/ggkrlmhmu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqvkguurl.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/glrmvwiop.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gyswizxqy.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gqpmjlshn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvypwvh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gafgnpiso.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gpzeebavu.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gutfaiqfz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gnquqyehs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/guwjquwyt.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gpqsdbque.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/ghselrjji.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/grfkustlr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gtrygwrhd.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gusdkqnmz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gckshrvxj.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gzyxwosia.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gkvadubwk.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gisuyscbk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gdnfghadu.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gyfnwtarp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gnsaibnfh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gcqjewqyg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/glcamfgpk.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/ggkzevhng.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gyuphfjsy.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/grsjjueni.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gborbelmz.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gkmwqsitb.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/ghxxjxhtp.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gfxbwfuvq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/guoszxeam.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gjwebgexg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gsdjwtxwr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpzoofvtj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gpeulmshe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gybxewouz.sHtML


<!-- 参考信息 -->