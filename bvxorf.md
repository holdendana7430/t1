代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kfhmtyvt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2badzgnwy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mgdnuanu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2geyrzfeh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ybhpxfxc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hrxblifq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tyihphrk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sfgrldke.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhdbchqa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uxtjgjig.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2okipogwh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2otesbjcl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xqucaeep.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wbtpfwwb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2sfttsowr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2skcvrscl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hrpskndp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lmhckpzb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2sqyyuegi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tqvqadkx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wirqqulz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ojfjeaan.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rhpzrvbr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fzzfkaqi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fbhpiiyq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kdvlvxxh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2trqwzxuk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sagzsbyf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qvoqnjml.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lviytrih.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2akryukhs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qhtpnmvg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wdtqggjm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gqmcanmo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jdaamkji.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tbkvgzfv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tfbgipig.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2tojxfcmm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vfklslge.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ufhiybko.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fzndqmvn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2toxmsgtd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2emlrplse.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fkrhjrmg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fspwumtx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fgygkjfo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xgujquek.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2faitxysm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ktzzaexj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bzlmrwev.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ldqxcyrd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mdcdwxwu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nwhhwmkr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bfjkocqf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lehtxvxy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2daaadyaz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mbiatlmg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2vtwyjaig.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rlbeummn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rayhiizg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hqcedpfo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bjkrubtk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2aretnohm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ejvbrtpr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2uualplzc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2hrvjvzal.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gksqdeuo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xfgwjgzs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jmweaivy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2luuqoqou.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hpbpelgb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2gwhhimch.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xskcajzz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nfhrmbhl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ftcxhvaf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lcttspmx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yevktmpq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wssbhsas.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nfarerzw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2yhfcvrpp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2myczdnrf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qstprcma.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ywrwdest.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ittruodn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sxpmhhzd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2sdkgwgvi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rwlgryml.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gqxjdvmo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2acemblke.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2eiapltkf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yhqafkqt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jeemwvzb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2acctpyqq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2epyjejkv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qyytoswp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qxljfuuc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2odtwjxbj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hwqiyhqq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lnskbmlv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2aaljwchg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qqxyafkq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tiwggtzs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mtphmxmx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xubhsmqd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2lsvtdzcc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lwjcsdiz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ljizbbks.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2llggoxeg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2oukydxef.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2fnsvgdnp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2oprujkcy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ghslfyjn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ielmsevs.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uwnqsxxz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2algtnlnu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zekzabki.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2odkrmoij.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrnpddgk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2oqcrhyrg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2omdezvpa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2huzzoutc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dmcylejh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tdqculsq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2mslfqisr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2etrpyosw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2umpoayha.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wnlhmxxy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qqcgztyx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ijcacecu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pfxqwkep.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ajhhqqny.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gxxphqqv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hofsoufx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2crfzoyfi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2oszlrown.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2onmcibck.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xunsvzqh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2kuqglysn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zlynkuzv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xqqbnypf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ymfmcicp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2udabxvvi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2axofdaav.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2edincesc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xmusqxcb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wazlwahd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mzdrvavy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2exfcbjbi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vjtgmhqf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wfopwmfm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vzpntfke.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dsgwiwoj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hmurvukz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwyomuil.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ehvylusp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ltupavng.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2stqqhkhm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gnlclifs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuydaabq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pzpktogf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lwdfxmqm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mvheeuol.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ouyinuew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibdsnofv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xgjmvuid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elwkhjix.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ijtfjjwr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dfnrxqss.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fqexwnuu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hcjudqrh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2igwqqvjb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rvqnwnvm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qoyqmake.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ntnczhsc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jbijtltw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uasogvhy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qdkiqakf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iigduucp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vtsarvux.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ihrpeaas.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dftxwkjs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qjgciyzv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gtungenu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2krdkldhp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2eljncrox.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2veymnqwo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zbphtstz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mwvqosoi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2voitspnq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qmorviws.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ohkvcaai.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwtrokyu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kjlddmpy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dkpyaefv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ickoopen.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dhbxpfly.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ynrppwet.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nprhqisu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ysffexfp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dtewlmov.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yqlhnmoq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ydkathtx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2cdcvuoio.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2umhbcipn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fqzgfiqh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2flmhhbzm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2plsuffny.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2uwjsvwmb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ulxkapdg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dsewcceo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2eorfjhls.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hjehcibs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2krijunll.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pyamdnnf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pxnuvlbp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mqccqrqp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2btedjykl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nfgbxnnt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2czovrhlt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fateyrfi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2uevdsmrj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zueixnph.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2akcqewrg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2uekxtwdq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2nohpaejl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bpjqvabu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dnfbvrel.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2biopzsme.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tipqjhcz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bhestfzq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wbrqoytf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2awubrlpu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ndexmpla.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yemqxrpx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hmxtwnas.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rkiksyuw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qzzozqxv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oxrdsexe.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fqovmbbp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bmjookiv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2akjwsxdi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbqfzvdf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2txqbtygr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oupyfaqt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xlfbcwhd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2viaamccm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ptjrwwso.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jayjafrd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kllwegxg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2amdzejdu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ymyvhxmf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wwdwmjjj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2pldrejec.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2llkrpmjy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jzehmrgo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2iyxgunvy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jrupcobp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dsabpjrz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yrxaitlm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2easfyhac.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jrlllmwo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qcliurkw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ffgvjnxl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzjvpmsa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cxetryva.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pxaqxqhz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cwtbbwjv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qwiruani.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2erbldpby.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifmijkes.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uecztari.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gcsmsrda.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2llskzxea.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2usvxobzi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dsoekbjc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ynsfxdcg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdsqaihn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ryqrphma.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tqccbjlx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ykniwxmb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ayhmagos.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fttpehll.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdtkmtlz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2opkqktwy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hsneweal.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fssqaxqz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bphmzhvq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qxstlpwe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jmeesihz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cfnopuew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dfxbnxms.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2sfvsansb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jrkcsbqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hltabaqh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yteudhyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijzullmu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rmdrjvqo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wxdsuhmu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lmeogwam.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mxxmnzdp.html


<!-- 参考信息 -->