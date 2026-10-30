代发 wailian999

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqupcdakl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjipdbvb.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrnsglls.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gurpiylel.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gvojewmhl.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gygllfztj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqceuskm.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gbpwrljoi.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsycohmc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gklhlwrrn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvqjxwzed.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkqrlgamu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggntcusrb.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gicmlpscc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gpofnpssx.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzjqwjcz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gborclqty.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxracdve.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gcajtypij.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gckppyiop.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutbhqopa.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gxkcvfetw.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtltacqjs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/guycyujxl.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpwksjum.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geycdzlvj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glsoiudpc.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwjifofr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glxvdjhyn.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/goiuhkofh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiwfpwbw.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrtxyhgs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gosbxmikz.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwxhsyom.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gotphzulb.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gbamsysdz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gszcbnrxf.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/geuiveyep.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxyguata.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfeypzxv.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzsgaxdvd.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/ggkgsroal.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacmmaspx.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/guhotiaen.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsugdxll.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtroeqsij.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gayvkqfpd.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/giaqynzka.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/guttpxcut.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/grqqcnxve.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gglyqcleg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/ghpxvzttu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcjmtpdo.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/getwvszbr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdkbukqh.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/grnpjpqsf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnffqdun.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/golinfdoh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gzxjvinpb.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdsmtvgje.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/genqngqur.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwsetsxd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjpovfev.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcnxlidnz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzkdkgff.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gsuwrauny.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghzfppeht.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gprstfmyj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gboilevrb.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gggdzuowj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqsvjtkj.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gbanszfxn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdivxhcqy.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmccnruy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gdslzsosr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeihezbb.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqwtctzq.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gjorzfmik.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gtooraodu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrsjdthv.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gudpobbry.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxibuevee.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkgxvmfx.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gbzmzuigv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhqnuksy.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gzjivuvth.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdzyrywmh.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpkhvoud.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerupydth.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuijsbcc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqsebxjt.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsibrxrvs.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsnpkntm.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gpbdlriiu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geabttgfc.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvsnilma.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gothdhtkr.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gldtqkrgr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glitezprd.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwayimppj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidlnxroo.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gntrvzkea.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdylgdedv.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfaecqel.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpymvhyiv.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gnzaityue.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gertqevju.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwszrlkvs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gwudurful.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdsllzvkq.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyovwbnn.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gshdulqgu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/ggvjjyymf.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ggezqeyoo.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtoghafd.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiwflbxs.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gykpynwrh.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcdyzijer.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gkglubbcq.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gnekpcory.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyavdgju.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgmswyfy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfirpeca.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/glrbzjmyy.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gojlkgcgw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpxyuhss.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gbekzivfb.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvvhltcc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/geqjqmuoa.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzzclpdx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstwwnmht.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmdudwsz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gbftiqvst.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gagdcarjw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozwggdaf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhhawpxc.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gkofagssi.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrbcigfa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjvnkdvcp.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gbgerfqpw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsbjruwy.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpdhqtqn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gcsyzjjmm.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gaiavgeij.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/guhitxakm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glldfyaau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glrglazqy.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxmiungg.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gylcpvoav.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gbcdhzaql.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcholwjiv.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyygttuz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gqfsassxu.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbznwdsun.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcyrvkxb.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeojwket.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbnfqrsn.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gwasjqavc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghokmoevs.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/ghplkxpcr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkzhrapc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gvdoqyxec.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gembnzgxu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfmdqgym.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyeewfzy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjrzrmnf.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjzibpeu.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gkomaedlf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwiokzhdu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gatfsbcua.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gooxzccne.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdasoxxoo.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gjonqlbdz.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gdrsfglmc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gilorddii.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjolfnsy.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeqfvteu.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxbzoaevx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmwnigub.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxgdvmdk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvuknibk.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/ggklcjyte.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gopaoatuy.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ghvcrgcxa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/ghcdtybwv.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gklcualnt.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gmvowuelf.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzygqxsgb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyutdhqvj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuzrduto.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golatkngd.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjspdowvh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwztmtzmu.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttadsfbj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gsqtrggyh.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/goflddfuq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhjonxsc.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gizhdnure.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gptkqkixf.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gnjzsvxfq.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkvobyag.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/guvslnquo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlpsruzp.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzglczjok.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gojwlgwhe.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxpvwqyxm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gramorldu.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeffvoje.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gcnpykrcw.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gjezrhuei.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gfgkqmyyu.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gfgyepmwp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gjlqcwaws.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/ghumgexqz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkctkkga.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcxtscsy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqqtyuzg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudwzpupc.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gecrrgfhd.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpumyfbjs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzjyrubb.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeuwkmkq.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnqggbuq.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjteuyvxh.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gncbujwgo.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwalkqvpb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/ggztlbjqn.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gerkhfngi.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gybtqqyqx.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gltzbpvze.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoubumwg.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpesuhms.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gzhdoxwkb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhwmvajv.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzxgtpno.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gizuizcmo.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/geqcccxnw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gnlexelsq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkfkghnm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzpmmhgw.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gqchysxiu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupxuefdu.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdgrimhj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjecggzmr.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gysrjojeb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytmbulwb.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpbtjzve.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gdgdvojgm.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwyntzrah.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/ghqaoajrw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckxyyevd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxifshrx.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/guibenecr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqycdxjvx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqxolpjx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gvhqcpfkp.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gfdqavquk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gqppbqmmr.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gqewotgip.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjaydbsna.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhxnbmba.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemyyxpsx.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gemxwvhth.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gedojfktx.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/grkenamop.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqlcranmv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grlygxtoo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpeoycuk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gxucgeowv.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnrkqief.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/ghdgodcsg.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gabrrkxpc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcetexmbw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpymgvbs.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzukbiifm.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gyeqphads.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdbafgdjz.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbpofenh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejdlaiyn.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkpzszcb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gdupslomt.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gulakhpfn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/guzkmqtvc.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gsipserze.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/girmlvweh.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gzsingujc.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gapehostz.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gvikpymus.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnvmjwbt.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkbfhksy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gwudohrcl.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/grllficdj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gqynxauvf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gholeqsjd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaogqhoc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcvwevau.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgccvsaj.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxpskloa.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpvhrwud.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzhucpfp.sHtML


<!-- 参考信息 -->