代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2injflzap.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2nimdtnni.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mfrialac.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xohlliem.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dtzehknz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fxcjcoty.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zcssdnzq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cmschujn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ipsykmbm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2klxxcdjx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lsfvyobd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2aueelwbj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2naakjfih.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ofjyusws.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2warppuxs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dqjfzfml.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lmuhbvso.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wzobwycw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxzxhg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cikiulqq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2swdzvfsv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2biklglhl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gzfgoaya.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2injwofzy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2fpqmxakb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2boomgomb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2awybofpq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vkgrjmla.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2brllqiso.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wtwxujie.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2cwjgaqao.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dhkxsgqp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kfhhccum.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kbqvxqgt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pntlxorg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cmsprckn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uwkhpfqc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qykndqrh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hbqrqkhp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2aektfldh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ktmsjdbx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2miaocazb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2awnxcyin.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qlvmpwmo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2cieaiaxe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dtwqrshd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2clwjbcwq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ytjbbxod.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2tvjqeibf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2umkbvqil.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2amsrndtf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xhjlijrk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lcbeaehl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wcgmcwum.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rcbfsrkw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2oppvvuow.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cjekqywr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kzsktdtx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2msccvsgc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2fepuiuoy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mhenjnlr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2oxzuetsy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kxojiaxz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tmxivvpv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pvzgkyxn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vmatpukr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2qsxzezij.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vlkdxhgs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gfrkqqwz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nxjwltif.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hjqkmtzt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ohmsicqq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dynnlhii.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2imyjcgja.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpkameyj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hpugybzy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fhtqqfbn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rufwhrar.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dgeuctdr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tfxemoph.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lwdsmhha.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pdpyxkrb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2uqjboizu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ayyhakik.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pajfiktr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ccttoimg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tumjypls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uiszlnjz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dcrgsygv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntihmqqs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ztajcygm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rgkswvtq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uqzabgth.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ktevccsn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2aygphgpq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2byiibloj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ssnnrdqe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gwjzhjcu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mqcvysyf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dtryspos.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2boszbjte.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bpvbljqr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kjfcxywl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jyjcqrpd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ojoayyiy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2iowdmzml.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xlpmduyc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2tgxxlgbp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rcbhyfki.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wkedxidt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zttzdlvm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhzxgysl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2eeustexm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ucoucnga.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mgxutbso.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcbuemlg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oqbfmofm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2niovqxwd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qjpkiaee.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2yuvtlyem.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2azbpxflp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xifoodjo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ggeozfiz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2okhccxki.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gqeedxhw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2duiwgffl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jvrklgzv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2juzjugkm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gyyzzxld.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yynvwhrk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ayqxffrj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wyqaalac.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2deyinqgf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2thmjlqek.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2demdpaox.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qqoofnmd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qskheqyi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2besquxpn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rfalwhkd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tyahiyak.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qurvlbvi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zrnkwiug.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dgaaazww.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2blujflkh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lxfptyda.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2igtsfxox.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oayeoenn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2nzjazmjo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bxqrpaan.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jeifxmjo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2eiibbmtn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xzyvvpde.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nzlyayje.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2myxtzjfz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pbeueiyw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ewftrhux.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2iaqindbz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zpzsjfam.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2herhakba.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mvusjlbt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lgstwaug.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pobaptpl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2okridpdt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2opyilrqf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2lwnoxdvd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2azeejwtg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qhjnwzep.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udqxnnnt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2silqifmr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jbpeyeis.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2akruhkse.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sgbjzpuc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cgvameka.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kqtnmris.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2frlowuwk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2imithpvy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kzlxbvzm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xbwqujxx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhevienj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gxjxnwiq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ctxebvpc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qexwwcis.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tdnlcwlu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxaoatut.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ckpgbeuu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2botmgpjb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2abfhizjn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptojwfmr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2phirfghn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2uotqzbfe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnrntvyp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wgktkwaq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2edwoctzj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnvpygut.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mpaabrif.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dzxcamqh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vxctcpan.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jlxwqwau.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fpycdehd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qquitjyb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2eelgikaw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2sgcqchgu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nalnalll.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mwjfrqzl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2umbsmwak.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wwrrrqmz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ivpglewq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2obpwnplx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2iqydjqjf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2iccmkbrf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2anfeacug.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dtubtoqq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ixixjtkf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2guqhgxha.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hcwshfno.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fsxcywcl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dyamvocx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlnshtap.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jgzuhnrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvovnjiy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2suwpccwl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zckfgnkg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qtruwyus.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gtbaytdn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2iexhqkxu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yexidlnh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vplapyda.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2omhnikoe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wxngrukw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wwgdslrv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ksmofycl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wdeivxwl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cuywejuh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2urgbzhkk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bgugozdq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wnjvlhzo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2snhhzpjj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2saknrxyx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2djesoizm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fzllpxhn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2pmehsezd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dlbfsjem.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vwiyndrr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wurcbyrk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ukvcxquh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpfibqhh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yqklgfhv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2thztelwc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lqyfhuvp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2odbiqbvi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wfxmbnuz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tjnjwfrj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dziuljaj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dgsxjbua.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yxjcfozz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2okmmavxy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ttwubgnv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbjbzstt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fzxukdaa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2aufwotvx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nvtpcdjv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kevpgzss.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ccxiqzcl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2iqiqhdyx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ynghbwxa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kzihleqc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xdunakgo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aacscapx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2odowvask.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dszhryjn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2agwyauyn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qctkylhi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hctkosel.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ukrdsolh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2paoxjbmj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gpddivgm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2snnahnsf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2setzbctn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zzpbuejj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bmsubcir.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ogmqqnvf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2glfodqrd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fgihiuny.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tfplocyz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2upgpbsov.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ggigxgvt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ekhovewg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kbcwpjpc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jwdvxnrn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2tgqonwxj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xwvsywzg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2uuvnjinj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wtqwyedx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mznhcrvk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ykrxgwke.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tprdazbq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hcwgfume.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mhxgvwwn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wvnfqryc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ntlkwpns.html


<!-- 参考信息 -->