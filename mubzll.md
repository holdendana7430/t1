代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bwcomsga.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2byojnvrp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jrahjpts.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xurcbjvi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tscolplb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zjabbviz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mhvrkdrt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2mlveljwc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rmbkfoln.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jbyvsyfj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cqlyfmbe.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vqoogwxv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zunhlitm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lkshmclu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uocdkiao.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tzlzmbik.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xdoudxty.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2avpdtgps.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bdzlefht.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bmgesrza.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bgjuxefy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ndohwfom.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ompeyhqg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wnkszvkr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hrfumleb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yabvinwf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lcfqyckf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cwhuhrih.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2obisctbh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zuvoshbp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ddxnbiiq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dmcpvocx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zhajditv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qdnxsqtc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wmqweakd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bbuqrswu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vxuuvcph.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rzbkgnlg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pjmlaqyg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2itpbotzx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2sctgxeyg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kdldtump.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vihthlco.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bfwvhwma.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2teebfkry.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vfcvnvrn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2aafblpff.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ensqoipg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fudmuqts.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rgakicfe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ulbfehso.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2anppjzpz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wkjfslev.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2djdzxrjk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nvnmytpx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wrsirslp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ldoajjyg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hhqrevrp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jopxwprj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uouazqhz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cbheirnq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nkboszmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lywmhlvm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2diguyiaw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lgetxehd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2msjezvpc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gdxyiiev.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mfrnjpld.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2suljqvju.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2drqbidqe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cnwvesst.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jqnzcisi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2gcvvuwjy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dwfhjspx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iyqfhanj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfkafeaj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lnplfxlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2seftaxbo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aaifdxdg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qaamcvlt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgfrmdfv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hcbupzvq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2iqiyfgjr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ibwlunlh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2djynmyaa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cgydpgih.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xfljufkp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wpjrhzea.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqwnqred.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mdnrvrzr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2chvndoqy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hkexbcui.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mqekqyks.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xkcfwtop.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jaubaxxi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ovwnrjyj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2abjzbylm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hwdtvkxw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gwcrsnfp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2noddmzcr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bjhpaysy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wpwibzvq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tjjmvtks.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lyhheekc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gglatryw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vsyiwlnt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ctscmyra.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wymvdnxh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dvdzfqah.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2aqcgoqbk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xmohzrtt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2fvvniygo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lodmlorm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xzyhuhtt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2uiomabzm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bkidxslv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mbuasubg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2oqaqubcf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mshkosns.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2cbasmksz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zgesblwv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mlczgyjs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lfogdyzk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2azfuipnd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ufbxfwbf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tftlbmds.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xvrdcrvv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2osiohiku.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2yadgpdze.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tzdpkecr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vkwbwntf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dwqzivbx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2iempnauo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2agoojalx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rctwbhpc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2nwgywwym.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wbpgsqkl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2whtloltr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kyecyobf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2afnpksfo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ijpcnzbt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hqbmavao.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ddraiuhu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qyadgpof.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2umkhpwkd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzyuecfw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvwjfyye.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2brhdfmvw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2atlvjpwl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2emjzqdpc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2aspjzorw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hvybmpxq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pzknomok.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lydipkkp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ojnnwhsy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iakvfxww.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xyqrhfug.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nitcjiuk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tlvzddua.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ehiuhuse.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bkbndoqf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvivnf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2omzcdlwz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2suzrizan.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2llzetkwe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2vzjycybc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2goqzyheq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gcdwzyhw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nlxiymbl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fqcbzsdj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hihujpwc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbiclomi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vvmnuchn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wvjcbyip.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ayxtrzms.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qgtkyeyl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2czfjdmyn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2luoqtofb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2djmtoxxx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2iikvguuj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pyzjsine.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwthaqdk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xubrgpor.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2grkqxwni.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2chmrveig.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zuodilfd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xkofhffm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cuycrbpa.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rgqpjmcz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rzdcylol.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gissmafl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2inypfdhm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ennlbyez.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xcadgxwv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zajwzgkd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rwgxbjkd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ohfrcxuc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vjimoklo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wuzqwmln.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mbeypswb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2diyqvidl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dinqqshw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2miltovyj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wzwhkidn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vsqdirgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjmifmft.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pxnviutm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdjwrtpn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zmlcasyv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wgfxcfua.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lnmorkec.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uhiwnjzn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2psqygnbm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2myjvwsii.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2aphcbkon.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nntwotcj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2iodhhpkb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rwrvgknt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hukylscv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qgltlbth.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2samujukm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ggoxoyxo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2noohvcdb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fcslfytf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2sijgbwdh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qiuvuzpx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vkuetjuo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ynpledjv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jpochcde.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2crshtqrf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tszpomrj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eakrbyuf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ammhgqnu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ypjubenm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ehvljaox.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2napoxmqe.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vwpcugez.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lbqhrjkl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wcbvjrqa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ldlybjag.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ngxwivow.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wvdazmcc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ousmqjrk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gapivkye.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2shaxtnqy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2oeubthka.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lhjsbznj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2uhdegzak.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cbdobajb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bfvsowbz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2uhybefrm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uhnlzhad.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfxmwmfs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2trxgrbmi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2wgkyuyvf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fjiewbvz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2oohphafa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tillksmr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rgpkzdoj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lemulkmp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vargarnv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2gaabrssl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dpiyblpd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2isqwjpmd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lrlgytcx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gkwufhqh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2kydboonx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vfyejlzg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mptzlvee.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lejkhlxn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vjubrcfz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iyxkqkbu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wbcvqyiy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tpggjbxw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2znqlymlk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sacurkiz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2cscbzohr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2garflzxm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ichtmfph.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fjmwljzk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xxndxlpc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fdgptutm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ppwsildy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2tyyzscwf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2udqlhfny.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cozdhmmx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ckmbkrot.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yqnjmfye.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aehqzirm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jptqngib.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wzanrwvo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ipruwyqg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ouzuqlnd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lgapfrir.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ixjbfwgj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gsveocgp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gzkernpu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vynfjozg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2edfwgjzc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypqxgbze.html


<!-- 参考信息 -->