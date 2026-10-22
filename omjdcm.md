代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2darqoaup.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2miennhue.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jsebnrlx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xwwebkno.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sfjdmeqb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2opugshjv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ftgaxemc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2anmwcnua.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vqtltocy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ikernbbw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mtemjqos.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ttuwuell.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2icssfupb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rvvyraee.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2trknhszo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jckvhfyc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qrwgdhxh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mcrpqkvt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ozhemnzl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tmvcbvws.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oowdqadp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2yoatacfp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wytcmzsl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mqneemkx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2snstowym.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xsgfmdjc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jbexaakg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rzfumvju.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2bojkvtmw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zdsjumjj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2teomcndc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fzvaqmsw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rgvldemx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fdmeddsz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2oehsieir.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2tlbvjifk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qrhpimpy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kfufbpay.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2yyschvmn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sjjbpczz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jliourvf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qfgnxbxd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2lodlytdy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rzdziqvk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mjyxbojp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqdfldxb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wztfncor.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2thukdaij.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2axvzawum.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jqjnfsik.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tbxslsba.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xeuygvlm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kgkozlcn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fmgoqfot.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cfoazbtk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zytyrctj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mpvegpvm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hhiiqwgd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rcefhwih.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fyabxzml.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jjyskeym.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ostmcphb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jtdaihho.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ldlzygel.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ybiivnhi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2frjrurxw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nydcdaze.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mhsosagr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2blgpdrxb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rvyipbdp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eplmnwyw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2upxtxmfp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zdfvupsc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2axlntihv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dlvuckuh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mslmgrck.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fskpiuri.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vyqmcrmq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2qpyxcjgb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kigtkvda.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tpvzpteo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nfuiitpu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zksxmwzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmtfnosq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bvntuqrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjmeamnl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gyvwkxal.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2seengqzt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fruwmdnq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2empwuusl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xmytcnnt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2zasnmrgh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qxyzdsce.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jxbeijiv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lfnsstej.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vjkdjaxs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhapkbw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nluawedy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2iwsiluew.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nurzcmjx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ljrrdcnz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zrdexvwm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mpuoesvf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cbqwptkt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tytapmch.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wmldzxob.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ncdihswd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dydkickq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cdumxaoh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2plvocdmj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gpgxoqrd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zwofonly.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2scrkhsbu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fywvfrtf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wheiwylg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qggkpule.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2twudyrwy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fqlrjmcm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hlwhdhmf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qbbzhnmw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fkkufdqf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uizhfosy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fsnmhuxm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rsjurnrl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bmkrerkg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lboagnan.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2clfpghpo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lhdutako.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fdcoklpi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uaftjmms.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2otapmgkn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qiwjyqta.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rohdecba.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pwhptmnq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jdupmxzv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mbhmjfdu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2uwahgxko.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nbkjinge.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fdqbxxja.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2muxellev.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zotoxpux.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xbrvczyr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wdgpzvfp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2oiwdizjw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uvyhqiar.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ebyffnek.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kjukjdyr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ibxcyxss.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ydrcgkxw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uqaijkkn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lhjzhquz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mjttpbzn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2klgtedhz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjjpvuit.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qwkdugig.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fjrircpk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kflxtnyv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lirgmsrq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2svnlwhlg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzqcmor.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2cmenihtt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rclfjwfl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vzajcequ.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xrfuomjd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mdqyfnbf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fbgnkmti.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qesgcert.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zrnudxrb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fswfpaif.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2blxwdcez.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2euqthibg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ejmrbwbv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2scilttad.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kptcnxss.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2aywaimjz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qznxdpas.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2crbiwvav.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2rgvcejxe.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2titkysbn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hdznalbr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mxkjfuqv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2viuabvaz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ukwsdafc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ztsosptt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jxarmfyi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbssdiuj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2erhuecdl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2trafsoms.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bxhoudqu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2idecgbgh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2folxesoa.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zhcqtgre.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2onqafogb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2beausqjv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ruqmiqlg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2iqedxfrj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2peurbzeo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hszyijhm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2sfivdaqs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ryiwvbou.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2uwjpjxgr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zfbhafgw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2sjuzdwiv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tfabnuie.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2auayivna.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wdrqexhj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zmkjczzb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2evlioxxm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2swsmovoc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2toylutdw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vcvyukty.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jnzuyptx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ymxijtar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbjqfiyx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2twmpmdeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgdnulvk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wmmonckn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qotuxuof.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2niczjrck.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hrzclhvr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fsuhhebo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qyipjxpq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nqpgtmnl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2cmcieyvn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xayjnchw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2byrzpknc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mzfslxwn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jwuvtnma.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2npbzowpc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2czthprtf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2chtqtdnl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nbzyxyzq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tvmzgaoz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dsdhjjci.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xiradfur.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lhbplcna.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mypyknwt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qxfjitje.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2csfzzrtv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aoohbjyv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zyngaooz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2pqcwumkm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sndatobl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fxqidffl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2abyuabxl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eeacclvl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sngkusgc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zaejjget.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ltjpbdps.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qxcxlbkh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wcwhnsal.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2atxoorcz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mbburvxj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpvdgmgu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nhixqccu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2umfhmnai.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zsbfuute.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rzybvzku.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kpgtfuqg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xnsjjuaq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jawfmeyk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yjxkvdmg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bqbsaybg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lloifdew.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fegwnybe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uobgpjzz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rkunbylu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2outhxydr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fcwgteoq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2uacmajhf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jjgaimhr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2sixjwpay.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jwjbvpgb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vokjebbh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mcsarfet.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2auohpdex.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hhfzklnq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hixyztie.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cdqaumne.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2mjaofjxs.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2adrimfky.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mbvypgwx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gnwseqwm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xlfqmhjk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xbmhtczi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rhsagefd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gprgocyq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2shmfclgj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vkjzefnr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zarkltjd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vpxyvfut.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dhqgkixm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fiwxgvrn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ykjgugmz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ckbgowfq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2utiwbund.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kxzalcur.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ksdadsfe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2msozlyvv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vluzgjzl.html


<!-- 参考信息 -->