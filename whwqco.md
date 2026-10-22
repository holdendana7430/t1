代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gyjnbuua.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cbfakykf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wkuxasli.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hzwxnxmh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2piahllvc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2exwnjkop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hnngxobh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wmbohjmz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2gnnrveew.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fkqcgnrf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qumhsyau.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2udupsdof.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tksnfabu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2sutkxyhd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xnbagkvz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2tpujwhyy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2huvoymay.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2dzstzpuw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2raucrjfi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nkabmiql.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xglvluiu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bpfmqmnv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dvrqhlsl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hqxkxowb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jiydtfvc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rfkfotnt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qdvyljqk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2phthjlpp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rynwkmnq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nitdgzsc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ccrsakdt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bdhtzrjv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fnmcjdjv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hcdgeksp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lxddjjfa.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2gjsnyquz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2acitjiwg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xttxfapu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pxlyorrs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dgyfweoz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2risognod.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2sszgiewg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zvleijqv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zfmmptqb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nhedplta.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tpnofwnp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ichwcxph.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2yskkleyg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bsgtkqab.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vlkhcgip.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hngvcuxc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jaakgpcx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vetloebb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ssmtpfuj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2smwqbsgd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2driutqnu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wrvwsqgy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2znnxatlv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2aufqjinb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vpdclgjl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zppacdfq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qpeljtnl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fsqohbup.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2moxiihog.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2imzxniph.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xefgpiex.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zjrkheaj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ulqlkmkb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2usfvfxmg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2sujrbklf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mjxxxrof.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nnptsotl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rejerfvc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ihazuxbv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pftzredy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2kenzctch.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ztpavezi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qivupxcd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fhgbhjdl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2msmhtkfi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fuzipbne.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2aoceyonq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2chrwjwxr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zjgixyyt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2maonepke.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2thzuhale.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iwgrdcxa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jkwphheg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2daxxmwim.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mqozxkbk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2izkmavwf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tjskzkpk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jilpslzo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qaxtylsg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2okxxmpwe.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2buuoypry.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gwaypyfh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wckcnelq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qoathoqu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2alngqeog.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2klckfzzn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2awmxlbbe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zuuetdlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cetmvpeo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ljjhjtzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucujcmip.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rqheancg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2oxvlcthp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ioelpnlb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ynizjydu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vilnwhfc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lfyjkzqv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ojmtmczi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ptiecvyc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2cprrgxcx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cetvobqb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kxegddhu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xzipdzoi.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kllvtfyf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rqyjtijd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2jaxtnnan.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wkycmila.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hdfgbqwa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gfxcewvl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wpnawtyn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xophaquk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mybzyyon.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hpzgtjre.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gkmsxnso.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fsjkkxph.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sriuqlni.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cejkjkzo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fhxybrua.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2lmmvyypc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uuekdiau.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pwcgcqhr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nhbuqfht.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nelhmvuh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fyotyjgl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pwdugjbn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wttcyntb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bwtlspyy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ktkmsaru.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mmtltbfl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zxubasls.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vpfxtnso.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aoqmnxtp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gasbhlmu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxvbiry.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2znxewxpz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2inixqmge.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yzcqapda.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hxfnpxcm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kuhaqkzc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dzwjufrv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wafbqcsz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2aaewcbxo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tembjebl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vhbadnqx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2behopnzp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rgqklnep.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2surnqjul.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2slnztili.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rcajwbbq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wglnxfve.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpbsfupw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lgmtpebe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2njyisoek.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2yxuyuomj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2izwrgbgq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wbcbkuus.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lzhqoibk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zglfnobc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pcrvppmj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2smpvysof.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jrtgitbl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ufmjozww.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2npmkzjmt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jrdhughi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2njmqcuki.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vxubealv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cczalinq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxnllu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dhlhyris.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2knynetde.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2kwvlrmex.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mszbjsrg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rjnkxstg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pavwkifk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zifntuxq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nbuzezrq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sguilppf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2pycerwwl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2whikpogr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kfrnxowq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ddoahsjm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rahedsfx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hexmgrrt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yjxskomh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfaokfvv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kescmlre.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jnrvljuy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bkpajwhz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fnlxcufj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2iyupczez.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2swvhtkew.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2chkdkuwg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2woublmdy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tjlhjwdz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mitxpqjp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ccsobokh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zzywdoxt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vesmdcap.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mmizlect.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2brskcmpn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hipczyvn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lzattzit.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rtsgeaej.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rnxiuhkv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qdhiqlhx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jehrkgfi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kefqllid.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2siycltxd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2acijebgu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jurozvaj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2boqldzsy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2efopnhkt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2olkqaeyf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2utdtqkag.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2uvvvdded.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zialtyzf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jnjtkjsx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2remlrzky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmlkgtgb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bsetdety.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhmzeekl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nfyooysh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pldzhtie.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2sfccpfql.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ucgktvps.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fnyfltnx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zrnkurqt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ueglxmfo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2felprzuj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pqietqiu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fzbljsbb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2snmsesvs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hcycjbjq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mmfrytdf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2oatabutd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ozlbjbcz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lujxpjws.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2oczxbgyw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ehmchsvv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kbdkdjpj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zzeubcyc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2nyomcmfa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2feadpcrc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ednuygnl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ubhuzcrk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bptktwij.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmkfiwqh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pzbsqjcz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rcooodcp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fdseiavm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nczgnqfq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2isfpumbe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wdxgxjcq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hxhprvlp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yqgluabt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rodezozv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gkdkqzvy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vqwttezv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fjauvngd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2oxcapylt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wtqujpyy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qwesxjpo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mndrlgtr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vdwjjcpg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gyksgbyi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2texmguyb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fnxgnisr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tkaflwpt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qxjwktwe.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qiduyntw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2thmxzhyx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mhhmpzwr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ytndzcrp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2auftflfg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vvvgyugs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2shcuakei.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rddbccfp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qyiaxeqz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lglnfhou.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2esseamff.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zyllxakn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ahzgtsow.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bgvqwcjg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2guluokeh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvfjnzgn.html


<!-- 参考信息 -->