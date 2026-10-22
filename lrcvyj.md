代发 wailian999

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wvlwnwfc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pkpccylb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zqutxxbs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2uqhwtizc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fiuatepc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xxempcme.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2eekdhntl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2zkjkjsrk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zjgyrdwy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jlzglwfg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2dnpgnfxy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2vvvnfyla.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lwhlxyhl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qlvmdbub.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qnxmyhxg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2loljfkjg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tvremlft.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2apzefxby.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wjptviif.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2imxiqgrb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cmhkbedx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2skjzxzfo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rattuoqa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ixhvcbbi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ngrnhmmz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2cswqtjhk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rlvqxtmm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wmpozpls.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hkrrqlyq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tnxbtkju.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lgridfbw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2inivnkez.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wehukeuu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bnxqzoav.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2axyjnqfd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2isvfsuiu.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tqljmgip.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2llllxbue.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2yfdeljbv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kvxjkyhl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ghwwfpaq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hbmtuwvs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2shpmnjdf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ggpxefqo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kwabgczw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjemgvtr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nxpsuzre.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xomqxtek.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2nxzpibct.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jnqeuvuw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xrdhvbxq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wboopfqi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xztshysi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bxabpvik.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jotgylra.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wziayydm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mdgfdcax.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2sfdubkpk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jweceqds.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dynfsoug.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pezyltlu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pnfhbgty.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ypztftlw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ztbbinef.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ipmgcvdo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ywtdilsv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2puwbgdky.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2sbzvlviu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kyqfomse.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tyybyzsr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xfsarmsv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vfnlgqaq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zilirbop.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lptxfqui.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2udlkhaie.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jtvcprlh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ugjbsmie.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fshewllv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ejgkcbdg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rmrfznis.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2aoobfbfb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ysyuwrdo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lmpkvtkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcnemznh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cwzzjbke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsybduez.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2prpyrxep.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gyfbyvxh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2slvoemgz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wipwphew.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ffqcfxvb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kexjygaj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hdenkggs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ijcqrwjx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xdtbdicx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nhjnxytu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlgthzku.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rexddbng.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2byjqwyth.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2puyjecgr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dlenrqpo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2otyxmvca.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2oenrftkn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wtlgfyms.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2mygwgsoq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bibixvuk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2actmtvgo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eupqctes.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zphpngqs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2umwkdqul.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dvsiosoz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cdjlysla.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2armyxeeg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qodqgnwh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hzjmbgci.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2thbrkwqj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nkfrxgir.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gdcchpyg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rcsagykq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2uqiqrtjd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vizjncvu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvkmhist.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xckoayvr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2efaxsnic.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fbrpgdbw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mdnpuiyg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zufibjgn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2uguaxmui.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ckcnigbr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qvkxljgy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zijuwljj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vnsjpoai.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vddpthtk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dfnqsgbw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gmsrpbjp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2htqvbmeh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lkiiismf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ecruxjor.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rfjprqmx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vlqzzrjj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2zqbkigzo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fdchbzzy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bbqaqfav.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vlblemfa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2breezsyx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmdhpyce.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wndufgvq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mglhvuaq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ebvryzrq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ailmrwgs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2kjshdxab.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tmxlufny.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jipkdenr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2codqzayv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jrwwatrk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2slezyjtp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fzmrlmof.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vrhrjljc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2suxnqrst.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2alemglin.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2olaczevj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nhtyzaia.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2oygublup.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2snutefry.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ynfexlqq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jcqoitvo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vioxubwi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lbzfzlzd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rzydzghu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kckskfoc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nlxsyvvu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tsrlwzaa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwualqfw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hqbnbzry.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjpalpcj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zishyuof.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2exfcpadm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2judtwzox.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2orojtxuv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2meotvtew.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2aghrlbgd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xboqcxmy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2gxhgqrzs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ctnklxnb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ypkiepzc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvvdaisj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fglugakq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ctylnvid.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xvyjzlhp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jycmmmbs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2kzqgsmvh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dndpyevb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ghulfpwo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xfpguksz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pemnbxwm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dpmamwsk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2refamqvf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2raknudwu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ltfvezob.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2uernvhjn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ikjrqgfu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kneekqfy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2anyhznfa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dimjsxay.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2qedinnyx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bpatobpq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ekceuzrr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yaswqaht.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxhjtwxx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vyzoweqq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dprisawb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bpvppnjy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wlhgvpzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2javqeqew.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vcdajjpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltiluilc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fuguuvpc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2epqiskhn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xhropcdk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ljczwzmr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lwbyuvcj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tfpbpvjw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cwwucnbo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qnfklhgk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gzcwtvln.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pbpfxqwc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lzrmgmiq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xatnscwq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bmqoeqab.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dljdydtw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jsqowvjk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lwrlktfv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2sqqwvfuv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dasgeqzy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hdnshthb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pppytdyt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2bigwdvov.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zsfjzikg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2uvfxyhqd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lgxddimv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mzwwjgmv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fcmptmjl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2eizhmysz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vcaezrfc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kopcekqz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kkqhwvyr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jokgmhke.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dkmgzbkc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ryuficpo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tkdsxzdx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kekdtetr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2fkuydaoi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jygihqyc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2mmeyfplj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pghwtbbp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnbzwaj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rwpgwtdu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2prxllkoe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2awmhxezg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwogjwuy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hzftvdln.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pjtjoeua.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ozgrenez.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2afqvvwgj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2bsxsjmel.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2yselyzws.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xiqecqrq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ldtxeiuw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jnfvfviz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2yzbfwnrj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pqogpygy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ewkbdsph.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mcwkkzql.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hbcjophy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ksasnqpd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ravwctoy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vadbwqxm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bwaixtia.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oykivrfb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2odtbmuii.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2klatqmmu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2snrwzhey.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qquqvtfp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2elpvhout.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lfhkvsdm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yeejbgen.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hzpnffjd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2aqcsmetv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2avegyryn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qeldipfq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pfzxxyuk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2wzxxfsmj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fhhqisma.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2popcnxgd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jhuppunp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rbqqcrat.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vmillydl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dauchxmr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tyljqtqf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xkyquvup.html


<!-- 参考信息 -->