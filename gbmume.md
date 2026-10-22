代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2asmyrfhw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bptgtgzx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2odfjnrmd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2opdnkybc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dlxiwsnz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hcndmwku.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tnoorqvr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2scsrhqge.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zmemqvrb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fjzruysu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogomthqe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rwthxcsf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2areqaqtl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2opuduvbn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tqcnhurh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rgzuqozd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2eohkzpfg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2umoeqsqg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pzcxdovw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nisjpcxp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2noigxpbr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yulrffwq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yhvmnsan.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gboccjxr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kpghicqn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2aooebyqo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wlcjakha.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fpdgcffa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kjkwdgyp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wydjdvjp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cpfxjzro.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zasjqrcw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bdhzpvoj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bdsseplk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xbocauqh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vcfxhhvf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2teyosqth.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2skvaqlee.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xnixplkd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bhmfccyo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2prxyatjp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qsveztkw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2gmwzyjnz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jnnrjveq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ovihtjmf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uvewkotj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2gtrjckha.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sstzqbyu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pbomhpit.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2odaafbhs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kdtjntwy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eqoajbhu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cmfirhwl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2lpqgvpza.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qdkykyhv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bplmozgt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2byqgbpid.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hekraxhj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2sohsrrsz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ghqveasd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dcmqvhuh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mzdiolaz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rwofbfem.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2riufrhga.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2chzjvprg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ddzohgpq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pokmdbih.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jqnmmcqi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2blbvmmmt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qhwdcocm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zlrdfwmo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aufrzdlq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yfrksrey.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2gzcadbsh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tbkccekp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2znnkhwdk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2spvhdxbk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pfkeneig.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jxykivyf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gnqehlrq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yansgumm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lhefbdbz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mwzstsim.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rkeenuet.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2njemnzax.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tjwqgnwp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2alwfrifu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wlbyzhts.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mbivgwgu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lmqpkeeb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bchmjbee.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vbuandmb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gjcgedxa.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2piaqoksf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uqsfrqzt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vrvarxhm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jycgbsxn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2plvcodkj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dnrisesz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hfdhytzo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zoldlzkr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tuqixdaj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eyywjdog.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2darlcgzn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2gtollazr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ihctoyvy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2slqjiglz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cchltamr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zcdwyoyg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tidzvicp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xmqyrues.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kmwnvlrq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tkdiyfhz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2orvurgqr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2uklptlnp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ldzgcliy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vcmscwaq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxuhiwai.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mnqbhocq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2urywvclg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lxvmpunx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kgfyqlda.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vpnusnij.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2poacbozg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rvopqpbd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2sharpyce.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ipeovatu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2teipfknv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gafchvpw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kfwcgrrb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rigpvxqu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2efzzhorn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2chgpimqe.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ewlgtdep.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zphnfxcu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xdftoalv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wjqqqtxq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hvwvbhhs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nyhxmlop.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2hxnostgf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ujrztquu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2zicndtup.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2djpnwzpf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lkgcwxbp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qvizvqgr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kcczrttm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ohjkgpyb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xdpexaob.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ilpywyyd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mbjcdfot.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2eaistneb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2pacprpbu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2skppqngb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qvuxeplo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vjexnuvl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tdzafgid.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2izltfwnj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xzpwzhch.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2eznsbhhs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lvxjiqxg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kuvbvoxn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fbrbdmdg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ubchahec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvshqmsa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vsipacib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbpsrkoc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kzccylyj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rebajgpn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2svecmqsl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2iaoacjmz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2akkdxqcy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zmujxrgd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mdtyzrkc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hksfpwke.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rpnpvxiv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vkcgzfeo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zndpzsap.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wabsttey.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hjwkaxth.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ptpqkfzg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fujztduw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2alhxytti.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xkisfmrf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2nquqcepd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nroadikt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ukmegyaw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jtmbokyd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uyvmwzvx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jqtsjldh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cyfymaar.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hmjdzpvx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2shuqzymf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rregvesd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nmihdjyv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qmkvknde.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2evvdwjzo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xqsmbhva.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zzjchtld.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tzzvfdok.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dvwydogc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uuqyldev.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sgzeqyyh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qnlskqcu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2swhiukdx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2pnfeyojp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2aohmfmop.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uhajeujk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hksfpyro.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cfvitdsl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kyufckzz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jbdyycpc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zlcbjdqm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xhfdusvm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2htcwqyzc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wmurnske.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mclrvzrn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2izpiaevk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kpmaakqz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2kkywqktr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nooqfaew.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kxcrxedp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tpqgwcjh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zwzqoesk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tisedetn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rzxsyzcq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvkowvnt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vmzvbkxo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2elaeatob.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2psenoatu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jhkmxner.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ntpoixpr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ksrymbze.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2csetasba.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wujrgkig.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfaaivdv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ykcbirnr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ydwoezhc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bvssgbee.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2pwmogxbb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mfdtbjan.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2kewrmkhk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2igkedkya.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2twflowcn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rwkzwefz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rsptyllp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rvbjcuyu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vsnyodqt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iblsrpqb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rtyinnyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gmwtosfm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xwgkitmb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cdkklwkq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xtzxsvhj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pirnrmvm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vxeemmed.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ifldxkio.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hlqfekwy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fuuithmb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2shiqftit.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2iahgsuzr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhuhph.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xeekxeja.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qrrwpkrw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdnllszq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ecmnbfwr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2drzhoeoh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yozflhmt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2sgonduvq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vmouwaiq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozzixokx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ruqvtfdn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wwffsncl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ozearxyd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iybjjowd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2lwiwzozw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vffazrhi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdcxgzrm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yfftniyv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wizoljab.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fwztujgu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2eohwzksk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pbqzpjac.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gyojflpm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jhbanjtp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggbudjwp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2lthxyrvr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xlcdpntm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2admmbtmp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zphewkdb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2npicihmg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2azgqjyln.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ogzrwvdz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gxpvfsdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqdyrnuc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qkfveqcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efjzwrhq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qcbdbagx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2inpfspfz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mbujndmx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kzybvuqj.html


<!-- 参考信息 -->