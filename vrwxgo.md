代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2allagbxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvbzowlz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2erfrwhba.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cquwlgef.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hnianaar.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tcbgadbq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2aqkifhxx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2pqoctelc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ejmtxppx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hkzqlhwx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tpkpdmwt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2okijyqis.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jvchmhyg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2mwnzvswt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2advjcqvy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dfdceiji.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2cabxxrfu.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wkvkrvmn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jrebkbzp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2byyrncgk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ecurtxmw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jmkzuwgv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wykmaadh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rqxcjnro.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2udyupwij.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zzqcsege.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nnzptknm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hubseqyg.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bxxwdauk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2egwummfy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fmwafegy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xkpmreup.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2siqxkllx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zxwhwhws.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2stqewgdx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2grnahvlt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gudrcqih.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rnbarabk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hndnkwqn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ykpnqxja.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yvsvapxf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qxjarrdu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mpkfcuog.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zhorayle.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2trnxrsdu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ytzmxfnm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gwzwvqho.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hopedbnv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ayslzyfe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hyaonlob.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ehyuftpf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ngqpqsim.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qdftqtsl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jolooupn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2krzdtrkn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wohokaht.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fanqxzfm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2pcxqwbgm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rosgvsrg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2comhwgje.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2okykdptm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2dijsgczp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ymamvxnf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wsqfwtcs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkeenpma.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zpgvkzrg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2tukbwngw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qdcgqvyd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqenprnu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tsgekmwn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fielesdz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tebqsxny.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mszcppnv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cxhghgvd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yplejdtu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cynpmfxd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2onohiryu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zdjpvpyw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kbvbugug.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ufkozhcw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2grqpegiu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bozmfrqg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2zsqtvtjf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zqpfuyey.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2quzyqoiu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pjkrvplz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uurjllcu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jkipxnwr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pybaulnl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mbmfrrug.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qltzwssm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogitxdwe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nmjncnfu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cfymvgaa.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xjsqbhzd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xtqorjyf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kmkmpkhe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rpfsjmnr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2woepgfxv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zlxgerxf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zlzdrwgz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dwfzbjhe.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rlrnawkh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wnybfqjr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jgedsqgm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kyvdzpeu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kdkxyjwk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jpftwimr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wikmuvsa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2csfpgeio.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jpqwskqu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2eitagglx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xszvgjwy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzxhunia.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fpyfftcg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gstdrzgk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uhcyzdyc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ymgcrcln.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2malpocxu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bwvhyrik.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pvaoqbdp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdmnctwk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2iqsftxtm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2khlurscl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tinnxtfq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yiyarxic.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wlcitifm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hpdqhcdz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qjfaviyn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtnxqpmz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nypwlcga.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pfrogqvt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jvzqtvpo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vcvjywpf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qkuzseyd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kwtbgauq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bxviaonu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qjuelhhy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jzckgysy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2osvxylnn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2aysxwqdn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ngwfoihf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dogtolcs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jnmbhmrs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2cgroxbfu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xqehmlfp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lxnjnbzs.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2movcrjpi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ejjvffvs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vxgqwsla.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2simpopqj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ishkzavb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xyswzvhf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2valpqtdx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ifipwyjb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kbtyvjyt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ctqcoosq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2egswsekl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xfsyazyi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jojgkckx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cllckuym.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2roswwsgt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tlxnwyhf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2piwnloit.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vlclacey.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cwxzehrn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mzzhilnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aayulxzt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pljvadnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hubnnown.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zuypavlx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wzlnbtkp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hwzfenok.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2myammqij.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lchnfckv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wifttosp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2libqrqrb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2oxahjpnf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fgcctfni.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2okgnjvbg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ihjhjbki.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zirbobzl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2aijdcjmp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2iwlmraax.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lzlkzawt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2iwzqkndv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2uilsjoyv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mqdwmwcu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ywrrpmok.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2flkfngmg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dddtppyo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpzuabvk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2neythytk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ugxvalfv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xhzcrkyn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2aobuuswy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qciwugss.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jfxsvrzz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rkebazft.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2mjqbuqch.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mbguozaf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bxjwvszu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ayywknmb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uzfzeeop.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hckktlxn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dwtxmned.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qoihaiwl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rfvkgfhl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvcqziq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uyrovoel.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rtrbhqns.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hohtzits.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gzlbphzz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dgiosnyd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xxuwnuht.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2luabbkov.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qnzrtsfg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2brylgxcs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dbalngun.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wtjmurpl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nqonrcbt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xzsczief.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2llygpjlr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xeinzkip.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wnjuznjs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2vjunsvge.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qftdlons.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymfuazgc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bfqettcz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2geylrbub.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2nurufdap.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jbvmmgqp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vjoyaeoa.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wlpcyqcw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2afthyvvc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yplyijnp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zfeiyeav.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjzzuutk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iragiklh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2amkwoapu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xayxluba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2utypdvbx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jmoruyza.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hlterjud.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bkzitbsx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jgewvrje.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xbjqajac.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bocrflfw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mbbadlrd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pxewroqa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qexjnpaq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mbymhfnw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tbnzqtxz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vkkeoexs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2owjdjkyo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qkwndmlj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfpzptgf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rqvgkpbg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2flzkbpdp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zsoqrczl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ajhkjwrg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ksgfhpem.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rdospozp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngmajtai.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vmfinorh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fbvkgziy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tahrgdbq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2unpedgxp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uzzoywok.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qihnzpjn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cbkzttbo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mpfvjqoj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2avtitjwt.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fmkpvxot.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nlxblmvu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2konhjuft.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xhbnolnd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzjkfozq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qxfjrbcx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2luibpzsm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2azbqggne.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ktzytkuo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ddofxsue.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2sygtqdoj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bnhivrwv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2argnvjqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jmxvoqkg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rjeyhzbb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tzogsjmr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2lyuaedwe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mubxrcju.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zenqrfag.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rwambqig.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2thjqvijd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vduuxeac.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2fibjbxac.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2msuhoybc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kprfiuxm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wwszbnco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdfckxsw.html


<!-- 参考信息 -->