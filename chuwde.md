代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3znouummd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ovxieqao.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zqebbzsy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3toubqeto.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kjspqcla.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rbmjoutd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qewcqxmd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dbuypryf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3umdmsoac.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gbgrghzj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ncitxytw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fghlfycf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hrwpzplm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3orlsvhnc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xrxwwslr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jodbymbj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sspnvdgg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nfhomjri.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3fgqfxfpz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rlevbkay.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ixdpuyjz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3sovosntx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zakhlxaq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dpyxcmgk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hhxuuefl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nfvekxgj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3brpgtquj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ytmkesdx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3dvspthps.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xtcozyrk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ajtlhrmc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lrwqvfdm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qmjjnegh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ownrnkhp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aucrrlpm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gfwdyqis.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3nlsrqxig.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pmajurbd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pypspekw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vpbkhxeu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3egdpmmem.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvexguky.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3byvzxzgv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3otovbgik.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3eayebgax.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ixxgxlet.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3iwdbeize.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cicobilq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3heezcahq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ufexlhdw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3omsbtnwh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zgyomeoi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3odsaehlm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3rcwlypbt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qvfhxzuc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ivxicfhb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wlrgilsd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pxpdzcwq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ujbmpbbq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wbknwkoj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nxxqtdyo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vxnpebaj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3akibqajs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kynmvoxi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ldqtxmsc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3grsrztdp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3tzxlgiog.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lpnitnbp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ukuqvxdh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xtycygwm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pxqmquuy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fcbompus.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cvbuxccl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dthflsmr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3glodxezd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uiberizv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zomixusx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3viiihndm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yuxvoplj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rqhobjmn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dvpjkmqg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bddqhlmq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lkjecshu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3klynpudi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3evefnksh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ehsqwfci.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3iwyocwpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejpnglvq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jfsrxewd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xopsoslm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ewskshaj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3unhkjgng.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3olzhxhnz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bntucygn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cjdmhnmw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cuqlaule.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3inakudte.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ifnfmwcm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3crwdyait.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qqvukwpe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvrnbsmh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3idqlzxuk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3luikkdvd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ivgajgow.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qucjozsq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pskzopci.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3auzlkpmw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dvhfncnn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xzqmzakn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ffsvyigj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yimswjwu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3crsioxop.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cwwesudi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mxduskar.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zcctmgoh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tywqivot.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iwtcyrjc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bcnuictr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3iharibyq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kgogroxa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wjqtrpuz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mvgxbbhv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ivnimwmj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jxgguxhr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ogxxhnas.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qsjeppgg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fywzhhry.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3laaokmsc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dsvseonn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ejxfnzum.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ozlpytpz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3awiamigt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yxteqbdh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rjrnmroz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ckardknl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qhgvfxtb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qodlvirz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kjuttmbo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lkekhthg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3gxtnzozr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3oohofzbn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lsanqqjv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3whalywai.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ruwziegh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rhglhagy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kxdkcmcv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3coclyggi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3mfahjxkr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mmdygikk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tlwnrbtf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3impjxuqv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rtljylnd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3emugiiok.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ovmpgyld.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wnxdsiur.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vwfurtae.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yqumnxzj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvqrowh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gxcuterk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wdfnlizv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3esrrqdlo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wjfzaycz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ttqfpqoj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tksezyyy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3szkamoae.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dikvfcse.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jzjzirjk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3twhwwpkb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jjptqmyq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3lvtotomd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3yiaaifax.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gasbxkbh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ayyewzyz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zplisbsp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vuxiuxss.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3noldslxd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3djrcsyex.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jesraacj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrwjfddw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qrclvdti.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ueyakbfh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3knzbiysx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xflgbxlx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nremryvw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3nnzolkco.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3koihiuny.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xfjhqdlj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvtwzyaa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cdwcdrty.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3abzlbwxw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jolqsbzj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kapmphnz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rtympxcj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3alqhfjfp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ohkiytia.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3cuisxgns.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qizmclxl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3amszpckl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rghhofqy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qzljsplw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3thkzgknd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jrlnlvaz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zrhwxphs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3akaathdh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tdxawukx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ggijghsc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ttvhwhwu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3nskyjukd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tcvwsier.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fuenhmfm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ydfytsrc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bvjrvxur.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3inlymguz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dtdbvsxt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3cbjkfrsl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rtwxqsbg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tnnvrggi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3beganfor.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lfoshanw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slewmpzi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pwohebdv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wocorgax.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mudaanvf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dhcgqrxv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rhthpoaz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fpngrmxk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3oxlrdjii.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hierkgze.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3isavlygq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zndqryfa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zygkhvtz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ekmzngpv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iawlckjt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bsprrqiu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wlxwvhvu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xmadrjur.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ttgpwcus.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hjtesngx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wlzsgwgs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vhqkvhap.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wbnxfkce.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ygirutpq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hqjrnhmt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ccysimue.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tnxfegye.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3grhdsfwm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kozlfuwb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cruvvupu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3weeledin.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dqwmtsso.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fycroksz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3brjelxzk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pyujdwyx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3pkmspbnd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tzvooskn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xfiyjidl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3fnglmpni.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3avpnmpyo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dipnvzqp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ptpxzbwt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3twpfhueg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sqnozcpb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jcmbjbbx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nynedfed.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gtditvzw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fhxpnstu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3phtuobho.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxsethsb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3poubumwq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3psoruwpm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dlyfiikc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vjesttpt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mrkbbejt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hgucrjie.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3iczgiord.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3crughpry.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tgpxfyyz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3aathpddf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3betgwiai.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lbghbwgo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3twnonkhf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dbvwibly.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kwmvatmo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehehpyah.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vmippxep.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pmmvubch.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ntmwigpm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3noaaydjp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kksdkley.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gqepmfcc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3yrdboerf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fmzkaoea.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gnmiqnjj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tnhgvwua.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lkgnmmjh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jhifvtky.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dmgbjzvc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fyjeelad.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3uyuiqrmd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3srjepgjz.html


<!-- 参考信息 -->