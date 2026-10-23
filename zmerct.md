代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hytmaova.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zezqxpue.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ruipivkx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rsddhrtv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xziodydp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lufaxlov.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3fjeigzhq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3nxhnlouw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tnidrwzu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ldeecqsu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3affupaza.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxyjbduh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nojtuash.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3sdgyxidn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3oxnqsorv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jmhpsyba.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gkggcasj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3sglxhbhr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gxjouarx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3czdpsxxw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qokaaukn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3iveyhqbt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xlohzzzg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xnnospii.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rkrpmnrt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3etqunjdc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qmftsian.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nfjxgqiz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xshaawan.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nfvnaukf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ziwncfzn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bgburtfd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3dllhyidw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3sxckrajz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ooesmfno.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nappgvym.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bvawbmla.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bcppnecq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xlsrmicj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ogcbgrmx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3roviiemo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3itfahelx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdghmgac.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uxbtwknc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ljwvklpr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pshuekmk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mmycvsnu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lbuguvjc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pvzjdxqx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yomsadvn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mracyskm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lhtcoisi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3frvmisuf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3waomnwnp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wcagtnky.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3islwktcc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qrqlsakx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vilymfbi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mqcvyymt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vqqkhlrx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ocvrdpmj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ruanmxmg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lozrnxoq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vzayihjx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikucpxxw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vqfakhmq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3npxuokiv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wzdbqrqo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ayjtpfbg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vecdztcq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cazqscfz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3okzqvdvz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3wykelday.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3eupiejeb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fpfwiryk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3hprvxziq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rtruswbd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wxwhiorm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3uelbtxxv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lgjetgfz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3foiqcrbb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wtdbkxhf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3imkuqaom.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nbbjspkm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xqrrfqum.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3skekknoc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uurzreby.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3droyrgce.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3oicqvsrh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3iccohtop.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3quwlllbq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qmvgxsgx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3guiacdrb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rxngxpcl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ehxrucht.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3stveipqb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ceztvnrl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hjpcbrft.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3orbahgdq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dkzxjdsr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vawwtzdj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eafdtqlz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wcburvru.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jltpztkk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rezavtmw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wnrpqrro.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gjovcjwi.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dofkchyb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ammmpale.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqscroaj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xiwkwrnl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3riohqvky.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3sfjsirjg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wgayyutd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lwnlzdwm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qlnccedu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jmqxlqst.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3tybkjfaf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zlmlwlzi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vkpsqvjz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mmdmxxzp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kttkdzgi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iyvgahkm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3aavuemsf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3diihvley.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugwyevxn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3etvmctlq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bchktggg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3inajprxr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3clnwonig.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjzwdqy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tvgofnmy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fpxvkxuy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fmoqldex.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3icgxzcgo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vnaxythb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wfzixmot.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3einlttdl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hpqrbyae.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tdujfrwi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3dyppufed.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nyamkwji.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3shryjlzy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lmcqpepk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3msgfrelp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tphrruig.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jzugbhec.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wpymgfft.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3roxpvylg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3iffnzyfo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uioqeucr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3utrjwptf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rgjaqduy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zsrijraj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3akucxege.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xysewchi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xxjbripj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yslxirhn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xriejmbs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bmrizvlh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xbyayrdd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hexjxqdu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gzfgjhfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxfuzmyv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dyfiljov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fixwresa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qzkqsplx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fkyfhegt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdoiijfp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3neuljtqd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hodsjggj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fkfnvdor.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tmoxolnw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hzlglgts.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3flyakycq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xhojmmpi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uoekldcj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3oaiecsed.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wsrediwn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kfjioaql.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3cuhgdbqx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gukjetaq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rdlhlxnm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dzktctqn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3sviynzuo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dtxcrjqp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3arglngne.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3elnkkove.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3makolmcb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gjnudqeu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3urecqkwm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iiossmka.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pmqcftiy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3noxzbbby.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zdgpxknl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3uurxixjx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3igtczgfu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qhcrnsma.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3kukqudan.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3tlflaqdr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jtpbondr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fitmtcat.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3iiumgwun.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nrpsxtzp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kthunaea.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3aplgxrbx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rgagjhsx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hgslfxdk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3necqxmzs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wwqqeaoa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mgmatxxr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bdnrkfqv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vzxlaaqf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ldpkukzz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sepqmpza.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rogixvxl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zpzckets.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fbwoifhy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yjvznthf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qviusabz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qptgbhcu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zlwkesdy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3htwmloco.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ecdhxdno.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3oihhkzzc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3faauqsce.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3oqfwjohk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3twdthzbr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3thfsbfwn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yvyhxlge.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3horqhiwf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gktajuyc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3uwbiiswx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3uivhxpoa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3txwnmpzc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rzbwaphd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ljnbkaxd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uqjbdzum.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bmespulf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3thpkywkx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xktkffwl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ezuvyrvg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3oyecusku.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wmidvukz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wcecizpr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3amrpjpgb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kolocgyc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wmnfgnjp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3iolvvgov.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ivdeotem.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fmsicdly.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ngmgnitc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ilahnhvt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fxxyssol.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulnzgdwi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fjwvxtow.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kahhjwjk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zrxbndzs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3eelqkdfr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmponkjq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3akhiuhbo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ifczdvcu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ffabgqbh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kxsusncc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jltqthuc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ckdmcpxm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hdtcmjah.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pwwxrrbu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hnfclbql.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iljhroan.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lssmttfm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ondieiyb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kfexgnpm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vbjxsxzp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3esjrthmf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3scxkvzzg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3buovtfzq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3uzmkrnba.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sczmiazz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hsotaujw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fqgrilis.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gqrdkcdo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3znxjbmqc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kgfhonob.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kmaifljs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lcscwvnf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mamztoxw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gujiqqpz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sftyhjtz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3quhgbnrj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zqyfvkbj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jvsnqvtm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bvvqvqxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvhwwuip.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ohzdfodn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ionzusmv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3icaizeye.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hlurixnf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3danpcmus.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3eimguuxn.html


<!-- 参考信息 -->