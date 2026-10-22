代发 wailian999

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qpbomwse.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lrjiyami.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2abtoleer.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nzsqklgx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rdrvzvrr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wiecvhpj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fmyoytym.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2oqcrodaw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qonxvjhh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dxxsouqv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bgsvkcvh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyoftotv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2hgccqjev.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2sgpgbgcw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mlplmvjb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2uozutdpj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2awfrbvdo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sfwnnzgl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tswbvbak.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yqcilahh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pgzlsabo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cmlfxcrq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2amcsrmlk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rlhslldr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kojedhst.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ohibminv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yqyggczc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fovwbnqv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wmssmqbj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vrckszlb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yreineuu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2dyneklzl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gwrbbmjr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgbffylm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2exgjzgjr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2odrxllin.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2sbkkiflx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2idguihnn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jnlikcij.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zsiemcpt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yggbzfcc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ajnuzvif.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tgoirygn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zvojhqub.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2gfdkvucr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zdoxhput.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pektazpw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2qooravij.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ihsidibt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gczdoond.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hqgdgrbj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kkrrfzzn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2swpkejxv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2okcdfupn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qowngmcp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qqsaokdq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2npvcyppl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bjispcka.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vxytkipz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2srlmdlqh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gvhplklg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ahujogir.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dlpcrcsq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2hyherkqs.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dkcekplu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tznhfugw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uhrbmzdj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iaejtgxz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zegaaqme.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kkctdjqu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ofsefrbn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yoymvfgl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nlogjlqo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2eqloqnbj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pmevinja.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2towutesd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qqflzmoi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2odxgdnio.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yuwtkkiq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jvwkzdnl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ptqvcijt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2neqyxsli.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2alzcewoy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2iihjvciu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2oyllajbg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ktwpauqt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2rzognhzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezzkloof.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nxjeevkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osyceswp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tdtbshqs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2poylvihz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ijkkvoaf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ytmybetp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jsnxcwed.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nwnjwzvg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pmqrnsbj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2daooaure.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ikvzgmrw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bhnbdaui.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2utefgujg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gttirzyg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cubrdegz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dnywmdhh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lccymmfv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2bacbfsej.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2bfrthhsi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fatmjmip.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kqfdlktn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jmnwwetg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wmtvoyjg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sukyxrsv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2aabnjyou.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lszdhhcy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gfvwdzss.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nmkdtnot.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ltlrdlre.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pwkfwkaw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gqarxtcj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vuhtohuw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vfmqigov.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dlilwgpd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dqvjbjti.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2churyyui.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zvhozngl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bsmboyew.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kbsvtigc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xocotele.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xyyzrnpp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qutpnoqc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uovlffmc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wsuohmjw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jityzflj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nkzmlrtv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dbuikabi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kahaejpv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qxexrphv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ajtzbupc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2bsapkmse.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xcrvscbm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2viuhownp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kdygteyr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2clxmpgbv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2sshrgvyq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vxemfwro.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qdfukles.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gehwuulp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2rfaygpud.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2oucpzzcl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydsqqiqq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hrxxlbwc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zxchaeez.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rbzyxtpr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ozmgpzdz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2oyaoelkb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2frmouwhi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2tqxiwfst.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmerixdg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mhtdccpb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ocnnzdwi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2zdzquwzm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ruilutfe.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2holshqdv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnjhvjjw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2seabrkyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dzsoqkvx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2inyrhmab.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xefhjeua.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ukzxzejz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nwbckxrr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2npqqdloo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hbyechcd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zbmrkzkh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wkcyktvl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wrliowrq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2unvtlwlq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2nhmqvtbb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2smzzxaqs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kuympwzi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rojcwyen.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jriktuuc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bbvxlxdo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cqlalmjo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hssnnnxs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ufmhyufk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2penbhkct.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xzwlevek.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xajxqlmb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2uoizbmih.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pehquflv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfnjlmiq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2yvtccjne.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oqnjizxn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwajoxgw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ppyzegfx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2guthsuec.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ltiiskjo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rspfnwot.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ctotdyjg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2frqdbote.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2atoahbol.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vmbxwzzw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lvbktqgg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qqnetrli.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fixwpcwg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rplknepf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2aqhtejth.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fkvjgzsl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuxfjplr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ixrmjpdl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2nmdinybs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wrluicdf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bfatpsje.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pqcxxapr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2otvtdnpa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2wagzdgms.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lyendnze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2takxjdjq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iecxfhci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbiageyc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wbovjewk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qiyezhsk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lyhfefje.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wvcaswoy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2gwerlopx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rvijzafa.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yfovyopr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pooznywe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zzzrdskc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ytmpgixv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rqztpila.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uwbnstln.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cyywekuw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2grfmlphk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rbbutpux.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2utbikcir.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cetrsdal.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fdnucfow.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qhgonzaa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yblhlupd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ydpviiip.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dblxtxba.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ywsstsra.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xlsjayhf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yxjlbwac.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xknnahor.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rbgcieqe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dmvcdduo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tkryyoxv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mgeomjvd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ygjwehlt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zfxazcwl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2irxclyok.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vkkycccv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2viapvfyb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dbilysww.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wcrrbbjd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvprreim.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nmwpzrfn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2euwlollj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2acscgzwb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpxvvizy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ehbtpplk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ooylxemr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2gvpsctvh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2aqtkdzwi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uckaypvk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lsprppeb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jshhdibi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qbtgddtc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hzqpxrkr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ocnoixfc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xuvbirez.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rkpqwaeu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqqlrk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2bnetzhbq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rcuqmhjo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbgtann.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pnjpudud.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2upwwicum.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dkptjqxr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fbrrqgik.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nygwnnxj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2awwaxfdf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xslhglcs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vmwepkfx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2crxmefib.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lyptnqez.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2mmjwbjrs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mhyplpzc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gfsfdqab.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2yukvqhdh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sujdbpve.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2lcfcorhi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cszwyxtf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ejrwsdsi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yixgvrfu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vyiprzvk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nmrrcmbq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2japdzmjj.html


<!-- 参考信息 -->