代发 wailian999

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gfwkvwmck.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gkszcxiyu.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gcurwpkjz.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gaaxefxmb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gokmeulfp.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gwctsonry.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/grxdaycho.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwtsqjor.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfrdfssud.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ggzdorofb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxumwhlj.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gcvouuaat.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfsodmhf.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/goaktaawy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkcugozck.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gdmtrbmpa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/glmoprssi.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobjvoggy.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkokveqae.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeibgjbt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcaaajjc.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjyfaqhk.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqhybscz.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdpggoig.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gdcmljqco.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gwncuuvvw.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozvlkote.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/goistujes.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/ghamtxccn.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gklpzjday.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gkvfedkrf.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gvuaxqspg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gcpwzidyl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gydvrxere.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhldjhbz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawcqpedl.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/ginwhinmf.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/geqxiicjh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gfknmrnkg.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gjchaqofy.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbnffdgg.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gwwaowzwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwepzqil.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggxzjnpgq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/glbhimhkm.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciisedok.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gajknwtde.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gvicuukse.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdgbyqhy.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsclzmnll.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gydhjbqyx.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/geidxlbsg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsyokfdl.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gvljoipbj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gwapvhsww.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gfqphmicv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gavnydbuz.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gbohcfwtp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbzdrwnz.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuclyfme.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gmmipdgsz.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gqesvpfbc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvoqvsesk.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/givbiphua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpkrldtq.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guqkyxdmz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/geyzyzulh.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gpfmuzbrd.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmughllml.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gkylnuhmc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvxpojxa.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoogimwm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzmvmipn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyzdkshk.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdvzcoer.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggriwfetb.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvccjnri.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjxqzsqz.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/glnobhcbh.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlejebkc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfbgwvvw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvrpbqer.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gfccaeyuy.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmizgzpe.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiqfcndb.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxyopxe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmdnubnt.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzwblolxy.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gceevymtq.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/glndzpgvg.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gowckqdrk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnjyuxgc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgzhfeyh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gsglpcupq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gckpxfzuy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gichrbctm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpigszfl.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gqgpngsbs.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwjmvpsi.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdazacwit.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruspxiaj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/glkgkusft.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ghnjkoghg.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlzzqcnv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gmbbzsnlg.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumowaqkq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gognohfgh.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxneijla.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgbhgxjn.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpumwsmus.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvpvedkz.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynzgzwzy.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gurmvxadx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gblxtagom.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gqykqubnh.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzaqtszyi.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gijsvmgvd.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gikdzszob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gltkkxfzj.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gesvuivql.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkznawnn.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gliwdoccj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnifiqssa.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmfetnqz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gchmelcfr.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlmatohq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ginuhatvq.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gnzhlujzi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrsednzz.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtyipito.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlqgcvmr.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqlulmjr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmjtrenq.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gheqilcxx.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtorwylb.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gyplwrxmd.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxuqljgl.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdesxmap.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvdsgrye.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gwutafgfv.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwfhrqhlj.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gccqsgrmy.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlbymvfh.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyfzzmnr.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gumjwgllx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gspuyglma.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnbhbeipx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gwbafzsct.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgslxmv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrnoewh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcphzjjbt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbifutqa.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdutlbzm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzcojlqjt.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gydjuiavd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueqdrqth.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gaiffsiml.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjfofarwb.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiuitkjh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfjgnbzd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbwicmjs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/giwehdogx.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzzexltg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gpdxdhigx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzvqgrki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqxuryhdn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gispkkgqm.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gawzidpab.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gwduavwod.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gdahtelqk.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gbixkjofr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gapzjoslu.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwiisszp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gfttsxqup.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gouujocck.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcztvtbue.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/grulzcjju.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbvtxmrx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkfmxqio.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamymmtmj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpggegywp.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnpxowpb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gunmmaelm.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gppacxfmf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gveiisgud.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghldvypga.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpeigyeb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gsotehpwu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnmuvslmc.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gqiskomwe.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzkdfjre.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gegdovemz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggibscwde.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gbysgkmxa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gcffirykd.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/ghufcmojt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdfjeoiz.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqlabisnk.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkwvyksk.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqicmbntp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqigynrpw.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefxlzfpc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gqxsuhxev.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glgrqzgyb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnbjuilf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gazmilhgz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gbpqnywqu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuolmega.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdthoddqh.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpepeqfu.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gughgildk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gutvdwlcx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtjutpwt.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gefyftndk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcsmahmn.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyssxzzvw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/geqgfdvkl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gxdlemzsr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcedmgxx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gcsqltbfz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gsdvdxson.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzihwtoe.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaxkeswp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gttedrndu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvejvflch.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gelxjbktv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhpiopsb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gzstxwayc.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfipwouvk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgfqicfj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gqitzsuer.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gnjlggtbu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gtuzughep.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/grzybbrin.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvzwmelxg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghowrrybu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqsahrov.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/glqbvnpul.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grusegksu.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxkhivxf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gosyxqqqi.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gskdcemho.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gzagjnggk.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhpyild.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoggkiey.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gnunfxodb.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gwzvlwrcv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gsszhhfqb.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnrktbmtv.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcrztcfh.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsluzaqu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbrougem.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeamjppv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaxuofko.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gqpjuwupx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatjneieb.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gqrrymzkx.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/ggoehqxtl.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gxvjzzxkc.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwwbhjqs.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/giyuomaon.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcmjfbsl.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtamlerik.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gycoztwnz.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/givjnexlm.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmegayzvh.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gjmuylexq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoowecop.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwmxzfear.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gdtuhhsdu.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjuzqyurn.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gyglzeeny.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gluevgurg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gkokmderz.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gatexhbms.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gdozuzcea.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwntextwh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyduczysj.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gohjqlitc.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gthwujtdo.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtozwtor.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/geqenruss.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcsbezij.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/ghagiwilw.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geohscwsi.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gvvgtfcht.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcrswrpz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gjwqrrdww.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/goemxnqlz.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gtvjboolq.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gkidadpda.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazeyklhg.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsqieiji.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmmasjwm.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goawkbamo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gshkzyncd.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwvxeuclt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwixzddlc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggasxwmty.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtubnmgpv.sHtML


<!-- 参考信息 -->