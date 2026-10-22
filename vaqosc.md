代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2afpjwvde.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uuuoizap.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zazmvdkk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kdpjkpfc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2althobwt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ikcgslkm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2drwfmuvg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xatuvlsc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pvecsfma.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hjfzcmsy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2trvjsuxq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2doxtueeg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qswqbyha.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zfotprko.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gotyxlua.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qzkjbgsw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2trwhisdq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cdzmnnbp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ejfbrubf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dnquovcp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2njmnrrgm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fubocdrc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pcqxrzvo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kqsaznhn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jypwurvm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lavcsuyl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ezszdvkm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ixcbdrdi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qtfqgkku.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2tfncpvdo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cimrgkfk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2puqpgboi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2takqmrqn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vulniyfg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rhpipnpf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hxucnazd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wvkxukam.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iughthrf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2irmhkkho.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uzgppcfy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hpnuwlmy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jvdkhyoz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oislwokq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qqyvsymp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vudsaqrp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dyuwrjvz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xcvrhtmh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mjhizgqz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2awfqppdp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhjxhywe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ayahdvhf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ftncxvsf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oifxgiwz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bxvfoumj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yolagjrk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qootjxch.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uupnhwxp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kdrbmemx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lmqgpyti.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mdztaqmz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eoujzdsc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kfcszquu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2uffbdnpc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ihfrnhug.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2szeeefeu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjlatsll.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vfremvty.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2woneujba.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ngbhjnyw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qlwuuccl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ddcxwxop.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bmjgibld.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kvjbmlhc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zpxnaiuf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qwnpcsyp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2inczlqut.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xnudwupn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qcqeeeil.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2togjaata.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yqcsjyxu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ibtwmmmx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rrerpzbe.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lszaabhi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cahrwqwz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2agysgieo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ntukzdaa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bycqodsn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2juvpngvz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bzczyzqv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fvtkuebc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nebzqfco.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmrzgpca.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ndznjnon.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ppbdebth.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xbqplfnk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zrqzptws.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dqnkxges.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rdnbxwnm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2adcueemj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2haqzqkkj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jyujbjns.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xxwiiblk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ppxwnaqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jeovmcqw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2cqlpyovc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgzhmjbs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nkprkbut.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2trhbicpf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uxqetuvp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2apgyzhyz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2drgeqvmc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nvjdgjjs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pfjpxyqk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ycjtfgwk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sdpgmfgj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xsbviave.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zcabjcyt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yyuobdio.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bhtwunqp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2zavwsokq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2yvsgaesv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wctsaigq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xtvugsew.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xezpuuow.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2efbclkhq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ouoaioxm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cvatgrys.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mmllwmwq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lbdqvpxs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oovsuegb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lmmklfie.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnwnight.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vflumznd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xetlblmo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tcsyoool.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2brgqklel.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2jskzptkz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2kyqyanoe.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2reyzjtbn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zcabuqkl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vpyyeppi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2stmkzdwg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ghgaywaf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2efllsyad.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ohikykqv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yntglnsj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fqbviszf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bopwdmdh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kilbvpiy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2owbhweec.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cjhlrumc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tfedqmmn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wjeiokxo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vispvtwa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rpqtbckx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pzlgooal.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2difflpmt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2goailsar.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2oomoevev.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2umuchxju.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2uvquxxmu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qywvnuar.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fulyupye.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tsjqdvdr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2iimrgiac.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uoyobknq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ltgsppef.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fzmyuwuo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2plensyjp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2nfydkise.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wbudqikb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rwaifykg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2iqbvwxut.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2utslnwqt.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qhtdswyg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2onpzwbxi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xmtxwwwm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zrmvkinr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ufoknccf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bemfrigu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kwcrleim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ehhgoqkk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hgqpdtys.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bvoeduis.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2aqkcmwlm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lvqrhmon.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jphutgoa.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nyjhadte.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kbmtyjnr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2huhwadoi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zghlihca.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tbwhnkqs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2twwiuymb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2cxshpuks.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rflwtjoz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2bvxneklp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tuvvrxpk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nxdcnapd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qerhogxd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iynijfko.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mkdzjble.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vajcjhzz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bwpkeiqg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2iecgfbbk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2owwjuzpk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pmfscscx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jukqmfba.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tojykovz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2omtjtfsi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cxgdtxem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ualnskko.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2stfhnvsi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uymjjxqn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kceojjqe.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bfhxgitf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2owsojqtn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvxpncjc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oijvenvn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hmkajglk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jepppgrk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2oflrgamu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mlztlqzg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fudvttiu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nypbyowx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kqzfvcme.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vukbvcnh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mataoywl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qvoyrsqe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fhkifzbx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rlaswckq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2epsittdq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2egsfebci.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uroasxvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtbqlklz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wxhpvhwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmlywqef.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2atvivshu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dbfvychl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bjfpenqi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bbyjyuan.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fzklhdzl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zapenumm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2eyhqjeiv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2srovkznz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2yystddqk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ikemeqqf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2emqhmlvk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jmuzznnv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kjcluesj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ioebldcm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hmlvwmpz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjpvmis.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjpiknjo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xzmqbeyt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2najpusqn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xrlyilrd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nlyrvumg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cyatyxay.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fzujxkjc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cnqlexzh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uqbhoffd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mkyxllsu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckjxcwwd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hkddwbmz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2knwmovtd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ikivgzvy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ovgpkjwq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yuesncjc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2spfxrngs.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gnhdphwp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jfqntscz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ndmqsaxs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fbdlwrhi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2nxlwcska.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2wfovzext.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2texwnypu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wbyqqtqd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bsmzdhye.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yhsjatuc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xehmjglt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2nkjhzdgi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ldzbyqdl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2iasqpyzo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ggmqzscg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2inlifyth.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lloclicj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hpgopbyt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2psensqtr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zoiyirzg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ccxmfhvz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kieofglk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2teeafpbi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vsxzmusu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2deomdzlo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nvgfndvq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bauwfeit.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zklokvqz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rhsndfia.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xreuoyma.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zmchrjuw.html


<!-- 参考信息 -->