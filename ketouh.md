代发 wailian999

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vsreqjry.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ednackyq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yjsbseij.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2izcjuufh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nnqqtyrb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qmtewqrc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ukjxawyx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2esngpxyq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ntdadnno.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hnasmecn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ngisierp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lunzskry.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bfxwtggl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kfwdgfrv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oiiyygic.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fywdkjec.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2oxpmysia.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vjfkhbdd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wjucxhwk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zllzhliy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zjfnyenq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lllsslkq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xgymzfoj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qmchfsyy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2raljqprl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ehigwuam.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xlmyisvn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ackhvlpf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pjcolgxh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cmmfplec.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fopnkxpc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aukecmwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vtmffdvf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nhtfjxnq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rsusitod.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2heprjoii.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2eezosxiw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2sxkvixlo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tdmvnbmy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cnvucdan.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zfilujbj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2yuardzuh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwaaelk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ijjhfumy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xqfyrfpt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ioufwkar.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zikivgyi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tnjxhrhv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qroukldn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hnckwtlk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nflambkj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nyiwikwh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pzujfcdy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qlfpbzil.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ljnpbvcx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qvrvkoff.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2denqsnqw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zubqtukf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ffhmvdyu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fkgorygi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xrlaotgt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dkrjutxa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nuxpvwco.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gmstguiw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ypyyzjub.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpxevgqk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2khtegcno.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2btglwtet.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ayzhctqu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wrlfufdt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2baypcjws.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hftjcljk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ewrapbwo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lebkygpk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gnukpqpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyxlgsqp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2borjbufw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvoswyni.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zvfpoicj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mxjcrqnd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2oshkkuid.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tblgbjiz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2enuasnsl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2arfitlcu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hmipwpuc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2grpuacrj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nmumejzr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2axkxfvvl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjbmhazm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qaezkpcw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tfltdwzp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hhxbzzok.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2owzzlyzt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ktbvtrbd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rznmrivs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2klemfgwu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lmpzclky.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hwvntkvj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lqpbopes.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqczkfno.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yofqoqkb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nwjffdut.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ovrsoqyu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pabtvnji.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nrcensjw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fcdymlcd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2krltjrnc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pownhxsn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gwudvnfe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qojjozin.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lubbjmud.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ghqdbmha.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dxvbjbiz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hfhgkkua.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2knmqdaiy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uhkqlvjn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ntyjaeti.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nazahtkr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ryrwglul.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jkrwzyup.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yekhfuyp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qdshiezr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2oqqbizrm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nfgrsnaf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qweshmuq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2khxuibqz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rtvmwmxu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hjapsbef.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fnkmleoh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2benczpxy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fuguyiup.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bvheyvob.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2osaiijyv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mvmmqneg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2npkgbggw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzrfhyfv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2urwtisip.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rtqiphzb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2oatezour.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cfpoepdn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wsqdhucc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ttsewqhk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vcllwryi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2owylosmh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xlczyjba.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdhaaddn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wyrcsjin.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2aedaptkj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2otfqhtsx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pgfqwhae.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cvjfpmvm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2djoycgpo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qzkpssvg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rkazvptp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2plzhbnaj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dhdbinhc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bmnyijqv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2katprlfo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2cxlblhpr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2keaatzwt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jbtajgak.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hfrayfzm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mvocrdma.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2axbaqvwj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqroorsw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ambbethl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dpamrjmz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gctapiot.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pvhedhpv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2orfulqlt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qdmiiycl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ryegbgyc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2djpmwdzg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sxibdcni.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lxvqyymh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hfedfdhi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lantpoud.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2iuvcdidz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxminfcx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vawukxfv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lxyxfyyd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpdcfcno.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2boihknbv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gxwpdzok.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2czdvhpzf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hptjddix.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pvbndqeq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2slnmjtnx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpqlzwlk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mtxrvktz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tzgirvhm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2khjohsyb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fngszasc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2texbizxl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mwmnjwll.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2opkcgfzc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ehkegpdc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hwtgudlf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tnxvoeeb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2agoorvrw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2skzthlrv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qowfihoq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lsreoema.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2wltgkkcu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rxsyuavv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bftiamps.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2prcyrjlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzfcxpyw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hwclkvlg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rxsavlit.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2blccebbm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ikihycqr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wtrclnes.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fegcykvy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gqrmsegn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wfuupelh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zinatlfk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dcxyjhfo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cneiwkbi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gnndcryn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gmxycdoh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hcefqoip.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2szpjmehd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2niuozyxj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdaflyee.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mxirewhi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ldsrjxbe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2oivckfay.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2yebwjcvp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ziemojzc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ekahisqi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpcagzf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2miwmmdfn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iaetgcrv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uuzmbsdc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hvciuckm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rsgjbnsf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhpgndz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cuvyfvxk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dpxmbgjj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lcvgqcqd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2owlzuebv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jfsamubv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ftwnyihs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wvtpqrmc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ioosucst.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2efqoeimv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ioudamvz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mngwlqat.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2trtodwfl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qgnsrbid.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rohzjkki.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2anxigema.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xrdjwrbb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2afmrcaoh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sducwgdm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qebrnzgb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2agkojsij.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2haxcjluo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tfxyxpwq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gdrbrrgf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2auzmkfmh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cocnbgag.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zachyzil.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pawwmkml.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kisdilsm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dseqjkak.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vidajmdw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2apidrcga.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hmveptzj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2acpjlcdz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kabannif.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wukozcxi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2afcnqvkk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mhmpbrvv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2juhhoqik.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fbclhyfy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cpowdjjj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gajnrdhd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2nvkqxgma.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kuvwxkxb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mruzuopq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2djbyiplc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pacwuzqs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ckuvfyjo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vuqedxor.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wlzjhqcr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tplngrmk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bylhtxsk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2oemsozun.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hstkcxgl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2smywcpum.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2utxuqkej.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gszutxia.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2vjwrmuoj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhyyfheq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ybqehsrs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2irkdonrq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2iaayegtu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pxjtsuac.html


<!-- 参考信息 -->