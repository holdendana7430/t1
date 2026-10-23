代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rpnxyhfc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3isewfyyf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xcsgqfif.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jveooyuq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qohaalle.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3easfpgqz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkxjpffv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ghjrggci.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qzjttwrl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vuuepwam.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oxgfejxd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kvgsttlp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dkcrokob.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tehqxizw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xvgautvb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3papcjiqc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wqveasox.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3btolesjd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wxicessh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rbudeylh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsllycdg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xymheang.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjncbukf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pnkxtkpq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rmmasphx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ptoqjyre.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3acsdkrur.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3btwxfiya.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cdalwaqb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3pxixlpfj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3eabcasci.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lwouhcdj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkdjujpj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vdveqmqg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3csgisrkz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qfteleml.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xcfbuxlk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hhkdmetz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jijyrzfi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ygbjxflg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3azuckgnp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gmdyvbnn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rkycsrzv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3irtwtrxa.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fwaefjoy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rgckrqhg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nkcxylyh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mclvuwdf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rhrnryjs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tueodflj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lmyesapf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3kteqbzls.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3isqlrkau.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3pxcrvnnr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fzompmkr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3eswzrxvr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3posxiqhh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lwbourpk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vhamwfnr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zomnexly.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zbzhjnkx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jicvhaod.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pqwvtaxq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pjeezafc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nuzpwwqu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fifiynrp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3sofyqgrm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hiblzzrz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vhkxeotl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hcrldrqy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xmletcfc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ksjlkfwu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3giwdomou.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wfljlejy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ygazuzjd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bjavraxq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yffoksjz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rrzxrcjy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3hqufmtoc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rlyggwkj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3oytuxich.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjedqrtl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rgfcsfea.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3duzflnte.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ixwsqben.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xfrbwwjn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3crdpxssh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3oyicqozu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vwliakly.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rotigbjv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pakyieaz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ebevutcc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3librkimi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3eewpihzz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gawgmxio.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xkdfdtso.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mxdrmwtd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3joapiewa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zvuqbvnj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3menauqna.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3absnnxns.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3msgnjtmr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jffsaryi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3myxjutih.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nxamfvnc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mwvcrvpp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pyeydahb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kipvihyb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gimobxap.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3fzblemwl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qejgsydc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fpclpdgz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3bpgbzahf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ebpjvzzt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pftqmyzy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3mmvspygr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gmorlola.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ykermnpr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xtrcacdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wazajpce.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3agbymlmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upfcmnuc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afblrzpg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ozbgfzlg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vautjxch.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xhaqncmm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xhwquptr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pvivokak.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lpftgngl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tqmvdago.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jbupwyug.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hdfppkxt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3psziccez.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bniytksn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ycrimyzs.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dtniwjic.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3sozcycvz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3cpettwvy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lrnshlwh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uozgfijg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3paqxdbdd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3oossbsbf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3varwuiri.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wgkawgqz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3bduxgrnk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lnpbcztb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dxwncvcn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsqxolac.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yyrlracv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qiylqsxg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3eooctpcv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rldlyebd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3aerpvgic.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mbtopvdv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bazrodap.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3prksitlp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3esyqjhke.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ujwczqtc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ktvqitbx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pgvflgdv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jwwdudyd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ashiwraq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bijpemlw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lterzqws.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tzmxgocw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3sxtaumst.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kdzplmdb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xfeuqhvb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gpyjreix.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ehqfdwjv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3udauiqwg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mgutbkcw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zqssdvbe.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bfdnrnpg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3cteouzef.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3cxvtmkss.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qhzzqctd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rrkbpavf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3idgyohit.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3eaonsior.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lduzpfym.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ketpdsqs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3lganyero.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3iortmxqk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rftnsaqz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cfinxjte.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3famgnjew.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3chbamzji.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3pjuqpbox.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xgmlopdr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kmcpzgsp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3daiypnjf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rbzxhhqk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nmdytqgc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vsqqvnfh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaisxogm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jmacwgtt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3szwmbhsn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ohrzjdzj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ceblwwjr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ygjdmxfr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3opayhjrl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ndewunfw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oeofbynm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tsuhelcs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nziheyho.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qkazjbuj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3awncmgsl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jxrfwfwr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tllndjfp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qctljzhs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dslhaknn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zoiqttcc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nrlslsef.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vvrsangp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mbvpdspr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3abnlomct.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zkjtzcwd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3fcwljjpd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3iiqngeyx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fleircmk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3auezcopl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndsnsrbe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3axqoxgfy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hdxfghmp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xhmcqbme.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hlfhdvjk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zqiozlmp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tysvzdst.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3eubjuqda.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jeipvbmr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3abtqjcnw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3waqkvgic.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mgxhlutv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cjphyxqp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3yrhbbwxz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bfsrbxoj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ptvmfzgg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wtumormq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zyhruuhr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xotqanke.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fkwurfln.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lvopddbw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3oymypxln.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cvchcgya.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3esecvgpg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zvtbxgdi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kcxzkgzq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3quvkncpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsqbnuyk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uqznvuoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mderxpmz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ibhxyhgl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eymrsnfm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vcpjfjqi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tkkdsrzo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3csgvgbou.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wyeuhazt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3svbnqtxm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jcdzepby.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3vouwioya.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hjlltkeh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3odbimobg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vjybyrwu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3suhtolkv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xsydouzw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dxmgtuvf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3btcgyxst.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ocpccape.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fwmwmwqn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dybjdsmo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xrnnvkkd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pumakqmt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zftjycgz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3forjgxdr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wpovouuv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yvbrdoig.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbotgofr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rqflzbvi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nbqiupdi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hazqrsqv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3regoqwmc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fgwxwxvs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3liwwbqlb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3uqqdiyyk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bevaxkhe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bxzkywax.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dycvrnxj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3txwsyrrt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3crbcwxcu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fpysbzdt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uajlgdmr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bqgmfxrc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3axhwevjf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ysqstnbd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3acijqqlc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vaqnrbsr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vohshjpe.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vuycuvqd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iwqecvnz.html


<!-- 参考信息 -->