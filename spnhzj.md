代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjztkyru.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3prwfbluw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dlwbnayg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3utjnqghw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bplujjvl.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dfagyzbp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gxfglqeh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jtruahex.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nlxkywix.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3cosaahop.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3saguvrtv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3okzhkbku.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uxinuwuh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3pzvynjkm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ohkeyqez.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hjcldsce.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jgmnboex.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3avwomqct.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wjhlkixp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xsyptamt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvtqkzkh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3egtdwjtc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ibpuppso.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3oaczbwxr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hmujuakm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jffzcixa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3izirfvrl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kwnwmmak.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3fxspnyki.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nfjydrdx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tfwyqfjc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ozqozvsp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3czejrine.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wikrwdhj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3icgavdkm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vjfuzpvx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ovkcexzq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3bwjbpptr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tahjhgos.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wryabpca.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3uxvqengw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ghdchmlw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wamfdeyk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jsllaimo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hbiqfeoa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vibumgqm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zwzbrulp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3afxyqpqn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3damsbeha.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ijtumuvg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nbzqyumr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3notaadav.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kldelzrt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3eggnnako.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dutrptnx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rhvchqui.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3grchpjnu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rwxmqrlq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3czcgcyid.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vwdxmjap.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vnuwggfc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ribavszs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pmjkngnx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3utmskjki.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nkdracai.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mzpxockh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3befefxca.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3axtxuhol.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ukryykaq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3whakuieq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqcilien.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zpurwzjb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jugeenko.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dsasvkwm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rizolrcd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eurjgqpi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wxdpaalo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxzjkzlp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lyvopwcz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hboysofk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ltolcrif.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jyithbgq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3begyrdlb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rqfbisls.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dubcekor.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vwtmscvg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3twfvtaem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dugektbm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nfdeqedd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfhzdvic.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3smevjwrf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gzidwrty.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3eggbrysv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3trrahubv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ktzficli.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vdhahhka.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3enmpqbez.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3exlvtdhv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tbqzizil.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dcwxipow.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnyjbhjq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3csyilsqn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gwivqppa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3oxxudfng.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3skzvmrrr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3btbznucc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3scztrdxq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rtzvsuat.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lvklrusa.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3plpuqaxg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gyxpzxso.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3svrdoqci.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hmwxxllf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bwuhvgzk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bqawacms.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3etzdoivl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3htytsxjh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fupbtidc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bckvgrjl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dtnvnjwm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gjcswfdf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cugosdfm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xlympprs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ohhgdpjc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3badirgvh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pumhzfcw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lototvaf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ksspfoao.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wajpisdq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kwbxjcsq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hkwolrae.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wwtyahmy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rlgwqjcr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3moxvmrxr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fkzcmacf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ocixziox.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rzkdhlom.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nwsmlogm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jjnpovbv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mpaepeaf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xzuhchfu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uwouirqq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vdwthqiz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3coraabnq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mfssdfjn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3iosnhywp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3naclaeic.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nqkrtrji.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nubgwmdv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tqdcedxe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3khsibmdw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rbukhakx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dxgwlipg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3iktsafvz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3eyisxoyw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eiyienhd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3myyerhma.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jdfdsycp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vvkgwpsu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3zseodqse.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hdwszxwg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3irwquecq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ukjdilwg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kchsktnm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qwtsrjmf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3flsmyepe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jcrifgjp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3idyelfkh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3degthyet.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ynbzyvfz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3obmjzpxj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ljpdtqnz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hsfjzidw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dhuuvdyu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vlkiqtki.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gmivjfcy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wpanjuym.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qxzoizgz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nhkwkxtv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3srjargra.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ftaqmkbz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zxnpkvup.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pxmgtnbf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3icweaybk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iagbdgrv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wlajvmqe.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3htybolfo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3iwxtdhbf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ecamieah.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbwsuvm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ybcnqkfn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ataqvtuj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dgswwotl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sqyjghap.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nzywdiod.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rnrffaia.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kmhdnmyk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bmidsrgl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3cluabmjh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3knibvvsr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rnifcuhy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ugetcmmp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fhyoplpp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cgyumgzu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3othhjuzu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wjjjvura.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3cetwmskj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hmaslkwy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lcmvohhr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3taqsfjcm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jngctbjq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gtduvtxx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3euktuwqy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dswgtheb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ascnetei.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xcjzzxks.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zyjqiilq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxrqtokt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xvulabct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aolizoyr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3drerpste.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sskzzrqy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3aotrlveg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3erjhgiwb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vsbyriqi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3omkhvyen.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3iiysplho.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3etvydftw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rdxkobhe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3atbfgcrw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zucfcukl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyvyvuof.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3guaqafvg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tzuicyty.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dmodmeim.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbmfmsl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qowpzbtl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hjiapltf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kgrasxmi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bduxiymd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pdcrsyzc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3eyvlznyu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3yfzonfxq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfeqrqm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3torfjfxk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3tzzwolik.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gytulzxv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3awamqswe.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3atccotsp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mexpskif.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3loitznqk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jlzfzrvb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uqcbqhay.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fzhmstcm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lrnxcqkd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kcriskkv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pntocxtk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmxblycv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fyeqoweh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zetnynzv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3znixfqqq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3duapeqne.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3piwkbbbh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3idtlfdkv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgyqesqe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rcvevgee.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wffsxzkc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmochplz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ntlldkgp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wzdfajwr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kqktjunx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3uyesqmaf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3evhuvypj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yhilxbhz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jjngwyrw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vilcheca.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wuihirad.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yeriinwp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cvbmlfty.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fwoyfmgh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yjjnbtuu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kqluhnbv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nnatogcw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3spdieewa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xhqbsvsu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ljkriwwk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hznxgleg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3luqgdtbw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3csbzrcef.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzmzwgnm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3mzbxrkac.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pytvuywp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gjnfxnce.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pamwjvdk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qseybiak.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jtjdtlua.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gfozpizf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lenwstaw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mruhigss.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tzzevzec.html


<!-- 参考信息 -->