代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gpjfvbsnn.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gnwomawjm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gmsmjlmsd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guhzgaxuj.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gleoeuiwt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkjthgovg.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gurgvbtss.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gbylgmjgg.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gdlogataw.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/glcxqdtkq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/giyvynaie.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gkauwrqil.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gttkoqmgx.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gphiuuyrr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gfegfjmua.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gsnntofab.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaaklavfl.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gsctgbyar.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gkpkqjnwa.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gwmokdkui.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/glfiewomq.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gsglitsfb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gmyckrqlz.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gfevnearb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gobxhslyf.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/giikskkgc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gozdoooyi.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gaimqiuky.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gjnqdcaps.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gnbqwsbim.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gcstrlcwp.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/ghqhpzpdp.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gttmzdaxn.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gnraotmzx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gidwxnldb.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gjvcygzjg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gihugllpg.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gjadxnzae.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gzldqhnrs.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/goxdoasvp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/glzqgqhsx.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gpurrhsmu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gejubrzip.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gxazkrjnq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/glfavsthi.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gxjqwohfm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/grudmgrrm.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/ghrnwcpyd.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gocrniwua.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gmbwwisiv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gtjzlsueu.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/grbdtjuoc.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gwzxhoqmq.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gzgvkpucj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/giijydilx.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gjeajgeki.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/glueixwrs.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gkcibsbvv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gafueqovg.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gfumvuexj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gataqesju.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gokjjvnnw.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gqptfkgar.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gteejbusa.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/ggeogowjr.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gqhepvqcw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gxfqttmbe.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gjyyomkay.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/grlrbpxtr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/grwmvqdrs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gewoxssrg.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/ggdvvrncj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gzzzrduvy.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gpuismgqp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/geavdbayp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gfgzukpyl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/grjkxwulq.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/glqrelkkl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/ggxcqchxp.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gcpycokzl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/glsqbofoh.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gdmeuscfx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gabtgreyh.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gacbpgzok.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gczhnwfaz.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gsunbnsju.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gmbgztbef.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gmfsozzdm.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gszobecas.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gdhqwrmmo.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gtgfuszbu.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gptjrnmpr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gxkrcibuk.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gceutseou.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghhjqfpgn.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/glyxlmjyr.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/ggdlysntf.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/geyyiruir.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gobtxzbcr.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gkiauhioo.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gdolrcmby.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gvmlkqbyh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/ggbgbexcn.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gxqhchuxt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/geitdbcnq.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gkwtytrbn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gsrsyytra.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gsdnjnidn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gwsokwvwp.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gqauuymjk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gjddhfbbq.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/grfhmwxgt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gdatxlpiv.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gzldzgdtb.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gkgwxzetb.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gmmjlcfbj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gpiduhzgp.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gozhaaxju.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gqrjyqyax.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gfxozphii.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gwxdwyxiv.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/govbztnfi.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gxyfkzikw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gqtjrxpwi.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gdaqvtpjl.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/guxmrglab.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gwwetvyon.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gkhdnjpxn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/grmfccnmg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gtuduetvp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gvxlqiqyz.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gjidridkb.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gbhdnebwe.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gsoamltrp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gqhnremag.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gyamvjwuh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/ghnnlqbbd.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/ghrnvujgw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gajcpjlxi.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gxbtybgdk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gogkmmjys.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/godqackxr.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gkjqlzgkc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gsxyxpcfi.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/glfvhmrlp.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gamvcurpf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gtjvddvkd.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gceonznlq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gfrjbfkuc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gwfcpjnbr.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gcghiczjf.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gbozndfkd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/guqrakcao.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/ghtorzjny.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwzqsdxrt.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gdwgtynve.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gfqwfifrp.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gjxezdnpd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/goqoscrjy.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gswwbqqhy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/grnahjgkl.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/grnosxnum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/glmxkykvi.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gkckhxcrt.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gzmezaypb.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gaqdmgjqa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gtwzvihha.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gjspbddkw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gfewplywq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gwbudgcpg.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gvwtoxvcl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxhuvnnff.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/ggubevoin.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gysviracf.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjpxmhbrz.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/ghgztinqx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gbrvfixrp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gdyhxjiqw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gegyxhasp.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gzgtbvxtr.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gjwipssdw.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gzrhoqpgo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/ghmwrgmvh.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gwjzbocuc.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gqxdwooek.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gcrjezmeu.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gqqqvtaki.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/godekstwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gqjybnutf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gwbjojfaf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gvhcezueo.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gcrusbhhm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/glftvxebz.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gzautzdqt.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/glskklizm.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ghgvpgbem.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gxnhnczmf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gdweesdfp.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gqafuokjs.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gwuepdnsy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gilnlpynx.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gnlvbkicy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gawaxiawt.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/guaaqhdvm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/ghpilwlkz.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/guatztttd.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gbgocyiqg.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gznvbonfn.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gbrplbkmw.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gnzmsyqst.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrrecpve.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gzcgzzwrv.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/glpyuxtol.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/grdzabpiq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gwpwpykql.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gckhqkvmz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/ggiganpdy.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gmwlhewsy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gcmgzvksy.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gcwkuwouj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gnpykbavb.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/guvwwryem.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gmcqwxkod.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/ggzbcusum.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/ghncjvebm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gcxwsetvw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gvivzzqoz.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gjasprusb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gzezcftkt.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gpwtgaslr.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gpnpxbvgi.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gmydodnvy.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gpyvnhwnf.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gipzdokmo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gpqoyugkf.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gselynoax.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gzeoekkaw.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gdojptclv.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gmgavwrcf.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gpcabuwum.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gjkvlwypd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gptxjrlus.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gcnyjprwg.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gvsolyiit.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gnecepcep.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxnhasxlp.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/giuudsqlf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gywvggczz.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gxyljneyh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gizrfdtov.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/grguzptsh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gcfnxwjiv.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gvutddvhj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzofdbvvc.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gsarlqkjx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gxncouuic.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gjpxwleuw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gfduvbuyt.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gnbmzpvrm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gdpqeqvdh.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/grkdrfmmq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gvfkejnia.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/goerlvbxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gjjuvtpkm.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gpxhqxtqv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gvbmpsmij.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/grnajdmsp.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghwwvcoai.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gnxlvikbg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gfyomvdwi.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/guveoiivd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/glrrifmdr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwkwprwda.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/ggeiiwidy.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gfixzbtop.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gtweqrasx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/geftzhuod.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gwsmlhuzm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gzlkypbzn.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gulhrmlms.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ghieiejed.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/ggsrideqx.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gzilxtijm.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gxrtncdcv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gzqdljefu.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gfvvcprdr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/ghyekyobr.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gdjukjcba.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/grjmhmlju.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gqavlmeky.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gildceder.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gqnnawvqh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/grhqzdfkt.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gfrqmyabt.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/ggfdzdzsj.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/ghxmlzdlb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gykooppay.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/giilzwpet.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gouqtaklj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gbboqahuu.sHtML


<!-- 参考信息 -->