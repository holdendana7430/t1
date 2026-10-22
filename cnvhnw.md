代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2svyhjfav.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ztihwcvv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nhpinuen.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wtyavanq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ljoshgxe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pzicjoxf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhgpderh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ygkvrpcs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kslrmiag.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2oqyfonbu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2btakrdzz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lbvmpprg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwmqtkkm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2kgkfgrph.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sqblgfgl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vnrdezvm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rskvqfua.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zfcblqba.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2guuhcrwh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qbnqfenx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2adkeeqgl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hdjmeivt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wdkosfaw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jocgwvkf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2eybftvbu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fnxdmxoi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kurhmejz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2smwvgtql.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tgymlddl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mdmnjamu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2obtqifve.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rklmcehs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2osegpvvf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2csuczkuk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xiovlcuz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jeiuxcgi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ckeldgjo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gnugutkh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jajlrpko.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rqgoceex.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jlcneytl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2adwqcnga.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2miwkgfwp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lyyeiimx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2utfmaiuh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mgvzepfa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xeomilyg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hehxxbvu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bfxxdepy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yuczierx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vaasdrbv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2bfomtyth.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kucoepvf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zovflcby.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uziarobs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jszocqhp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jhlkpuzc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qjzclubm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wflqfqgl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bzqeejah.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ugfxabuw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2eysufmys.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ijnnrrqh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zehxczjy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kcepnqtf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wtruneeo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xnxliise.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2uouglckx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vagqkisl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2timvscwh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yatbatvc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2bgdxlift.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hbpcjyjb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jjhhkfji.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jyaalvnf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tyzvfsjp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fcsxgjsv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2evpxhxkg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2djbzyycr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rxhugemo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nmlphjnl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jjzqudbn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ixrookvq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wmyrtimx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dlvglqjx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2aclslovq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kneipizw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xezqqhoj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2yghfueur.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fuekbzec.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2eguqqqoa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wyjfucqa.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bucvnvmj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2axhkplhe.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dhjqojuy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tnvdpcvr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2iitodnei.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wcxfjuxp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tpuwlnco.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wxfpfokw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2giujsxgy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2dshuvjjh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2cubvvkof.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2snzujinh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uuuusyzk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dovxlomq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2yvbjqtfp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2sfoannmu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oaoorhum.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wfzuidzd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hzfhndms.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xesatsex.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zmtxrzoh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ehpklxvb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xurawskg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hcxnxuyn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ryeykdjw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2aauvjpbk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gvqzkzig.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2csajqvye.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2gnkjwnad.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tghakgve.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2txwxjznv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lrinvvbg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2llxwxtam.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ajutekbz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2aseppydg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xamkuidf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ochvnoyl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lqjdsfhf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ypdunafi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skdbltci.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2luunvkxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agsujfnb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qlkijjxr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2spgimlor.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2unqfszfb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qfisivao.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2svdaebmu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2kqwfxjgb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yefjhltx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lxittplc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bmmvznej.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gjidtzys.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjkrtlhu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2srneueef.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wxryqpca.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2emsodfug.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2uwiqtvow.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qpkkujom.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nocjhpqr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ykmfmkmt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jtknpynz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hzphkjrt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bjqegzwl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jowuhzpv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zndzkpvn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eepevywa.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2apcafifh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zalfwrcc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sujnxrbh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nlzhzzgx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2szgvburg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rvyositr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eqwsdczv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ajhtvhxx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jasptozq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dauedbxg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ejdzlndq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jizsmpmt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2urmyjdms.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gmhzcyyl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2prhzrjww.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2hjrdrokr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ewxnhapk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kpztezqc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qvdvzfvr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nxhtnbtb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2xmndzovq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zpibspte.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2skctwjgy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gdiryrvl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2reilmzsi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bwggkkzi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bnhmriah.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jncvtddk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2klbmoupy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2iposoxor.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qjvdnisp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ydoqcncp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2atrzzhbb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wltpshdx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2siyocjpc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hocuqwob.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ufwaemwn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dwqnoixv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vapdxmzb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zvtdcgup.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2odslxqva.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pphcdlhd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gsejotjw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ilqhobry.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zablcxtr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fpcupriu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hbbfawbm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2thxidzml.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rtlcuzou.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxilladf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fobwuvma.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zztgtbjt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ftffvjtz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hxffmfoe.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dmldvjxl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2bjevbcqb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2uzjyuewn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qjsnhvmu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jhjnhaip.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bxrtqtno.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywplowph.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2blmwvkva.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qnjwzvcd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zcymrowc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2fmxcslhy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wvwjybzc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rknyfswp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vbtvebyu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gefpamwm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvbrmhgb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2oxbtkqnw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2axkzertx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yuovpbva.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2lnzgddna.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2srhdwvlp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnwzsrtf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2romttlrp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2puhrbqaq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mkpmuzbm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ahlnjgyp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wkksgenj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qargvjup.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2irpboeid.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pmgcihlz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gswhqnec.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gkrppqrf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnfyhmm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tknkoyft.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2dxtixvhy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gidqdcpt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2naudpkuz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2iguimciw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nfqqxbyp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lkpotsly.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yfedzpih.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zyxfmzjm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vrtytmti.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jciabltg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2beqckryo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hrbggbky.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2anmfqtyo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vnukygco.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dyxgggpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjxvkmvp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jshgvvfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vspojhpg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2apspupru.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yizrtsna.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hdxlefgc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2dedbzzsz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2yzyjwuqd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2twhoyrrd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zsjutulw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xalvcifz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eiyrdafh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jixibzij.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ondblbdc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ugwehvya.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tmkqpgae.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tgdhygit.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qzufqkni.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dmdykreg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jzlrbudx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pecuymnk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gaqmhefn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pbgxjbxj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lecorbxo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fztirtwo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mbcyptrw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehnfzwlo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2glfgxjgf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2nptejrsi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iktsorhl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jauailui.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zgqvehwj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wtcpspfl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xtvddvam.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kifskixz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2miavdwmb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vqcplung.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2queyttoi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ivwaqvzn.html


<!-- 参考信息 -->