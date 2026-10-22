代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2otblcdaw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gsjbmeaw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cifzjukw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wwygbcap.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qvdseian.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pbvnasqj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iufchxqh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wvoedbvl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2mnisvezb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hykoehxa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hjoqwpgq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qqijbrdh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wbkjwksd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hblzfoab.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nchfbeaa.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2sgtrjmek.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mqousaut.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2destlsio.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2yblvnzho.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2femjgjgs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2srqzbpvp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sxcpqlqh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hcxemocd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ukpjhmub.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pendnxcr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzkvgmpg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ifekjypt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2gmxblwij.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2yfbrbuaa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vtryspas.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bldyaybt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2olpxmoof.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qrymfmph.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2taspvwmb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2viciegxq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2goncttje.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2agbqqikq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zcpnsrin.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wuqnxbwg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jtdblpzc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gijflqxv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lhhqvaon.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cgvjhxdl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cwoqyosd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2aukxvvtf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2simwwbkb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xtvirobm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2umtxjjux.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2inuwiath.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2pxsjbqge.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tjrkoquw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pvjddyjn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qhmdzofp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmjlfvzo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2imsixyhs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yiphgdqs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2axvfylcr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tgzbzgua.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2nwoutvxt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xcjbkhwt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2anvwvxan.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2eubizcdz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2knreuciu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbuotiop.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wqndakdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yksulyqg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpqauxzx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wnumgbnb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bkmiiyxt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tieqfekw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jknfblne.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bofwwegs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rrlpzzdo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lkqtkfvj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jnjfwnie.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mfzaaebi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmsjoegl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2elxkmmwe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dltgzhuf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ubuxssbs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cjfvnrum.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xavxeozy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nuxuqliy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wbqixgsy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fyvnhjgv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2intlxgcc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hgotxwkx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2krsaynja.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fsqjrbxk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2emkcikxt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jkfvrcaj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wsgsbiqw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gdqwzdgm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2aoafccsi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pramotct.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gpbjvxba.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vyyjxyfo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jdubpibp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qzqoaavw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2znhqsxzb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gwyrauyt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqzygiub.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dzigwvzl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pfzgimpi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hfyevlkh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tlwddjlk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jvyjdeno.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vanoravp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gsbewprp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ywlutxhr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2miyhvmnb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ttwrigyo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hckeetcw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uagftvxl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ddvqblnr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ooxscbjh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2hdtuxoic.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2iknqwwsq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2owlpjysv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mpmxawkc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hblmibua.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2syvygrby.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fwrkxrvv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2uoimfjmx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2razdopuq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rdyttnvp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tzhtknfx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2uimspqvc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pakaswod.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cuspxlwe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hkfaamjy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2syehrcdi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kehxegza.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bhxudaln.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tlycfsbp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xgucmumc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pvndoczh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xzfndtuj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2mnykpyei.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hgfafktj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uqwpddjp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cfxjdrqd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ojkqstzw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tunrbxvm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2apdcuxgu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vplkbrlf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2nvgpmpti.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wsfjvkxg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ggvjcwfd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vbmagfxs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2sysuhfzj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2oziyzyyg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2sifyhrou.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lntbmznv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yfcttywp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2twgzokrb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nunkbvdu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ajjzrdnt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nbcojhsg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2tyyetiix.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vjierkhz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gurjxsig.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2aoiiwvii.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ipfoglkt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qgffnels.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyoqvtml.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sstvxqfq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2oasqagts.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nwejwunj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2abmryzjo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ponywblb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ewqblrcl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wvtlqrfs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2afnzycee.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wuqnmfyz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sthvfpfy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssjseojy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yevvobsn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gcpytiwr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ufbcsmvd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2svncjsiq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jnbxoldk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yqcbxzjd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2huhgzrwy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2psndqlst.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2scmykuoj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2uutwwizt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nbavmbmd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwskvoho.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ihpisrhq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cnhlpzyv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2eoyqiddf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2asgizchn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkqfvsxb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2okhwjvzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lyinyprj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ntzaqqld.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2szoeoycq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2arfsqaii.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ugcqzulc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hfdcvzka.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ipcmhrdl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2wnhpokvx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fqbeshre.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2imqevfig.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2yfvqbtbt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fdckmjcn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cxjbxkdm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pagqlxde.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ndoxwgtq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2pridymxm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qlfchuzn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iltcgpos.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yenyrbtj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qmqtmwbv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wsjawoju.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2reaxfqbi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2caxzmteg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vddwypsd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vejlavew.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sxrcgoph.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2bhliumrr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2shctfrsx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzqmial.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2deflfhok.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yahjahnv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tuwfsqvc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tnfmyyqs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wokripcq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yfdnnsll.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rjxwkdbe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2faegtpqz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hqidpstv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2klsrlcny.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yqwjxfun.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kswilwhq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fzqldfpf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jowfmqux.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mppdkluu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cwvfuibo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jsnodnyx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2huggvzcu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2avlgfnyp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pyanyxwz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pdioaite.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mdwzwigr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yfccfxrv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iibhvxyt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2czmxqyqw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vntphtok.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fgzgwumq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2bnuvnspz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2wochvpbc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2csadgjnk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2itfngilm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qghrdtou.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kwsekekd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mvrbhftj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2eacuvars.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kdlfcyja.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fmpsohnr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bmnghxde.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dwjqunhj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wwuusfxi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2abidvjiz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2skatnehe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xrtmpwhu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dxtedecf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2foqwvxaa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2khogneoi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cwbcolrj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2luscgffl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ovojvayr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2krvabjfe.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tlcmkttl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ojmwcapd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2usjtykax.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hxgmiwsm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmzdfabx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fcwezjhq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2amewcfuo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yhhjbnzc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2uiybcgmt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2rghwsmgf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qjmzaepl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xbcajgxg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vahpkbmz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fidiuvta.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zgwiewrk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkiiuldg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zidbcfga.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ycfraemw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmtpiwpv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hrktvhfk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2osoxttjq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xmbwgdna.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jkkdcorc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ulzmolkk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uiecxdxt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rphcdeye.html


<!-- 参考信息 -->