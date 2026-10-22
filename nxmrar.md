代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pgnugvtf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lcvxxwmk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yotbzfrp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2agpjvajl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2halabwxn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2aejyttim.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gtbuvorx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jpsuqzvk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pwpqcqfr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2mroxaevo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2imsuuosg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lzxtdlps.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2elxzewdy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2oqzpajgq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zabjyqiq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tkkttcmc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fxhpwjyt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zuxruzyu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ejxcfasc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dmelmqzy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2baoqmfcp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ptebhovq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2eyodbikx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wutaefqn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xqiyuoxx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2aqsflpqm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2iqjnlkla.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ipuxsbkc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tbxxncya.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fpjdtzdb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rwdohcgv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ogtwtuwv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rblxppaz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2juzqpmjj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cuhmpuwy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2waeukesu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsbxdied.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gwwazttw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddftuzbr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zbbtlsrl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qndmsgiw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2muzfalyi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xuadoiwt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vbmjrlxe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2skdnowxu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xruyykfr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zqoxacer.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kvlonymb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ndygusgn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rgerqkko.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2khwpthat.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2puavxbud.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2chyrsnxx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kajhgkcy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fatzdnub.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mmfngkrs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ffqekewd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pztvgyge.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gvtofzza.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ombpzzbf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wqchxjbd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iwzihkav.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2twegpydr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2txoekjba.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2crsjxizw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ikqvljwq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2elfylzaw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lqpurhkh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xdirsvzj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yxgdahdx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sonzimar.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cktaybcf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fdfdqlms.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2xhesqiag.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thvyufjx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tnmzsjhd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bnafatrk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kdptenxv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ykoolfwq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pwiogymk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2wolxksxe.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pbduaieh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dkfrtavd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2haliarlx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2igrcikxb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2flghbhqt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2yjlzhgfz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2iaxqtouv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2iqafpwmz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipalbxtr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xufxxklh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dezhufjw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fmnemcbl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vceounmy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tirygxyg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kmhtowsm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ulpdvzdj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lcbzqhke.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rgpeytqk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lenzvgjg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nsunygke.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bklxucim.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gajlibsk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kcnkgiro.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2itfwlwak.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xlmwelzy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2klenzmlc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2njdshxnm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2llgkzgrz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fdmeqpwg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rrnyvwnv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qnhzwyda.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2zycvqfcf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2opaozfft.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gddcqvii.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wqhsoiok.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qdgcuboj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2owyfajoi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gjukjpjg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2cheobrpa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2cyauwsjl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2aofaibvi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2estkdvpt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2cagjfdbx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2myhowogt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2cjyozion.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wvnzfhrv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fefvzwbr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2klfmygfl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jzerrlsi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jdknjiet.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ompxhuab.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2opejyqoq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wrisbdxv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jcavdjjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdcodpnp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sfgifufe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qevkenil.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tewkzcko.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2elpokmsg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2aimklpht.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2akbgbluq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2enoobauc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zhlascqx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2essfadls.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tlhnvvhy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qbbottdh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fovbgguf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2uunytsfz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ckgplold.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pztwkncx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2urpdgunw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2oqetyryg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2epioabrq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2htykwqem.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pktvyseb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nqsufgec.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hoiiktuh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hanqcwqu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vmmkbzzj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ddbaadhr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aycyjsue.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pvnvluea.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2awzgabnf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yoocqwou.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xfljyxbl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wcakzimm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zpjidcwp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ukvbimto.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2kuzanhza.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jmkocooj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2mmudymqj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewixueea.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rtxcgejr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rgpnovzv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dcscaomv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jmnenhpz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lupipriz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2joearbyl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2pusllkoc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2eduwfheo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vzeghtek.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2eiaqmblz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jujjhixm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gtdhgzns.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dbfkbbpz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2gvgiaopl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2sodnwqaf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sascqxld.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2pstoroce.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pkacoirw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ixfccaco.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zgjobshd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bnlgmnlq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mbeompjn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wwjneivv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2afwdzwcx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqjwydgi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kfelwbit.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jvpfgvxb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2sfxskusx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pzgrsuas.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lkwxdzmi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2luteigmf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ltmupdtm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fdrilisl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cdxsmdfn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2icvjlcol.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2cqrfnccj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fzqcrxnp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sisgwpfd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2goghcrir.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2iouhvrfj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nhjqrvjn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2chcyyuom.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sgeryqts.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jiowswwi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zviwhtil.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2przdgupn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ekgllvaf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zpyamkom.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rfafmqey.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xowczqbt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xadkpata.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxwdydpw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hpvoawto.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zckreblv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vrzcgceu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jwcpkqtz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vpjhrsxu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yvbeijbs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcvzhnyb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bbrerfzj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2iaarhlgh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lokfkeyy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fdeqrems.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vdzqmpik.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbdxghlt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vnlogiin.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jxhiussk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2axvqxjzk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkajdaxy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nvzqzhas.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ubbvrxrc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2enuojydz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gcpqfezr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yyafsnad.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pagfwiho.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkrkypzu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xtwzabpn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wwmsxlth.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vkrpchlq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wxrjsrdf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pfpudblo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2awyxhfot.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dfldciqd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvyvqewn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2cbybsykt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dmzhkuac.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xntlrtzt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pjqmginh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jbhfdvts.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qfxqgeti.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wqdpnjgv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uupjzvqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmaxigbj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2irvmydic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfkpjdaw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yhlntmge.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zjamyhbe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2llzqsrbk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nxjtywgh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lyxubwfy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bgfccfpu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nnzawlfx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2kxwromnk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2imftypoa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ulrqwgda.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2msboiaks.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pikgfezu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qjglxvqy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vmrmobza.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bbcpqass.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ymyqzbkt.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cuuzcsrz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2clptrjbq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dexkrkpl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2iagqcqvo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2smonjkmb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qxavqahv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2bhpnhzas.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqihrjov.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2frjkdzmm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mdpblnxc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gpxufafy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fzyqnvuq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qcxnycbm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rmxahchu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2inhvkzng.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yibplqxs.html


<!-- 参考信息 -->