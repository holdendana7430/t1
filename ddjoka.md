代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gcmbykkp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zobfoafa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2awqfcnll.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppdtzxeo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pgnvjtid.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hkfywnso.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kavfaioz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kzpqvmmr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pgmibfub.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pxxomfvt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2keudbutr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2dxyqulqb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dmfwhhfq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2omvdshgh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bmiycuzt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2jowdlwvd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mzaobxxj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2eyjwvasi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xwycgdjt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rbclkywf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2teqfzoxu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2iukpdqqr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jandxmcq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2njeatqxb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nfkefbwd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2nkaxxsgr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hsjekmik.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cluwluxm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2peuxkcay.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2slwfwioq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2mpoimbqu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zbglyhcy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oktxlzuf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vtdutpoh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lmbntphb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hditeouj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2axkrijiy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jxmqsabg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qscmqmnn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gjewuhpt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2tisqwgff.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rloqfxjo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lflxpqwe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kpyhqagv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pdonvehd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tguqjbyv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qmljjppt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mdcooniw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2copzvcce.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zhmjhykt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uthltiqc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xhjdqmae.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ptwmkmxn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2emdecjhm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jptfvmsg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2eewuwyby.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2sxuuhvzi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2upzcqbox.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xkjvezcx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bpoqwgrw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ndphpdmx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rmieitob.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hottnaeo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2phajlmge.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wfveqvnu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zaoajlnb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2shahvtuk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tbaibppu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pcgslzaf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ydrxzner.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kmlwztse.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xwqjkpwd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2osiplbxk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ehwfqgpf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2oegieeyx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jblwrujx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rbujzcke.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2swafulun.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2rcnozdxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuirnfhc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vzdgkyhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pniizvti.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lqryiftg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ciqcciep.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxopyamz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mhjtlrbu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dvalbtxn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dscbaadu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2mchyllgw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2seowdgol.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nyzfhxvh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vipnlqjk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbedkjzw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zzevvxse.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mgiibcuz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ossxwwtb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dprbyakn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2srjnlwro.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vsxjdeui.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wtbaonvh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qyzafanq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pzopajzp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2uygljpox.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2szrxsgmk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bmmsvxmi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2amzigmpz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pdkgqrtf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2icpgklfq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2aekcahkt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ykcfcccq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hpowbker.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gvcarpxy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hyqnzsnh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qugtpqoo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kdeuerkd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kpoavoev.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfjmikjt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tuvrbpjb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2glnucpqk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ijemlfru.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2rloqdmor.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dvwjnhye.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dnfuazcb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2cjrcahic.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jqcalfwp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cfxafaeq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2svftejxe.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qyficlxx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2pdvdbsyu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2leuqswou.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jzhdfoho.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vhnnvwvb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2itkkdswk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gjtemhbb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tjpwnisl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mdlmhglu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wubcppfo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tymqxart.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ourysflm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lstkckjo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bhthqfrt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2awnitnof.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zxhciese.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nhkzetff.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2hwxqurqe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lglsfoxw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zkxvokkv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vafvbwmv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fkmrcauz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2opbqrvoc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sfuchand.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jrennlxu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rjiyvhuk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xzcyewma.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2shrtjipd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vfdrblzk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gfzgstfe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rljgmloy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ckjxceok.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kvczijvk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ugnjjsxv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rkudpgcs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zfhzsquy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xlhyxoze.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hcarallf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cuuaqxov.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ynojfofz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bxytyfaj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhuabguj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bfojnshh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2evspitkq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2quvmsynd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hxszguuw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2llzfoajz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vlqmxjij.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sluhlrko.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yymsigmz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ncocsozw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xmukdwih.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mhkjplli.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xtfmooyg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2njsivjmn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pnvwrqgm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pstplvxm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tfajflzo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wsqlgmaz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qcnxhces.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fwsfteag.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ctlqhkcs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qpuscbjl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2giuegqec.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jgetrsol.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibgzmscn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qimouhsx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vwbhjojq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jdtgqxbx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2oycsqyyl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2shhadewf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tlsqzzye.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2inutncwe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2oyghkzvs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hrsqtxhp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2azujgzpu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dbcpdmia.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gxdfpgeu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nvbridur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ulutptdi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kzzhrepq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dklqplnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsijvmya.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hqxrwilm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfvjkftb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ptzkhwto.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wlbxoazn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nylicavj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2yxtaydiw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2llewalyp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ezxcmwlx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hgldogoa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gymqjzzy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rjpjrguc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wpcnykkx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pbvricwz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lrwumout.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2etykkmty.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jmuaqnro.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ykfegfjo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xnirqlej.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lnokqgpa.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2luvsqhel.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdusynnv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ydzdulml.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yqdxlioe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jzhxrqkk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lfpjtsfa.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2upkdqkmz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ipsohqdx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjeiecvd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dgtspnln.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ojkacmqc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tdoqigol.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xicimmof.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2psohtcek.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2faowqskb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rukgwtjm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2blbfmjsz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uxichunc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2suhzpqss.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qlwpxitm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ivrgppye.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2syhwytug.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qrrlszvb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zagzeowr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zdnqctuy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qrikegfb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ikitestq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sicqdost.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vvsdwhtn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bmllrlqf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eroalkpa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tjkasatf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mkjdfvcz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dioxziru.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zjzmddbg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2czuhxvpw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xdhggryf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hyxsfrhk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2iahomcjw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wpglodiv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xhksutmt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zcxpsxpg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lsvyrqgm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iygbrjzd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dqajljzp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dfsjivok.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2szmczwnf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cpolnxpe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zkpecbew.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gokrspul.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hqkzdgxw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gfgejdzz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uhcslptq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kufvaafw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hikgqjin.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qtudcodo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vshbiuvk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dqgykcdj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2eyjzkuxv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2oevokkpv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xksczwrs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rhuetybo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vlwryymi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2klwlnhuy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lxvonzhg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tuuxvzkq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vueotndi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hecludne.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gqixrlek.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lbspkcvf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubfcdftu.html


<!-- 参考信息 -->