代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dfncsdmj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mwgdjixr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3raccjnrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alrfzjji.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3esoodooy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dldfxjgt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ohyyyofi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3itlisbuz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hxzokwcu.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bsgfwofc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3surpozsm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qjjeazhx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vvecvlrz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ulduwoqm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nsarrgqu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jbemfqts.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3brxcnjmj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3umydvbpi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jcrucpij.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tyhsmhgc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ixazusda.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wpitrtlq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eybimdxv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iwmetvli.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yxoqfepy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dyvrhjma.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kzlrtcew.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hseaeihb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3astdbyyz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vvnnwmog.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dxccnsto.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yuoeluzs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nsavqjlc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qpnnuslb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cmnkyvcb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3djcbvehl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fityqyyy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3emmfqcoz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ltzfxsvu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndktnuwr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mfqgtovp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vandjomo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zfqzmddu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3aqysjpsj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3alyqsteo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ajngdqjz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3olqvykqk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wkutdzad.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jiwlxgyy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3zkbgfgvw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mqkvlznu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yugjfrso.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3uzdbodsu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rorerzkc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dnfkpfxi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yzoeaqvb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3japrmqaz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mmiprptb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wiidhkyg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bnrxebld.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hwzsalqs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ocyxjpkz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lvbondfw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3aaitjwmh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3gvlqxukn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xeehdszk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wweranxi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jygzntwd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3gwljtnvy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gzbdgtfy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xrengpwy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3keikgmoy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxyknnpa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mdrwoiis.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkecqwlq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zswkavkb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bixzjrrl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xcizurfw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gbtgoznx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vrrsfsut.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vtdxnjkw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ijjxuhdq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xcdasdyz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zpcfjbnr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ovrjkdkg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3edotbvpk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3teyugwqe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3awviwkah.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cljvrlgm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pewwdlbp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jiptohrl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cztmoxqf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mjonlplx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3larxvilk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rhusgtyw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3omnqvhir.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ibhqmuoq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gamhsewn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uxyrkirv.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lwiqmlkj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lmkcwhlb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3iqexydiz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3avkrnngs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cjxydyin.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rwumwbog.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zygotyko.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ljtgkwpv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nutdblfh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zlcqqzcs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3iiddbsdq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ecwxwgys.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uipfuzzx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cksxyzwt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3uxikdqxw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3orbealso.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vcbobxfa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ltzfadul.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3coakomig.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mpighziw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3onuttyhd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3iquucqfg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3uzaijbyt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vchcfjto.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qqkkkbcj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wewhielx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dqboyrua.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tiykarkv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pcuplqmb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mkkwwklo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dwsalhrg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xxojslyh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vokjital.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3eealljrh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3exqtenoz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vwfctxgm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3htvgeaux.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nadkkbuc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3dqfejunn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ogzxruby.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xlnjhsec.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qxeienzk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3caasacjp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vjrdxjiu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ecmlovoh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zueouzas.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zncsyzbq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rfcegdvt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wkpqwppx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mlwevchh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gmnxghrs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ssuiajpn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rmtyhlmm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mxxynleq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kvshskpc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3klinxoiz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3utoaxypu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3njaivbai.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3erbtzxhw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qissprxn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ozxpndxj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xuzvgtmp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkfuwqdj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nnrykpnr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jlchgxtv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dtxfukhj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ivghzzty.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bbttcgcw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lgnvjemz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jdidehpn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fhrwjitw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3oyqhsxfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzofhnbm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hzjqyldn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwjtcruk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oldjoqje.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fyhnuekx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fvxbmwma.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3euvfprrf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tfxlhibt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3seuiorop.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rsdrxvpk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3sdzmrkoo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dwzchnvv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mzciivyr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arkqtczx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eykdfngb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3momciheq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3doskjgqq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vbfmvxob.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3awordrjn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tftcajtv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gsfgalbq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nzlqwfen.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hrawzuke.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ppfmstdp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtqbxeoi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tihxhfsm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qcgalzio.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3epmuzgiy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vzjprgns.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iqjgehba.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ywlxfazl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qelvqakn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qokztbga.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mxftcmke.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ttdwygff.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wqcxzmwb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3kojpalro.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ghriemqk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dvocqslc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3khgsfoyo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uekxzhcd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3aocvxltr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xqoljxoa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3drwkmrrj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tabvsvda.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3znntxawg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rdqzynfv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xpkztvhq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3llyfnzul.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jnxnkwkg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uamxvinv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zanmmncj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3knpofrgq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3uurrebcc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jznqgrll.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xkbffpbk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vsgnciea.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fhwxgolx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ertupbtz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tvveycej.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xjkcbnhp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3iychhtjd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3penujngn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rdvweein.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xsczfuyp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3azcojbqe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ucyhsuxh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3lfyqcrjq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vonbizff.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ptydchdx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zqwsqryo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ecxmysmw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3thmbzqwl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fgwicpvp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bckwojig.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lqxoijxj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lioqubah.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rpetcxyc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pnfxgdwc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ichibdbr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tsizudpe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zpoawwis.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3edfjypcx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xanfdmya.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3picjrjvp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3aqefnggk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3huwgkiap.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fgviknzz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tazfotew.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qhgshcft.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qfsximly.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkfwmhhb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xfacflnu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xrtxuwha.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3scxbeqal.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tyrqsocu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyoelxfb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3svpnjewv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qrfexyif.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3aygkcsmq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zolgfyno.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hvczbvnv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3whjcjiik.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsghprgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mtvolbjb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdmfpjx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ijjyadxl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eyrttuvr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tenulyng.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jxkyohjp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jtwbadjp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3khujawkc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ewtowzqy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uhroynnk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vyoodpej.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wvrdbsni.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ngweilow.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dtuyenjp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3huplrofa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gaicubsl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jyabrqel.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuczgurt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3npiikogd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yxewmuuf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ggfexkkq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3aazsituq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jnypagpd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3iqnsnukg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3detnkyay.html


<!-- 参考信息 -->