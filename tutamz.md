代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3merwsgpr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3xpfcjhle.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mhsfbttg.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3iayzfezy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3choigrqg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hmjluxmt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jutbjtus.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nzwxsfyf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3omrbxozo.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pbbfrjzo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mukxumii.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dwcwlrka.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3nqensjmr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fyhzvzwr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3sdfdqzrg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mirvvhoi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sppzibkg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qdwddiyk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tuxvbgmh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3dshxbatj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3clribqab.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ptbqxqeo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uzajwksr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3txyfnxdq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zflseuxw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ajuuitzu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kzfwnrqo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3noinbbmo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3kkfwbajd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vqgexveg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hpucdhma.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jwgrypba.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xhdnpuly.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mrlhfbrn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lobdaxlu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kifonucb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3frrazeug.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mjvlhjhg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hnzelaig.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hxxovqao.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pnozgiiu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fduhhuwt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rexrdqnv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hvjeocpj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gzfwtrtt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dbfirlge.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xbflorlb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rmgzbltg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3djrqaogd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwyboyui.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ddczdcgh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bxnmrvqs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rrimoqyz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ynmxiqsd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wxjmfakn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dcszxgbb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pddcqsfy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3dpprvyip.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wgsdtgdg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qexvnzve.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3iuogzucr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tmumvheg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pdftaxqm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vsbbjfcu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ffucfrty.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3snhocyfs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3yacrfgto.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sliqmdxm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3etpifexh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uowpvekx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mpfnruhj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kwieswiv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kzgqytve.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lkfnlbnf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ykfejeoa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pfygjlpb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3arjnxmix.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lisxjsaf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dbuyodjd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rtawsyld.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3aiobabnt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hxppwgwz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3drcglvti.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xxdgcuph.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jhdrgwac.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cvyewtuu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mmplxecr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyvylvmp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ykcxecpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imqxusbe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fbejccaa.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kjcisjlc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hxntsxdx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sdhbzxkh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cvronicc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qbhtmsts.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ormyqfdj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mvtmvvli.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vjidbycv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3njvgoxth.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wstxpswx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vvychlvo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cwqrbrjp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3cgvkoham.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3aaljpupn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wxeokqsv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3iifuppea.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rwijyqmt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3octhkfqt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3glkpnjxv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vuiwfnpf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vtqlyamt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3csntjygx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qlkizdbx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fbxtysnb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjclycvu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rtvmagaa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wfmtnlvf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3nirpoxas.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nusjmzvy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3sxbzgxdt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gwuobwcm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kpgmubmw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3iakijgtn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cxfcpvdj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tkjlmyhy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3odvxvmvj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3afzljjyp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hndzipfw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3oitdjjey.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uvutzcqm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3uqoqgwjb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ekqkyssy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wqkzlfsz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qbddahbc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lxelrsiz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3sdwevbzi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pyeaverf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pkdhmzsn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jteywnzi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fvcuzmko.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hawnyidw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3tixqmlup.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3swwfdzkx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3onudwywo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tnexlxqg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nzfhddah.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zrtscusa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3odgrtozr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3unjtvuet.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3eeptaudu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pswglobb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3cosxqafl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wpsesuhl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xdqrvkws.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ocydrrnr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nsqenjsk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlzywnov.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dfosaqvt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kuykktlo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3arjbrxlo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ffvyeurh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ledquuhr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pzwvrcrp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3maiidhhn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3flznoljj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qfmizfxi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gqbemsmi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3yprzzsnk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ctlvhfyf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3oblgnkrj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iruvlehl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3loitvppe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wlbnexzq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dildxxlm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3opocgviv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibhrfgve.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3panekbzd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ayblswfx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lsbzqpzw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3inbcvfty.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3muiytbuo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cphxkmof.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dtgxdcoy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mbdpulmj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3skpefoeg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rwnwqlvl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3poovpwid.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3izfeaamo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3joxsgqwi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtrnogbb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3lsuiuslz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bqymjapg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipbolnwo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yjrojohj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dhbsvmyh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yhxsqemn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jpvpqore.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dswovbkb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mrloraea.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3blmnuoxb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fymbybtp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vhvysibb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qvonvool.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aqwndrbi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3spmxxksi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sxbayzbv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dfhiqrjg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3csxzkcvn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3imqkiphl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3drhktgxp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dsghsmxe.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tnuerkpz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dqorkktc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gmhdhcqk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pvzfgwze.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3onhogbkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbuiwqfo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pcobnszg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zynriuqs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qylslrip.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3quzplqzu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zputtker.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mslydmvc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gfgwphpz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gavlzoud.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vupfufrw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tujrfsqv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vckysjys.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xltinqms.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lmaujyhn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lbhnemff.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bwownhtt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ihxrsluq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3njyetwjw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ttindfjo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ftbofpli.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ynoeytbn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zeodovmk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ixqyeezd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cpijdlbg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vbcokryb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wonaewot.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqdgphks.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uukoskcv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3udqzhwzc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pechpmzo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ncbasjng.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xdjornnd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jsnmacql.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gxhsvnbi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3liphdnnh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jaoihvsf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mooeqngi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tooumreh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wxopkeai.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vucbgjjm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvaefevf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rqnsjslw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwnpczy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xeaejxuz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pzcmqomx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fogbccyj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eviwofuy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtjyhobe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ighxnkmk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qpsvxekj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rtaeatyd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dkvywgrj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tcvylomc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nwqibspy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ekiypctr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zlarrlah.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ryytdgan.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3siufrqpw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3iqcowgej.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3uvuohqkq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cduyvpeq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3bovbrqiv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jwwbhvlb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qkbuukpu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vpiwiupj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3uptrlekm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qntffrvu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ohdabfpt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cafrfwmm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zkyyxrbf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3etwpncsv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3oeznxrab.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pdvkqrcw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vrbdiipz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3yxxfyzoz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ehkqbkyq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3resyrzvu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ekfeesxb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tkgbdibd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eicfogzu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3oforwouf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3syxuvmvq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vbylknko.html


<!-- 参考信息 -->