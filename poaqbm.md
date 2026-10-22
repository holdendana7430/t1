代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fgdfirit.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2imrxikqq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2erwhgoeh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rpjmjsle.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2bmprmuea.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2djlxhiqe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mfewvvpz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rpdbwbfn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2nezdipcx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2hwwghrcy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rihxewwj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2psnqxbhp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ljubtrtv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bukaznsk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2acsqhyyu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2spkkixqi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mfcdiwpy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2anttrwog.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ylozitdo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wnjyzswh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ktisceie.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bwnztvsl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2udfdjwjf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ydjnmech.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bvvzojpb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ueyhjcof.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fgvdswtv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2scrvekyq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eeuygtte.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2isnjhfmp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ezmmfyll.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wpadlnje.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eveuqrna.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2onehoktw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2scdzyuor.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2aesoxwnd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2txwdpkqj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vgmctzin.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2woqgnbnr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qsqikgnl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljctcbgu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jtegrrny.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sgetgtif.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vnnrjclm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2yzlhdufm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ziozjgms.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2glfpndeo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uaulkval.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2volwggbf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yygsojyq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zgcdklga.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xchocoqn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2riqezelz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dsjqhywr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ntxprfoc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yjbndkow.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lpqjxdjg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dtdigviq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pvdejnug.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gxfoeuxc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dnyezfkw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wrxirzer.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ogbqcgja.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uqtqcoem.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtvksckn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tftlrube.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmqjglhf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ylsolcdl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wilpksrs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cliohavg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2segybsnl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gevivrlu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zthrywfb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gttmdtgd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2pzdknpsr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sbtdsrky.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2eperswez.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dezveqaj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ekoqgqoy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fqjbuolm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ucayhpwg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nephdnrw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2krtlxtxn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ernmibhq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lapfdhes.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rzwwpxbh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2onfhnzjz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hckuwgda.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2cydpcjhv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nnrbnhaw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yxwaphaa.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mmdyozkv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hbikvwuv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hsidrpzv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2flqdjagn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xvettond.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sgljgmrq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mvsbnhad.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hlfovahp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2yebmzimp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yncieygy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2iitrbbki.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2trzzqmxu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lcfhvxaj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lecmmwix.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2iiznbvqw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mwqobktf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2lertadzd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vroxtuln.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kllbbgkh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kmhpuiim.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2iuxppqbh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jfngzdwh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2molwjzqq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gvtppzhe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hsmmaxvy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dqyncvds.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2joxygyfh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vnbthbgi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pltdlhva.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lhthdihk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2swuvefig.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2werlhzjw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uwdezxzu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2debfoexe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxcobxyy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dzzpyuey.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cvidbtbi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2evzkdbqk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ebscufqb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lgtcboaj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zgvcdvga.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xkmlroau.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2utakzppg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kigfmtuz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bjkdnzyn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gbtopvze.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ljvappit.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vpjqkszb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ibkbvrml.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wzaixcqh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2byckcahl.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2spwajyhx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ahsxtngn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2moppjvyr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ocqdmywd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ipaeyrpv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2pvuzufep.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2axcaifir.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2apmrrtvl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hysnfumb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ditbpcnf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2dgfmqtsv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ulcyydxo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dvldnqhw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hacnusqx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wdyuvrld.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jlgabxyx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xwipjdox.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hxkbbeyb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2oobaftpj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pvbltags.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2uqqdlwib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rprvmdow.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2sejxmonr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckqewtix.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zgsoally.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jqbidzmt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2oghqdkxx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nzlncgnt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2oelnnlmu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2snzarnvy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bbaktpxp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vbvxzafl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gxwbwvtn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzhojfpo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvitlfw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tekpdkuu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mnwrvzjj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lpmmavwe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bezvwbsb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kntdflih.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ljinzhlg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2snkqurqm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hzzzlgap.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qxvovfyp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ghlhipyq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2arrfttui.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2uokcorld.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2egpoygkx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2scahylev.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpqbtnbt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zdizhmzq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tbtsmimp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zrqkqccn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pzozfpzg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gndzmzwr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vrranflc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2gccqzmys.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ikqqpdxx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lfsdihdj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nrkkhuly.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tkxadvno.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ukllvkhk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2mbessrxu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2htnyragj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gziioggg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2slmnrobc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zkmicfnu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cgmqjxug.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rcauzbdy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hrayohep.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tpxvtvsb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pgyrjexj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rscqffic.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hnpmcuye.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jiklusie.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xlgorumo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xubmkxcy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mzkdkede.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cammogfa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xzllbijh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkmrycew.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdbblkks.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2lzqwirqu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2snrgocjz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vhoaogka.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2lgfreiaq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kvcidfeb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2aeexxxhu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ajpzjpvf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lslhepve.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xxzidzta.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smjibnqk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bhghhpnn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ahdwgecl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2juwzscix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rvgcytpr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zyhbpsso.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzquvjte.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vcgraxcj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kxmouylg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gpoxvuvn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xubqcckn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gugrdscw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2junvhulr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mwtipsea.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ydgqebyr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tdbasbla.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nkyqwble.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ieeevnmq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qlorjhdq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2sslqfclk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2grchausw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2efufvhqo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hkifnyar.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wilsecbp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vqrssisb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ganqyssu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcdbxvvs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2psxkgcez.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yssqwmun.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gvaqbwcz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wacodesp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2llqsdyvt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubthhhcv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrukthez.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zlvfyghh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zboccfmc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hmhrdnbw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ufbabrgh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2iwozhoei.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kmimbkxr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ymdozuzd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gyuzzqrg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2utkqsboo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rhwlcaix.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eyibpraq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wqldjtsl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2soxjcfar.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vitrnsaa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jqxdtknd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zfrqywav.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2angbxhze.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktjsphih.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dxndiiqq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2gzmisnbb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tntbavvm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fqagqmbh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zengsycc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fggwwxgx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2evfzbjlz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mbeylbnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntjzwzff.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2maojkgpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdpvruqx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xbtaujme.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rveawvrr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wlkdjmnb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uwldikpq.html


<!-- 参考信息 -->