代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kcfrovun.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fmiupika.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rubrpunr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycybfhyb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rnjhuiyx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3iutsmfve.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vamslrsa.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ueoncddz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3munuikwf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3eksjxbfo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lvtkzobx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nlsyxflm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ssmpfgbm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3piebiepz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3vjdofslk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nrspbbkz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxlwnqx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qnbaslyv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rgodlyws.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xjkaozig.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vaheixta.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3msxbggfc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zvyncsgo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vaqhmfbz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lqqfyuen.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ngdlugtt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ogutahgu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sbasczdo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ccwhxplb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lxqwtdiy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qqhqiveq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3aelfnnvo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3byrrfbzg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zfmrhtvo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mrayzdcg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddcxrhes.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ueejpxlh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ftnqpzyu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ecawqqty.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3fvtzdhid.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vtwvppbv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kjsjzxwh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iqwzxulc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zkzytpvq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ztatmwoo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ccsoqagj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hkefgctl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3cuuonves.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yvomoqbc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckuigkzl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lidqmigi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wqmpxalz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rkjjmvhu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3uspfggvb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rbobezif.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ugruwqpj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rstmybiu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lobuvnis.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rvqvvtbj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zahfmktp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ggjlgozr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uoygqdkm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ruxzxcjq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wvghnhrj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3scezqcoy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrsjbkmw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zvatrgzq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mxcbasmv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fvlrewgf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3buwnnkbw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nxkckggh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jgeosbcf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yreemilo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mcmtetgq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3awfrdxpa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jrctcpnt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kibfvtqv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jvwrkfro.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sjyraqba.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zahktmia.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kilptaeq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nwvxqkay.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3iayxppha.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lsmjyhfd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zvhpnfbk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hgaeuxsp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ngogyswq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3panbmydi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bxxkycqh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eaeadvah.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3myozhztb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mnlyoycm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wnuxhbcx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcubeyye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qwbdukmx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mehfphvj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cpjanhvc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3shdvthua.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ptpqtcen.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3iwariqip.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3uiigunwu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3oytdqwdh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vpltawls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfurgnwj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hbiwyuri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjtniwmg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3keyptmwu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3obrxhcbi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hjwlahng.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vlqfqawu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pvrtxnsu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pansiulj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wgsqclag.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3haoehioy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jfcnipki.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pvjkmvaq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbeeeqkj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wmfrtxru.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3odrkwaok.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3cvpcduwz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jjmdqsds.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3exvapsam.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zswexhbm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3upnhswel.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lywspdyw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fmgovhff.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yqzpgrkk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xjmzwmzw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3irvvdwht.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zhpsgair.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pgknvaoi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhmdbvbz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3eopjazfe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3twexthau.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dacslyuy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cywqciil.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ruiktppc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pekgnvfk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rropjmnb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qrmuyxph.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vfxbilgh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fvezocdy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jgkbfwho.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3knpazisn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cogzxlxp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fheqtnoj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tfpozasn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wijmojnd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hwtbqxkp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jjkczkhe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zvvklqwm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bnjfbtud.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3osbnfrfx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3srqbavlg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3czqmdzdy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tlvbtguj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qdchovls.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bqmskpkn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bqahvlym.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vfmhtevc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dhojovnl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fsbnnsoo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3phiqauxs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fetagbcf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vrtozday.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qxzlibdo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3hpozdpjd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tavxashc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hoskujvw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3goyizkyt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3iepdvlax.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dioovkrq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bbxhgfbb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3urkivrpo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3bpqioeoo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3crqxpxnw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bdptyjef.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lwjyoxfy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wuuxmwyw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lllubqoq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3brgjpuzk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3txkiwbfk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pefshygb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lyqbaqqi.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ttjggasi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cjzovtkz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qomfwquf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rgzjlgmj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zvtxghzs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hfphuxik.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ykhrecpq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ictjdajz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pkcrdjtc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ltadjula.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yvgfulzx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qbtrczlu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qtjmqjwd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rvbevdbe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hifygyai.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xasnvppy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3guqtrmox.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rqrutibv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rvnyjeuw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ypknhfju.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rpmgdfmj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyholtwv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdqmdtfu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3blwnzdyc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vlnxshwg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmhivmqr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cvbnbswg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qliqwqtf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3urhvfogt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xzaxewws.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3cfqzcrya.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3luoidocv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kwrlehii.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rbmpaqmr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cupvocql.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ictgunxf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3byiafklu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vbfzglst.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xjsmigkn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dzdvpvlg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lirwmiwe.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rhgzpviz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3udkzvujt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mtzyqdek.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fctvbkky.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tknurirb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wutguykr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3taltsofl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ppeykobw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzyvlgzg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bdkiehnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfjqgvet.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bgajyrhb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3agwhenzl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wbvfttss.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gjjsrpjr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fdwzglob.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ehxernrq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kwnpgjsj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3fmsbvuip.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vehbcmxr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gzdqgrfz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gzotjzjd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nqtojupe.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ogidehom.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gbdagmzv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3gzhrqjal.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ygyfvbxu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cdjmhddv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gxurntzw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3nptwaztk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vtykfjfj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uxkrlfky.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jqvvimvb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hoftwnzu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3epjqzpdm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3molsbhbd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejlwvwfy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ojuctpog.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vewuozmq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rxkeyyxp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wtegtrsw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vkemfubn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vauwwzgd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zqnqayhe.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vimzshim.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bwshkvqq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yhthizkp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ofrhydfj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3onbxfenr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rigilykk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dtcnwohj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ycfpbwam.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nifuxonx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jnrubptp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mhjtfkri.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxpefwcw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ixsuceqs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pyepkcfh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vctzbjum.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kgntxamm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3krngabtx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rzetqvab.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3utzeaism.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eqlxjemd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fnprbxof.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uhhiuqqn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hzozpahx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3namxgavc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zjjqmxbz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3higcqhtt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zrjvsnso.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kmbtunhw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vhfbzjsm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tcvewzbg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dsdsjbzm.html


<!-- 参考信息 -->