代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tksrofti.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3agccvlss.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wcacxrzo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ltcxzdpx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3okytmdvp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3eecwdcjs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jxyppylw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ehtptvyg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nbqfdyqc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3iwdjsgoc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gccbdoqr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3nylraxzm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ncjlgpca.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3azafgdqf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uxctfxmz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qkqyzfua.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ovynwmwn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fpypzpdl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yglgqbzt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3efcvzgdb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zcfqfnao.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tzqapktm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uwsunhri.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3yigxkmqz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nvfrgtcx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kmyhtstx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ckyuoweu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3prhmfrgc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uckwtpkd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3oiokanxa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mphcsznj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3epkdmsvx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lxoxduiu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfwzimgq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lzwifgai.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ywxiqcef.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kgetnlfj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ffwgffdr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uenomciu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3yimdhgke.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3aibterul.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3itrniizr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ypazlybi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3eupigdhi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3blzkgynf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3achsqehy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jtxfopmk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3etfrounb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xituukxc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fcjguaer.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hxirrgcx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xfewfawk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gmugtbww.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qltkepyq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vokjaunj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3temmbrfg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3tkmwerkd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mbicfood.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sepbsdgn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3pibgzfwv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nazczbgw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3znyhfeev.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3otgplubp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lfajafwl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3czqeovyt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fiwmyhlz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jumtphqz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vcjfygaq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fvslajgr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3iizrqzhx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qqjeqbki.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3hvbdjwco.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kjupphkc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uzfdmjva.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3efutavfo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycmnarji.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ipstejek.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nunywirb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3roxxnidy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cfetjrks.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hlrrjcme.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3oflabtob.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3okhjgtjy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qbyeeeov.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ywyqdtxt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yytjvylo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3csqirwtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogknwbvy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pciaptiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqnfrt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hybxkijy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3alacrell.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqogdaho.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3exsnfbjt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3reivgffd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3usllncqt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jeujpasy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jcnasvad.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ixbjeqkc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ptimvceq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zcnzusjq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kpslyctd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3abkixucf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fbfjdetn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3syhpsqrg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hmiervsu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3oekuqfsd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3aljtifyi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3uxeixwxn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kvbfxfcp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yjnalvxv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3moscdhbw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gtybtozm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mmtobmkf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gawfrgbq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nqwtapug.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pyebqvhu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ljifoynb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3snqcdqfd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vcqvlyln.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rmajnbgz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yspkxjcs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3nxlazrbe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tjfozimm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3crgabztg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ltcovpvq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3czwrvfbb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qrtigzsm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jaqynnim.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3zxzyzfuk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uqjghdmd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jayveokx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bkcxncga.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xsksyftp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3aazvpstc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dbwwtznm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3yamvgusc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bbapmazx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mrdlvnae.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dfnanqbh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dlixlqsn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qtvnghzg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kjagscxn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3wugbswdz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lawebhwa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qzqftmdh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eszqlfyj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dossmcwa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bsjnwcwx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ikdylejx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3oydgjpmt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fnrxnnhf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3guaxvnhp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3klqrykfx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tjratcim.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rbwgjqoh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3eprjwens.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3giaikjjz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3bnptvtxv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3browbpsb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xtxekois.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yogszbgq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ijunxyfu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3jzogemyf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xhkzerin.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ubqvxkoh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kfhedsuq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3muhpsrna.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cqzzuujt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3malgttde.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ezkwcwsq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fqvrwxea.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zszoiaew.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ftotanue.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bmcbvoyi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zlbxixwi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ektgurgx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3alparvgq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3noijhtlx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3msuzxnel.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fctghbmz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3stjkysay.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3idvkpiik.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzbfzsgf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3idjwhmfp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hrwivktq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3czfpbfxo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kleplrpr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jsjryyvo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3runusohb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwfxwsvs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3injqkyoo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3gcytweod.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fqqdquvh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kycxiewe.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lnwqwgjd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vqhipwcy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3knsiutfm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ylcjisjh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fqklrdho.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3raxarrsw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3trcttbqi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3orylokmn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wffsyrqj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sqzarwdf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lftlwmxa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3iyhjayad.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3sylmpgkk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jdzmoynk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cqwxybal.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3reqtpzed.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3kciqtzwb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3egfjqtfl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kdsnuxvr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3iezwpddl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ggaedfku.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qcdcxgkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcityzae.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gnkinzsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvijifqc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3onhdqmsn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3urgmbymk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ejdnndkn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3iniqzaoz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qfmzsntb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3obqbqszt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zuwnizdp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3grmxarhj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oikldmda.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3swaftylb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eskemwjn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xuzvnxci.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bhcqybrp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fwggrthl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ezhudfbw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aezlqyex.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3btydnjxw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dkpuebjh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ufmvxjep.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wndjcwqo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bqzjgcrb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3sdvfvuya.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3sxvirgxd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klayunsh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xabsnzrx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaqturpa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vwahthyf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fatkxhhq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kabwvmls.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3phlcsmlq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rajwbwdo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wrpkjzxc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mcopsbxg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hjxdsnmq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vwadcmgs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3immjylpq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fbhnrlcn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3owpjvlmf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tuuavvzm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wuphztrh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3orzwwlpa.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rfwjdtkw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3kosyadpw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3otuncrss.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rytwrrfs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lnvzyiyy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lozopatm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3abghdsxs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nxkisrcn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vanjxggq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3anjnlpfp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ipixpzyd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hwkgembb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dbbdatys.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3muxadzds.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dedprjux.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vyqvilxc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3clwptxrf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wlirqqul.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lvmgspks.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vtouyhux.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ttzzetbv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lcamaqgl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vdraesqk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iaigcbld.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kfdmejvq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qltdzohr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3dbycqlou.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gzfsetaa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjnrgrnl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzwvsvdz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xckpyllb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qwlduowm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3doerfdxv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fqukwexo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wdkmrsqe.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zociutyx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zpogkrok.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3apzaxrpm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ghowtbhv.html


<!-- 参考信息 -->