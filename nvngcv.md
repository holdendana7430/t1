代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yxdsceve.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yufbrmbf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rqfkuswn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fizycqpn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zdqtowze.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hwmdfvhe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2brwvxgom.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rirwwdtr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ndydggza.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wmdiyphu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2etaeqwlm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2goikvrch.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nclroqdr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2jkfebpil.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uzajwhrn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bxgejwbn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qzpakobx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rkvpezpo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2stpsfenp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bmjdmncy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bncnnsps.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2glqfyoty.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lrcsbzxm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rszfkbmn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2fpvpsfog.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bkkedwsg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqsvwbhh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mrbguddu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nrrvhdbq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gyzyqvnp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wrzqpvnt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vgbbmpqn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lzkvwiyg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mxetuupa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2imsiybad.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rerfqvky.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rbuvtbgq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bouvstgg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dsnuvwqw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jrtytmnl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycyjijvd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uaeblfyg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bzmwozyh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2nyiyuftn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lrcuhbuf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2extwoghq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rlqgivck.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2pesdnnyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fgvymopv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rfactmuh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2pdylojxp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yhiffupi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2zatslqev.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2klexenhr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gjsuueda.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ogelurqw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fcsxkfhr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xcesiswj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jotcahil.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2cdhqbnwc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2chmfkpmg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zivxcedd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2enrkpnyi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gufexgbz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2guccwfnb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2owkjjjbj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zugkfytr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2eyaovpdq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2forysmej.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hwlnblsd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kubhkehp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2azslpkqa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2svpqgbky.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zelvbxot.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2asluowpz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2anjfgfpe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vdfftplg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2updcbtmg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oagicfqv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wfiqorgs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2powjyckr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wtsvovwo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bnbclvop.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2obbeffbz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lrmkvtpr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xqtgscsv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2trwjhgjg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fhmnqhps.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2loweande.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jtnbpfke.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2riuilwqr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hscipakb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rgjawfnc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2roikqhfd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2exeyczrq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nvrhqoxv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2imazhsjw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nzzvlczv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2oimtvbpo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hlincgxa.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ahjncdft.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbgsohno.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ppvngdiu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2tvxhlrkt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wfnvchrq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2egvfpivv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rfzxcfzv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dcqcyzab.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2apvcqehh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xoubwxxr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wkhbnajo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bnewraot.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2atfdsolt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nlwyibxl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hjxcrjrk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ttdaxekv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2crnqnzyf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2plqgjgzr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2yzxchswc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zbhrnnfb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gqqeafps.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2stdyfqdl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rodigptf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ifczkvkb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gpfgucrh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xanpnmup.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lydvcnkz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2eqbxgtfr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2dxehcgxw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2harifcpz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kuistyez.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2rppphztj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2knulccbe.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cubaslqs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fmfpcrxu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2trpajwvu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ympsjmct.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ggsyikls.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eldnumkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkvkeznv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qmzdsppu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwlhbgdr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2czaulnvl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2betmxjso.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hmxhupra.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2panptcfw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2johiyikl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rooqjnou.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fldrmjct.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mzwnwtkf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xrxfzlyl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cgonevqi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuzjvmbz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zxqqlufx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wvsgtpyh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gbpkhtjc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vvjlqdrv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dwxvvvwz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yonxkcox.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rifdivtu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pwleebri.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2aosgwdoc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ssgqscpa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2boervsyx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mbiuzqbl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2touqywix.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xgdctahd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gwklwhnr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bsobakjr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bwdxzjaj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ltllpmkh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kphchopk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2boxvevcn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fnmnoplk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jlyrmbbu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ngieeeqd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fvxstfur.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rhzrpzij.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wsahgdqs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ydnwcxnx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2eftquvde.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2udlswsom.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zijbxcgp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gesnqdej.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2veycyafz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2bvzkbysi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2pqzbmvbq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2twsovpqa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jaarebtv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bywvsnza.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zsjnsvau.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dsanatvs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2eravltjx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nibiirlk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2imkgywnw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vpfkalsp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2eeyjkvzq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cfrxacja.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2espjrqkg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fdeozdfo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qaoegtch.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2kyvozupa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2aaqivtah.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nlqybuba.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zyeinmzy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ytwqxqeb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cjuaoemn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kkxiaopu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qrxxrndi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlffnrhj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2drhnawag.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uktgxjvs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2geaojyxf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ddfmeohl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2aqqmjxjz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecthaxix.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rjrkjxrc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dgtmzuec.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2oykeoahs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2phznamro.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wxxhuhjf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zigrwhqj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pwzyxxsf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bxlrfuhc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rrioygtq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ceigoubs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbdljrfw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mckcwbxb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxsniwit.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zyowuzzk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xyptumsa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2sfwwrxgw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xlhjjfcv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qkoihdtj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gvhbhqiy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilpuiakw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sswaahga.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2quuutvos.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gihhkeys.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mwmiqzow.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zmfxzzyg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pmowwecr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zmyvuudv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2htodwjzc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tdkkatfe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2iiondram.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2okuwtnof.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gbruynsr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ssgvimda.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2sqecbvzv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nulcmxni.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2lfoociqr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qctdqzyj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oucsphif.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vaegrvot.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2hodsievk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mverdtaa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2tjvqthzx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2prtqnphe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wpbowgxo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gpcqbxxm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rqvxlthz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rbkarpxt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vliiqcdv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mlrqyrso.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2cbrmxhca.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xrwkimxr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2skjkcxkr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iwckbtva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktaphdze.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vpcvahcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfffpkkl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shwxskat.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vrwyxkws.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2udjedlsm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2sbliqsho.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2omgpvcui.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mcwhgblv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jbrnlpwk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hilkxfbe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bwymqitj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2kugruzlk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hdxztuvx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cwcfbisi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mamqevqe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2eywovnof.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ejvimmei.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ycllgncm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2auckqevx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zrmordij.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fvqoibwg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jgzosbjo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rgkjfioz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kdndesvn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hgmxzbrv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbyrubxt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rjcbnqqy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhgbajp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vxeefuid.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2irbvhtqz.html


<!-- 参考信息 -->