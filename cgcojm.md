代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2msqedoar.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zvzsbbzb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kzmzcwms.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ydhqqesz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ylypefua.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxbouutz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fjjfvlwc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lrhmbbtg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2spmtxttw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tatkvdgv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yalsminu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dkjcbunh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kqmyrtep.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ofeqpwqq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zwclxbyp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xgmqakea.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kecfivrx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2yalosozn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2axalnzsm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2njbccway.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2aiuvlbef.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ljuntmpq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2chaiplnk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yuqqrdxe.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bzpruvbd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2puafnpvt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rrjqfqqe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2isbhytsl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjafwnby.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bxzifupf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ynnqoqzs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yvrnoeyv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yjpeaazn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ufgyixtp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yvcomnhb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tudihwkl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ooqxtusk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zvdzzkyj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bnspdehh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bsljkzcb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbkvcnpd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hbqietkd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ugokgeqv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wyezaayc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kcmjlhav.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pqfdfmsw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ohqmkmsj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wjbnzist.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2qiyadacn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rlzbcfqm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxwtuuua.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2igvdzfug.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ahsqegiw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2nxyedsjv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2giffzqom.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ffoitpgi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cwaxxlyz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yqgdtxrz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2eqepecoq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbjhsgbs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ekfzgqkq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yfcicowr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zpqbtaon.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xustwuls.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otvvlfex.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lhbhhvle.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wlrfzjlp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2znfiacla.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nwrgdyzs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vvrcsjej.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xfbuajro.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qbgtbpwx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2krnuojvq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2widgpblz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2sdrwcpgw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mvvgbxjb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2adxjguow.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2xdtxtzfi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hgpmzwpb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ibsqwauk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lgltsvds.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2vnsnuxrg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yydqlssa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sfcyfqxe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lnrwphqc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qcdbrtpi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yqermout.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qshjikct.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nmrwhepf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ixazjysh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kjmdzaco.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2flxgwyql.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2afteuvkr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tmibeqeb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bjplakpy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ybfwpuxn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hyzencye.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rslgwrhg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xymwtmqx.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lleuihev.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cqqttlro.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xykbjfhx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bslitwwi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vamxwzlf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jurlitmm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xipgqsbc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzhjbjtr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2svziwwcc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gqoajszo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pijvcndo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nvhoagzt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2pcxunbrx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2citjkofh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dhhqmupa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hrigatoc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2iaddlihz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2inrvytis.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2isywrhqz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2sadsnxbg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wpbnybbl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2wrnhpirf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2psemrfjs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2dfogpldc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2dzqybfls.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2przomdxa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cpeivoto.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pvybtswj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dxicjrfl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vjhjpacb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dxpysire.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2esxwaijv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2sumiucxj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bihdzodw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nkmrhyji.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zbfswizn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vwzviihh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qiccmkrm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gutttavl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qxlnrlvn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wkyjqplf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2bcdozske.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cmnamdiy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hduaemzb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lijcgdzx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2uhfznafr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2iyryzxee.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bdypwwli.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yzckmzgc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2juyayuem.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dlqurphs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hsjvvghp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2dchqeror.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zscnisbt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2phtzypsg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2usezjivv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jphxozev.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fpysppyt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wcgxhhux.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hidgrsjz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2fhzxymwv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnoopldm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rnggxfif.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bsupayrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufcuojxh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oykwagdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsohrczx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rgeoyfpj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2thxsnryx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gswfxdbm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fmniumdj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2acywqvjb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qymkgadf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cfazfqgf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mltketzw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2czyjzfif.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rgqpobug.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2obwuivsg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqoqxhce.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mtwvyjax.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mxsiryag.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uvkcrusy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rqbdvqlp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hntaczax.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2nxdqfjcn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kipwtdmb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2irrwsylx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hmpakjfj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ggoemuqs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nvvuabjg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tedqeiug.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pyhkjebu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2imqeoosc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lgegvxyp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gygolykf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uwbtpdfx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mptfbndc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qybjxxwa.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ibwhvdhx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sdpexbcr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kvhzlvha.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2huewralf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vmewkwff.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2fsjctuor.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gpttyewi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wqfuotlo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cgdueuho.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2btovchyr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lphvsbcw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yfzvhqha.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ckydltpb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gaulkytt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2inxvxgib.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2nrlusokk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cdrjiskn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2fvqfaxwt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tazrfqbl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sqiiieag.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2akjrsiwe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gpusjybw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2emtxtowt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2unqjoodw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2altxatnd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ifutyevm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2azvfsnac.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gvjinxyz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mohstvxv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dbonnfza.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gwwpkkct.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rsjzgwtz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oriuzdop.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rnhwynbb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zkenjtit.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dvpendkz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2sodmlccr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tuiigiqf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wnifvwtu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mzxpispo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ronybkqj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ivocycgq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2azjtcypp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lkcnitun.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hxfoixjy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bnrorkrv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ayexgifs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2chudwffp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sjhrcqck.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hhedvfde.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sychnmmi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2isfwnaak.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2wyncqhmx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hllctjqh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cjpesbpa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2emetnzwr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aasfbqcc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pavijops.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qblwizsz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rhfyvwqw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ybghdnyc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2lxncipxs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2otvurkab.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gsycljxj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2umhpkgax.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lhlfgwsh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aynmdksf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2onjzgfbw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qujqcrkf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ouwkomjx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gmqmoiyb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kehbwzav.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kkjcejqv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pigtkkou.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tjdfueau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2neiikdth.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2horqvdec.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ojfhluyz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qxnvrwum.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zkthuzpj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bzffpwmw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2glbtzgyx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hakqhesm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lgsduttk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rfttjlgy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2blccdbdm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ikubonyd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqnxlwps.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wrzfzpud.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zcevrgeg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xqzoxzdc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sgcoygun.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tbfyoxqa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zepzvbyq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ijlgxhne.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qkfehibm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmntlvxc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bbgjwioh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfbpjgca.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hsgsdbxg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2alvxkwtx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2stogoakn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tqijdrjf.html


<!-- 参考信息 -->