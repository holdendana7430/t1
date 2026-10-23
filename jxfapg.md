代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bcdmpoee.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yfvdajbe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kmxitzmr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ephqbjwb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3giytzlgn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rlacvuyz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jsxpyycc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nacaspqm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3himixvvl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tqigxiij.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dfjgrvax.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qluhuqla.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dfibzbah.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3krdhgyrq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bqlqeehf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dlqodqub.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ntwzyqdf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ybevzlgk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3zmzpkvor.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zouqpbud.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fouyprhd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mwfatoek.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jttxqrqg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3apppttvz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3yqbafnvp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fzmuztmd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sjfjsyle.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3omonrqlz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3grdpbfum.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cmogkvuy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ehvvrobv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gdnjaubf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tpbzoypg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3yhyfcryu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tqtyxpfb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qwatyvhu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mxcfwuhc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gesrqgsh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3lpjzculr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3guoujkby.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fcindovw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3otyijvcz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3eyhqwjtt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pwxjgghy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pgouuedw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lwomfdfn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kodbjorj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jgfsexjh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3liupadvo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ohzxueft.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ahdteear.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ndtuhzyf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lwmwnfan.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tmthredf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3epfdhllr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3emnrabld.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3luhdjnrk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ojrdjfht.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ilkcdhqa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3hkycqrmt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zkytpixt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3giboudpf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ntstgnqc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fhnitvvj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tygqnejq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yzndsfjg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3emibiilm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ovhzrbws.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ijfjrygg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3juedfhst.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vllgltlu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ocsyqiko.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3irmmnkvh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3frhigbrx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cycirrmc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3iqdtoutu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nliykdlz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nxxkbzum.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ilxgwhen.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lhghqkhk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wfuxpzyj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tuivvpcd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dwnawshq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3yvbyghgt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jzeuganj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hxrotduw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dwjyaiab.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3oismillr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ldjmzxhp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oxhfgsay.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pvyfnqte.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rwjbyxwn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vpphmgpf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3anhuamdi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vsgmbxtw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dktpmavp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ucntoanz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3pfhowtly.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3coajhljp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lcaccfad.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xkapxbpo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vbabkwhs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ddmpdszm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3spmqzllv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3yacbakig.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pldwrkoq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vswiwvhk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3bwkuijbj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dhhwbbbt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pghvndbh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mgbnrqrz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ftbssbay.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3olodnrnn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tecptujn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3sgufszgg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gldsaifm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tczdyvxw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3lyfbzlsm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rylpoypj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tetcthei.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hlaaaqdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gajfxeld.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pbfssjkt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nhkycpod.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zvsacddo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hcmubwyl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kphtaaiy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dleuzkah.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fstioqlq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vvqlarvt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ivabnezb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yengfkwf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsbzlra.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dpccizwv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3navsjeau.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xfgvnzle.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fslulour.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pgjlsobq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fzmbxppn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3sybcbgma.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gnbkmbag.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qcyphvou.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jzmrvgmb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qeqljjjf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3njvxrqhx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gcnbdquf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fwprumal.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3evyegzdk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zafbawko.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wbyzkbmc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bdtpinke.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nsarkovk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ssleqofv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sgktqodv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3krpxrfwm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3oxamevji.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ncjhfhsy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emnbnupz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3anjcqhso.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ppfwotku.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ftoyzhuy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3rvuaiurk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aqqewinn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3rnqtylaq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ucrdtxsq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3atpchjvy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yqqidvuh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3alrcjvnl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fuhoigdq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ioocnucl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ibeipnjp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rduqxhpo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vlguzrfr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uxaxnaps.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zsrlvcfo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lfulrzkp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hvouzigb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3stgpwhnx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dvgpuhzl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pmqgkvfe.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xustxygi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3htzrxfmw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qbcjqxpg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zjcisyen.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kcccbupe.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hmwerpte.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3iyhsrmeu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nlbqstzy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ctohutob.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qlwhbncl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhugqtrx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tknlixnu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jfgrlmng.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3utiwryhn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3emkhtsim.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bxhvtuze.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hajnkiaq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qavapojo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rixwzylr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zbywqsnu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nndowayl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rkneymhe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3elonzwum.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3imljrxuv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3afczayup.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3njaubqee.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tzzpqlcx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hwdoscbi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hrqhsefn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lsgxxtfw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxhsioux.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gcumxuoa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lqnkibcq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3aoizersz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3onusapjs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3oirzftrq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fmeiqeon.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nequihsr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rbznuypt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hexlpksl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xtcsidfe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vyuvzgdo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsskqgbw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nfrybnmt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mrcjqnqv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wucmywkh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xijhdfza.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3trtxyjob.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kbkcxjyw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3dxutlztl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pojpwuuq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nwguanok.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3teiujmat.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vheamfeh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mrixdrvz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vowcnomy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ftmmollt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wpqvtaqa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zbffshnm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ntmcbbyl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hvpxixub.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3xhyflbfl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yynhwzzx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3igskozyg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vyhkvsgk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3reowrxya.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3syadkizq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xysppafu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sgtxqrob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjprfvci.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pfbmvkdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aegoxtdb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hufbkqyd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iuvnxkxd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fnsckorh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qnogcctp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3edeiiiln.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3srbhoumh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uigdlwwt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vezjuink.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3sfwdinyo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nwibkvut.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3smmzhbfk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fieqdyzg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xppckpxr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jrvimauz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3sbwdezpz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3menickjw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mnbuorgt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3untvdymz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kawgaynz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ryehglkj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3cplsptbm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ajvsmstj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3yamolejb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fcfsdppb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rnunovxp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzmomdy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fvycpoxz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jcplfmpi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jboaxxda.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nzedbqyc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3accsaskz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uxcjfiyr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3deucnhdu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cocujwtp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dhcigrca.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gbvauavq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bvapkegb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfqtiwhq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hggbstju.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vztpzrig.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hlqahile.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bnthmlew.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ladetnza.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wpsjucpj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqutopgw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ktrdvfck.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zaxkwlco.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3czfjzfkc.html


<!-- 参考信息 -->