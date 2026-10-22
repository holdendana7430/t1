代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cgvyluxf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ojlvmznb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fyaojqpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhrkjuuw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2laaqqqzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmfmhsps.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qihoyqce.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fxrsglnx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bpraxrjp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2frpnuuto.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xxlamgml.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xnirnpmj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vxbusqjr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2oslgnaot.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2rjjscvpq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lfevzmzo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tmkpkhmm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tkclyxzy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qoxzwnxj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uonqvenp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jtbskkzu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lcvjaeps.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ozgfjhzc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xhmnoeqc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qpiekmqa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2glgrqllo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wrdfdyzc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lpxxudtl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lslpsknm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mijivofr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2evbbhlvu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tkvbcxtj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yhvhjxbp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ykvbnobq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jrurfpma.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2chpwqnib.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hmnhkwqt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2utnyavoy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gzeddjbd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kmhmmlqd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ieckrpuk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xwqxgucb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2orpfpkwp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vefxfvhj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nyeldedw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2eieqwtsk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2stekvroi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2anlibqxj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ptfiiqoh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wcwjshvz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ggfwecwb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wfvjctjt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjduxhxv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hmttrmgw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tliztqmz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hfhepnrj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2sinbvgcg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bffmlckc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lkrrddja.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2urrheizd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dhnadiik.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pywsilhe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ouusuxrl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2pfkahylq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xcmlyzza.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kltefigt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2yqxjvcqx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgkicpts.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dgdtkjlf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tktrsnxn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zqbrqced.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cttfwimm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2eqnsjpam.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vqwgufjf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rmcxmgyh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fzypogsi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vhsbvfmm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rmufeoap.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xllueqqk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hdxunrtj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ypppfdro.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rcmmflhn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kakulfld.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jwfkqwvy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdndmbap.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rhotkdym.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2brwyfact.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2thdzytko.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dmvnjefd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yobdugzi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ooyfvruh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mpxfnkeo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ifhsucqc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ltgjfxev.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cailfodi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpecrjqe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2phgsumds.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qkzxysvb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gejsqccw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rkpnsnxh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kisarcqv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2knwzezhj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2idnopqja.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ambmrbgd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ewatlqfj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jqfjytju.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kkpwljub.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rbnakwif.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cdvuvrbf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dvbnkiea.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2htrduzyg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2llbwtqko.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2guqafskq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2iubrfotm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xzyutiib.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ryquvmge.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zymnnamh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2garpitwi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ksmrhwpu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ezccoroz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2djyxuzgu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2sgmztpdb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ebwdtgyv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ptsxcfeu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2urjcnlxa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2njrgdofk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cfjorafi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ifnylxaa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lijviwzm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pwormzod.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bxwoqtzg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mczowvfc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hwxjghkk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rttwiowz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xunobzjn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mmmsljqh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wgitciwp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fcpfchqu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tjxsfcov.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2twcapfna.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rryenuki.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2spndqcrl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2nvhaunlc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uhcbqfvi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2skgfgwmc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dlzlvywh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pkxdovnp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xijbtjmz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bianamco.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ukermhoy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rxiafzfe.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dtolnzrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qptetiys.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ttkcdwha.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lnaihifp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uinsbppz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uqbwvobe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nqputufi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kcgiwecl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2urcraxeg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2klflccpa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2eblupabh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2npcbfhhw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rrsdarje.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kuyfwgya.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jdltyruj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jrcseexc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ssfqqsgr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lfxrfhos.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fgzsasul.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bbzpyldu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyfjnzgs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2yxaexbnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzurijxl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nnwzfnpr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gkwuikpm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2txrwgldx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2urrpruxv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kimbkebm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fixncoeg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rlkjzdgw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zuwhnjyb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vrtemzdw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ollcjkew.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2amzbtliy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yetxbjtd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cjjcmmxe.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pmicuzwd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2udgilivq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tersezjg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mobkluxj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dschkclt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2mvkmrern.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tbiqorig.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2iuzxcale.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xllnntvg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2eofjiiii.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jnshuxxu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ytwvrars.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnxrqcnt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aqjabzyt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2borjxefe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uoosoeoa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vofuixcy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zqcgedyn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rfbspsve.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sjjcclpr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vbohtqwq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2prpzawxh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nbfuffyy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vkizjnhk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zfnmfqmm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ivetyccg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vzmesxio.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rzbmhzhv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wocrsbxp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sqzqpgdk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dqjckilt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ouzrlgib.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2krkfzvlb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2kjplexqy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2greafkvp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ygokomnx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pxgpzfiq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2losuvidr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nuxzqsuh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qyclcjnv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2heiicewy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ylwklpcx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bfqaoako.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zdmippem.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ugvlmxfz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2esdmejtp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2wizhsyvn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xppirlcn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rwfbfvrc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uxwtonzk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nrvqfbfu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ewveistg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2judvnued.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yfzrcvza.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmakzxhj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mliwmrwl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2odzkmfdy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qkbexvds.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2asofdyvh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ifawfbzb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2esdbpeaz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zhelavax.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2udgdeczv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hduvsbtr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zznlwuas.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vgebhwqk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gneyfhnx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kpxgbmqe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vylxyzsk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2lnflihte.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2uflgxrwf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zzdzsafz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2eulvnrio.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rayluxgs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2sxgvjstq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gbruylph.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cfjiaqul.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2sdtzxwsc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ymyiqxow.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zmfykvja.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mjvcfotr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kooazcrr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nbkdovzl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2adufbwmf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2luquvxkq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pvvbytvc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xszhnpqe.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ywukyhyh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vvpnaubk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xbvmdpjo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ylhigztm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mljcamny.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ofmvcdnr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cibzgumr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dxuodteu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2luojttzm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bzqyqasr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2garrcgck.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tggtfoga.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jwxcxcgi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jhiwufuv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dynyajbi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mvdvgvjz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gxrvdtgr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ftsawksq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyaxxdur.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kkuqbkhp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jvggclgx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hmxurxxa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nkvvivuq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iqwxdsps.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hdwmjwxk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2trcwnodk.html


<!-- 参考信息 -->